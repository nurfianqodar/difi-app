<script lang="ts">
	import type { Snippet } from 'svelte';

	const { children }: { children?: Snippet } = $props();
</script>

<!-- Start Component -->
<main class="flex w-screen items-center justify-center px-5 md:px-10">
	<div class="container">
		{#if children}
			{@render children()}
		{/if}
	</div>
</main>
<!-- End Component -->
