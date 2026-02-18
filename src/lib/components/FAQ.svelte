<script lang="ts">
    import {Header, Accordion} from '$lib';
	import type { Snippet } from 'svelte';
    export type faq = {
        question: string;
        answer: string;
        children?: Snippet;
    }
    interface FAQProps {
        title: string;
        faq: Array<faq>;
    }
    let {title, faq}: FAQProps = $props();
</script>


<div class="w-full space-y-5">
	<Header>{title}</Header>
    {#each faq as faq}
	<Accordion
		title={faq.question}
		content={faq.answer}
	>
    {@render faq.children?.()}
    </Accordion>
    {/each}
</div>