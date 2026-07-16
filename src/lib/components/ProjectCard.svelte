<script lang="ts">
	interface Props {
		title: string;
		description: string;
		hrefProject?: string;
		hrefRepository: string;
	}

	let { title, description, hrefProject, hrefRepository }: Props = $props();
</script>

<figure>
	<figcaption>
		<h2>{title}</h2>
		<p>{description}</p>
	</figcaption>
	<section>
		{#if hrefProject}
			<a href={hrefProject} target="_blank" rel="noopener noreferrer">View Project</a>
		{/if}
		<a href={hrefRepository} target="_blank" rel="noopener noreferrer">View Repo</a>
	</section>
</figure>

<style>
	figure {
		display: flex;
		flex-direction: column;
		text-align: center;
		height: 25rem;
		border: 1px solid var(--color-muted);
		background-color: var(--background-color, '#000');
		background-image: var(--background-image, '');
		border-radius: var(--border-radius-large);
		overflow: hidden;
	}

	figure figcaption {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100%;
		margin: 0 1rem;
	}

	figure figcaption h2 {
		font-size: 2rem;
		text-decoration: underline;
	}

	figure figcaption p {
		font-size: 1.2rem;
	}

	figure section {
		display: flex;
	}

	figure section a {
		text-align: center;
		width: 100%;
		color: var(--color-text);
		background-color: var(--color-surface);
		border-top: 1px solid var(--color-muted);
		padding: 0.5rem;
		transition: background-color 0.1s;
		font-size: 1rem;
	}

	figure section a:hover {
		background-color: var(--color-highlight-med);
	}

	figure section a:nth-of-type(1) {
		border-right: 1px solid var(--color-muted);
	}
</style>
