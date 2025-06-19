<script lang="ts">
	const { children } = $props();
</script>

<!-- Start Component -->
<nav>
	<ul>
		{@render children()}
	</ul>
</nav>
<!-- End Component -->
