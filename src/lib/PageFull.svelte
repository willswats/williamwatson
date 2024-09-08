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
		margin: var(--margin, '1rem');
	}

	@media screen and (max-width: 768px) {
		section {
			margin: var(--margin-breakpoint, '1rem');
		}
	}
</style>
