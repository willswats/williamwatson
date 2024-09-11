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
		margin: 2rem;
	}

	@media screen and (max-width: 768px) {
		section {
			margin: 1rem;
		}
	}
</style>
