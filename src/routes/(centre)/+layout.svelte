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
		justify-content: center;
		align-items: center;
		height: calc(100vh - 4rem); /* Account for Nav */
	}

	section {
		margin: 0 2rem;
	}

	@media screen and (max-width: 768px) {
		main {
			height: calc(100vh - 8rem); /* Account for Nav and NavSocial */
		}

		section {
			margin: 0 1rem;
		}
	}
</style>
