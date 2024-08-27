<script>
	import PageH1 from '$lib/PageH1.svelte';
</script>

<svelte:head>
	<title>William Watson | Contact</title>
</svelte:head>

<PageH1>Contact</PageH1>
<section>
	<p>Email: <a href="mailto:william@williamwatson.dev">william@williamwatson.dev</a></p>
	<p>
		Matrix: <a
			target="_blank"
			rel="noopener noreferrer"
			href="https://matrix.to/#/@willswats:matrix.org">@willswats:matrix.org</a
		>
	</p>
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

<style>
	section {
		display: flex;
		flex-direction: column;
		background-color: #2a2a2a;
		border: 1px solid #4a4a4a;
		border-top: none;
		padding: 1rem;
	}

	section p {
		font-size: 1.2rem;
	}

	section a {
		color: rgba(255, 165, 0, 1);
		transition: color 0.1s;
	}

	section a:hover {
		color: rgba(255, 165, 0, 0.8);
	}
</style>
