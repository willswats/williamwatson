<main>
	<section>
		<slot />
	</section>
	<slot name="footer" />
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
	}

	section {
		margin: 1rem;
	}
</style>
