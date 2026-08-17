<script lang="ts">
	import PageFull from '$lib/components/PageFull.svelte';
	import ProjectCard from '$lib/components/ProjectCard.svelte';

	import ImgPeerTalk from '$lib/assets/img/backgrounds/peer-talk.png';
	import ImgReviewCharter from '$lib/assets/img/backgrounds/review-charter.png';
	import ImgReactWeather from '$lib/assets/img/backgrounds/react-weather.png';
	import ImgReactPomodoro from '$lib/assets/img/backgrounds/react-pomodoro.png';
	import ImgReactCalculator from '$lib/assets/img/backgrounds/react-calculator.png';
	import ImgAstrocats from '$lib/assets/img/backgrounds/astrocats.png';

	const backgrounds = [
		ImgPeerTalk,
		ImgReviewCharter,
		ImgReactWeather,
		ImgReactPomodoro,
		ImgReactCalculator,
		ImgAstrocats
	] as string[];

	import { projects as projectsJson } from '@/projects.json';

	interface projects {
		title: string;
		description: string;
		url: string | null;
		git: string;
	}

	const projects: projects[] = $state([]);

	for (const project of projectsJson) {
		projects.push({ ...project });
	}
</script>

<svelte:head>
	<title>William Watson | Projects</title>
</svelte:head>

<PageFull --margin="2rem 12rem" --margin-breakpoint="1rem">
	<section>
		{#each projects as project, index (index)}
			<ProjectCard
				title={project.title}
				description={project.description}
				hrefProject={project.url}
				hrefRepository={project.git}
				background={backgrounds[index]}
			/>
		{/each}
	</section>
</PageFull>

<style>
	section {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 1rem;
	}

	@media screen and (max-width: 1200px) {
		section {
			grid-template-columns: 1fr;
		}
	}
</style>
