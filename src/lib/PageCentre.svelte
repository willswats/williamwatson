<main>
	<section>
		<slot />
	</section>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: calc(100vh - 4rem); /* Account for Nav */
	}

	section {
		margin: 1rem;
	}

	@media screen and (max-width: 768px) {
		main {
			height: calc(100vh - 8rem); /* Account for Nav and NavSocial */
		}
	}
</style>
