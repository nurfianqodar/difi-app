<script lang="ts">
	const { className }: { className?: string } = $props();
</script>

<svg
	xmlns="http://www.w3.org/2000/svg"
	width="24"
	height="24"
	viewBox="0 0 24 24"
	class={`${className} absolute -z-50 animate-bounce fill-purple-900 stroke-pink-500 opacity-30`}
>
	<g stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
		<path
			d="M7 9a4 4 0 0 0-4 4v6a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-6a4 4 0 0 0-4-4v0M7 9h10M7 9V6m10 3V6m-5 0v3m0-6h.01M7 3h.01M17 3h.01"
		/>
		<path d="M3 13c0 1 .6 3 3 3s3-2 3-3c0 1 .6 3 3 3s3-2 3-3c0 1 .6 3 3 3s3-2 3-3" />
	</g>
</svg>
