<script lang="ts">
	import '../../app.css';
	import Navbar from '../../components/ui/Navbar.svelte';
	import NavbarLogo from '../../components/ui/NavbarLogo.svelte';

	let { children } = $props();
</script>

<Navbar>
	<NavbarLogo />
</Navbar>

{@render children()}
