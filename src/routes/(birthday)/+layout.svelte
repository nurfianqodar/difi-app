<script lang="ts">
	import '../../app.css';
	import FooterBirthday21 from '../../components/ui/FooterBirthday21.svelte';
	let { children } = $props();
</script>

{@render children()}
<FooterBirthday21 />
