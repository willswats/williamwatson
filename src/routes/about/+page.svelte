<script>
	import PageCentre from '$src/lib/PageCentre.svelte';
	import PageH1 from '$lib/PageH1.svelte';
</script>

<svelte:head>
	<title>William Watson | About</title>
</svelte:head>

<PageCentre>
	<section>
		<PageH1>About</PageH1>
		<figure>
			<img alt="GitHub" src="png/ProfileWW.png" />
			<figcaption>
				<p>
					I'm a third year student at the University of Portsmouth studying Software Engineering.
					You can view some of my projects on the <a href="/projects">Projects page</a>, and you can
					view all of them on my
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
			</figcaption>
		</figure>
	</section>
</PageCentre>

<style>
	section {
		width: 55rem;
	}

	figure {
		background-color: #2a2a2a;
		border: 1px solid #4a4a4a;
		border-top: none;
		padding: 1rem;
	}

	figure p {
		font-size: 1.2rem;
	}

	figure a {
		color: rgba(255, 165, 0, 1);
		transition: color 0.1s;
	}

	figure a:hover {
		color: rgba(255, 165, 0, 0.8);
	}

	img {
		float: left;
		width: 8rem;
		border: 1px solid #4a4a4a;
		margin-right: 1rem;
	}

	@media screen and (max-width: 1000px) {
		section {
			width: 100%;
		}
	}
</style>
