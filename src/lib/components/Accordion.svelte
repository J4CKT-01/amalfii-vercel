<script lang="ts">
	import type { Snippet } from "svelte";

    interface AccordionProps {
        title: string;
        content: string;
        children?: Snippet;
    }
    let { title, content, children }: AccordionProps = $props();
    let isOpen = $state(false);
</script>

    <button onclick={() => isOpen = !isOpen} class="w-full flex flex-col p-4 border">
        <div class="w-full flex flex-row justify-between items-center">
            <h3 class="text-2xl {isOpen ? "underline decoration-amber-300" : " "}">{title}</h3>
            {#if isOpen}<i class="fa-duotone fa-regular fa-arrow-down text-2xl"></i>
            {:else}
            <i class="fa-duotone fa-regular fa-arrow-right text-2xl"></i> 
            {/if}
        </div>
        <div class="{isOpen ? "block" : "hidden"} text-xl text-left py-5">
            <p>{content}</p>
            {@render children?.()}
        </div>
    </button> 