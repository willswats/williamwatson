<script>
	import ProjectCard from '$lib/ProjectCard.svelte';
</script>

<main id="projects">
	<h1>Projects</h1>
	<section id="projects-grid">
		<ProjectCard
			title="Review Charter"
			description="Visualise AniList data in multiple charts."
			hrefProject="https://review-charter.vercel.app/"
			hrefRepository="https://github.com/willswats/review-charter"
			--background-color="#0b1622"
		/>
		<ProjectCard
			title="Astrocats"
			description="A Unity Asteroids clone, but with cats."
			hrefProject="https://willswats.itch.io/astrocats"
			hrefRepository="https://github.com/willswats/astrocats"
			--background-color="#000"
		/>
		<ProjectCard
			title="React Pomodoro"
			description="A pomodoro timer."
			hrefProject="https://react-pomodoro-willswats.vercel.app"
			hrefRepository="https://github.com/willswats/react-pomodoro"
			--background-color="#7e201d"
		/>
		<ProjectCard
			title="React Weather"
			description="A weather application."
			hrefProject="https://react-weather-willswats.vercel.app"
			hrefRepository="https://github.com/willswats/react-weather"
			--background-color="#10161d"
		/>
		<ProjectCard
			title="React Calculator"
			description="A calculator application."
			hrefProject="https://react-calculator-willswats.vercel.app"
			hrefRepository="https://github.com/willswats/react-calculator"
			--background-color="#2b2b2b"
			--background-image="linear-gradient(#dc8c00, #2b2b2b)"
		/>
		<ProjectCard
			title="williamwatson.dev"
			description="My portfolio website (this website)."
			hrefProject="https://williamwatson.dev"
			hrefRepository="https://github.com/willswats/williamwatson-dev"
			--background-color="#1a1a1a"
		/>
	</section>
</main>

<style>
	#projects {
		display: flex;
		flex-direction: column;
	}

	#projects h1 {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		font-size: 3rem;
		margin-top: 1rem;
	}

	#projects-grid {
		display: grid;
		grid-template-columns: 1fr 1fr;
		flex-grow: 1;
		gap: 2rem;
		margin: 1rem 8rem;
	}

	@media screen and (max-width: 1100px) {
		#projects-grid {
			margin: 1rem 2rem 6rem 2rem;
		}
	}

	@media screen and (max-width: 768px) {
		#projects-grid {
			grid-template-columns: 1fr;
		}
	}
</style>
