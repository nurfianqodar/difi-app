<script lang="ts">
	import type { Snippet } from 'svelte';

	const { children }: { children?: Snippet } = $props();
</script>

<!-- Start Component -->
<section>
	{#if children}
		{@render children()}
	{/if}
</section>
<!-- End Component -->
