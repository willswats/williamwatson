<script lang="ts">
	interface Props {
		title: string;
		description: string;
		hrefProject: string | null;
		hrefRepository: string;
		background: string;
	}

	let { title, description, hrefProject, hrefRepository, background }: Props = $props();
</script>

<figure>
	<figcaption>
		<h2>{title}</h2>
		<p>{description}</p>
		<enhanced:img alt="Project screenshot" src={`img/backgrounds/${background}`} />
		<div class="overlay"></div>
	</figcaption>
	<section>
		{#if hrefProject !== null}
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
		border-radius: var(--border-radius-large);
		overflow: hidden;
	}

	figure figcaption {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		width: 100%;
		height: 100%;
		position: relative;
		z-index: 1;
	}

	figcaption img {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		object-fit: contain;
		z-index: -1;
	}

	figcaption .overlay {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background-color: rgba(0, 0, 0, 0.6);
		z-index: 0;
	}

	figure figcaption h2 {
		font-size: 2rem;
		text-decoration: underline;
		position: relative;
		z-index: 1;
	}

	figure figcaption p {
		font-size: 1.2rem;
		position: relative;
		z-index: 1;
		margin: 0 1rem;
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
