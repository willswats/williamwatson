<script lang="ts">
	import PageFull from '$lib/components/PageFull.svelte';
	import ProjectCard from '$lib/components/ProjectCard.svelte';
	import { projects as projectsJson } from '$src/projects.json';

	interface projects {
		title: string;
		description: string;
		url: string | null;
		git: string;
		background: string;
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
		{#each projects as project (project.title)}
			<ProjectCard
				title={project.title}
				description={project.description}
				hrefProject={project.url}
				hrefRepository={project.git}
				background={project.background}
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
