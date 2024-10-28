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
		margin: var(--margin, '');
	}

	@media screen and (max-width: 768px) {
		section {
			margin: var(--margin-breakpoint, '');
		}
	}
</style>
