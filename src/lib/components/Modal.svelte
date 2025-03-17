<script>
    import { goto } from '$app/navigation';
	let { showModal = $bindable(), header, children } = $props();

	let dialog = $state(); // HTMLDialogElement

	$effect(() => {
		if (showModal) dialog.showModal();
	});
</script>

<!-- svelte-ignore a11y_click_events_have_key_events, a11y_no_noninteractive_element_interactions -->
<dialog
    class="w-full lg:w-1/3 m-auto max-h-3/4 overflow-scroll"
	bind:this={dialog}
	onclose={() => (showModal = false)}
	onclick={(e) => { if (e.target === dialog) dialog.close(); }}
>
	<div class="p-10 space-y-6 flex flex-col">
            <div class="space-y-4">
		    {@render header?.()}
            </div>
    		{@render children?.()}
		<!-- svelte-ignore a11y_autofocus -->
		<button class="px-4 py-2 bg-amber-300" autofocus onclick={() => {dialog.close(); goto('/contact')}}>Contact Us</button>
	</div>
</dialog>
