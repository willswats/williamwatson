<script>
	import PageCentre from '$lib/components/PageCentre.svelte';
	import PageH1 from '$lib/components/PageH1.svelte';
</script>

<svelte:head>
	<title>William Watson | About</title>
</svelte:head>

<PageCentre>
	<section>
		<PageH1 --margin-bottom="1rem">About</PageH1>
		<figure>
			<img alt="Myself" src="img/ProfileMe.jpg" />
			<figcaption>
				<p>
					I'm a University of Portsmouth graduate with a First-Class Honours in Software
					Engineering. You can view some of my projects on the <a href="/projects">Projects page</a
					>, and you can view all of them on my
					<a
						target="_blank"
						rel="noopener noreferrer"
						href="https://github.com/willswats?tab=repositories">GitHub</a
					>. If you would like to read more about me, you can read my
					<a
						href="https://drive.google.com/file/d/1Vl1-7_JHQzl3BeTO-okZSHXxZaVd8b_E/view?usp=sharing"
						target="_blank"
						rel="noopener noreferrer">CV</a
					>. If you would like to contact me, you can send an email to
					<a href="mailto:william@williamwatson.dev">william@williamwatson.dev</a>. Alternatively
					you can find my other socials on the sidebar.
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
		display: flex;
		background-color: var(--color-surface);
		border: 1px solid var(--color-muted);
		border-radius: var(--border-radius-large);
		padding: 1rem;
	}

	figcaption {
		display: flex;
		align-items: center;
	}

	figure p {
		font-size: 1.2rem;
	}

	figure a {
		color: var(--color-love);
	}

	figure a:hover {
		text-decoration: underline;
	}

	img {
		float: left;
		width: 12rem;
		border: 1px solid var(--color-muted);
		border-radius: var(--border-radius-large);
		margin-right: 1rem;
	}

	@media screen and (max-width: 1200px) {
		section {
			width: 100%;
		}
	}
</style>
