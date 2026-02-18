<script lang="ts">
    let { children, ...props } = $props();
</script>

<h2 class="text-3xl font-semibold underline decoration-amber-300 underline-offset-5">{@render children()}</h2>