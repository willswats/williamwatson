<script lang="ts">
	import '../../global.css';
	import Nav from '$lib/Nav.svelte';
	import NavSocial from '$lib/NavSocial.svelte';
</script>

<Nav />
<main>
	<section>
		<slot />
	</section>
</main>
<NavSocial />

<style>
	main {
		display: flex;
		flex-direction: column;
	}

	section {
		margin: 1rem;
	}
</style>
