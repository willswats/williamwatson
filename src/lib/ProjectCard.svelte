<script lang="ts">
	export let title: string;
	export let description: string;
	export let hrefProject: string;
	export let hrefRepository: string;
</script>

<figure>
	<figcaption>
		<h2>{title}</h2>
		<p>{description}</p>
	</figcaption>
	<section>
		<a href={hrefProject} target="_blank" rel="noopener noreferrer">View Project</a>
		<a href={hrefRepository} target="_blank" rel="noopener noreferrer">View Repo</a>
	</section>
</figure>

<style>
	h2 {
		font-size: 2rem;
	}

	p {
		font-size: 1.2rem;
	}

	figure {
		display: flex;
		flex-direction: column;
		text-align: center;
		height: 25rem;
		border: 1px solid #4a4a4a;
	}

	figcaption {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100%;
		background-color: var(--background-color, '#000');
		background-image: var(--background-image, '');
	}

	section {
		display: flex;
	}

	section a {
		text-align: center;
		width: 100%;
		color: #fff;
		background-color: #2a2a2a;
		border-top: 1px solid #4a4a4a;
		padding: 0.5rem;
		transition: background-color 0.1s;
		font-size: 1rem;
	}

	section a:hover {
		background-color: #3a3a3a;
	}

	section a:nth-of-type(1) {
		border-right: 1px solid #4a4a4a;
	}
</style>
