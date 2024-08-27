<script>
	import PageH1 from '$lib/PageH1.svelte';
</script>

<svelte:head>
	<title>William Watson | About</title>
</svelte:head>

<main>
	<PageH1>About</PageH1>
	<section>
		<p>
			I'm currently a student at the University of Portsmouth studying Software Engineering. I've
			built projects in my free time, as well as for Work Experience, College and University. You
			can view some of these projects on the <a href="/projects">Projects page</a>, and you can view
			all of them on my
			<a
				target="_blank"
				rel="noopener noreferrer"
				href="https://github.com/willswats?tab=repositories">GitHub</a
			>. If you would like to read more about me, you can read my
			<a
				href="https://drive.google.com/file/d/1Vl1-7_JHQzl3BeTO-okZSHXxZaVd8b_E/view?usp=sharing"
				target="_blank"
				rel="noopener noreferrer">CV</a
			>. If you would like to contact me, you can find my details on the
			<a href="/contact">Contact page</a>.
		</p>
	</section>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		height: calc(100vh - 4rem); /* Account for Nav */
	}

	main section {
		display: flex;
		flex-direction: column;
		background-color: #2a2a2a;
		border: 1px solid #4a4a4a;
		margin: 0rem 1rem;
		padding: 2rem;
	}

	main section p {
		font-size: 1.2rem;
	}

	main section a {
		color: rgba(255, 165, 0, 1);
		transition: color 0.1s;
	}

	main section a:hover {
		color: rgba(255, 165, 0, 0.8);
	}

	@media screen and (max-width: 768px) {
		main {
			height: calc(100vh - 8rem); /* Account for Nav and NavSocial */
		}
	}
</style>
