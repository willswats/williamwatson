<script lang="ts">
	import PageFull from '$src/lib/PageFull.svelte';
	import PageH1 from '$lib/PageH1.svelte';
	import ProjectCard from '$lib/ProjectCard.svelte';
</script>

<svelte:head>
	<title>William Watson | Projects</title>
</svelte:head>

<PageFull --margin="1rem 2rem" --margin-breakpoint="1rem">
	<PageH1 --margin-bottom="1rem">Projects</PageH1>
	<section>
		<ProjectCard
			title="Review Charter"
			description="Visualise AniList data in multiple charts."
			hrefProject="https://review-charter.vercel.app/"
			hrefRepository="https://github.com/willswats/review-charter"
			--background-color="#0b1622"
		/>
		<ProjectCard
			title="React Weather"
			description="A weather application."
			hrefProject="https://react-weather-willswats.vercel.app"
			hrefRepository="https://github.com/willswats/react-weather"
			--background-color="#10161d"
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
	<PageH1 --margin-top="1rem" --margin-bottom="1rem">Smaller Projects</PageH1>
	<section>
		<ProjectCard
			title="YouTube Alternative Switch"
			description="A Firefox extension for quickly switching videos between YouTube, Piped, Invidious and Chat Replay. "
			hrefProject="https://addons.mozilla.org/en-US/firefox/addon/youtube-alternative-switch/"
			hrefRepository="https://github.com/willswats/youtube-alternative-switch"
			--background-color="#7e201d"
		/>
		<ProjectCard
			title="The Stuffed Potato"
			description=" An example website for a takeaway restaurant."
			hrefProject="https://the-stuffed-potato.vercel.app/"
			hrefRepository="https://github.com/willswats/the-stuffed-potato"
			--background-color="rgba(0,0,0,0.5)"
		/>
	</section>
	<footer slot="footer">
		<p>
			View more of my projects on
			<a
				target="_blank"
				rel="noopener noreferrer"
				href="https://github.com/willswats?tab=repositories">GitHub</a
			>
		</p>
	</footer>
</PageFull>

<style>
	section {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 1rem;
	}

	footer {
		display: flex;
		justify-content: center;
	}

	footer a {
		color: rgba(255, 165, 0, 1);
		transition: color 0.1s;
	}

	footer a:hover {
		color: rgba(255, 165, 0, 0.8);
	}

	@media screen and (max-width: 1000px) {
		section {
			grid-template-columns: 1fr;
		}
	}
</style>
