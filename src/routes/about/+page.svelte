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
					Hi, I'm William. I recently graduated from the University of Portsmouth with a First in
					Software Engineering, where I collaborated closely with teammates across multiple modules,
					developing strong communication and project management skills, and built <a
						href="https://peer-talk.onrender.com/">Peer Talk</a
					>, a WebRTC web app for peer-to-peer text and voice communication, as my final year
					project.
				</p>

				<p>
					Outside of coding, I'm an avid Brazilian Jiu-Jitsu practitioner and a boulderer working my
					way up to V4s. I find that debugging code and solving climbing routes require the same
					patience and problem-solving mindset.
				</p>

				<p>
					I'm currently looking for my first graduate software engineering role. If you're hiring or
					just want to connect, drop me an email at <a href="mailto:william@williamwatson.dev"
						>william@williamwatson.dev</a
					>, or find me on <a href="https://www.linkedin.com/in/willswats/">LinkedIn</a>. In the
					meantime, feel free to browse my
					<a href="/projects">projects</a>
					or view my
					<a
						href="https://drive.google.com/file/d/1Vl1-7_JHQzl3BeTO-okZSHXxZaVd8b_E/view?usp=sharing"
						target="_blank"
						rel="noopener noreferrer">CV</a
					>.
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
		background-color: var(--color-surface);
		border: 1px solid var(--color-muted);
		border-radius: var(--border-radius-large);
		padding: 1rem;
	}

	figcaption p {
		margin-bottom: 1rem;
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
		height: 12rem;
		border: 1px solid var(--color-muted);
		border-radius: var(--border-radius-large);
		margin-right: 1rem;
	}

	@media screen and (max-width: 1200px) {
		section {
			width: 100%;
		}
	}

	@media screen and (max-width: 768px) {
		img {
			width: 8rem;
			height: 8rem;
		}

		figure p {
			font-size: 1rem;
		}
	}
</style>
