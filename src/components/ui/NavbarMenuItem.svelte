<script lang="ts">
	import type { Snippet, SvelteComponent } from 'svelte';

	const { children, href }: { children?: Snippet; href: string } = $props();
</script>

<!-- Start Component -->
<li>
	<a {href}>
		{#if children}
			{@render children()}
		{:else}
			{href}
		{/if}
	</a>
</li>
<!-- End Component -->
