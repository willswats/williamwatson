<script>
	import PageCentre from '$lib/components/PageCentre.svelte';
	import PageH1 from '$lib/components/PageH1.svelte';
</script>

<svelte:head>
	<title>William Watson | Contact</title>
</svelte:head>

<PageCentre>
	<PageH1 --margin-bottom="1rem">Contact</PageH1>
	<section>
		<p>Email: <a href="mailto:williamstuwatson@gmail.com">williamstuwatson@gmail.com</a></p>
		<p>
			GitHub: <a target="_blank" rel="noopener noreferrer" href="https://github.com/willswats"
				>github.com/willswats</a
			>
		</p>
		<p>
			LinkedIn: <a
				target="_blank"
				rel="noopener noreferrer"
				href="https://www.linkedin.com/in/willswats/">linkedin.com/in/willswats</a
			>
		</p>
	</section>
</PageCentre>

<style>
	section {
		display: flex;
		flex-direction: column;
		background-color: var(--color-surface);
		border: 1px solid var(--color-muted);
		border-radius: var(--border-radius-large);
		padding: 1rem;
	}

	section p {
		font-size: 1.2rem;
	}

	section a {
		color: var(--color-love);
		transition: color 0.1s;
	}
</style>
