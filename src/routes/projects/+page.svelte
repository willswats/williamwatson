<main id="projects">
	<h1>Projects</h1>
	<section id="projects-grid">
		<figure class="projects-card">
			<figcaption class="projects-card-content">
				<h2>Review Charter</h2>
				<p>Visualise AniList data in multiple charts.</p>
			</figcaption>
			<section class="projects-card-anchors">
				<a href="https://review-charter.vercel.app/" target="_blank" rel="noopener noreferrer"
					>View Project</a
				>
				<a
					href="https://github.com/willswats/review-charter"
					target="_blank"
					rel="noopener noreferrer">View Repo</a
				>
			</section>
		</figure>

		<figure class="projects-card">
			<figcaption class="projects-card-content">
				<h2>Astrocats</h2>
				<p>A Unity Asteroids clone, but with cats.</p>
			</figcaption>
			<section class="projects-card-anchors">
				<a href="https://willswats.itch.io/astrocats" target="_blank" rel="noopener noreferrer"
					>View Project</a
				>
				<a href="https://github.com/willswats/astrocats" target="_blank" rel="noopener noreferrer"
					>View Repo</a
				>
			</section>
		</figure>

		<figure class="projects-card">
			<figcaption class="projects-card-content">
				<h2>React Pomodoro</h2>
				<p>A pomodoro timer.</p>
			</figcaption>
			<section class="projects-card-anchors">
				<a
					href="https://react-pomodoro-willswats.vercel.app"
					target="_blank"
					rel="noopener noreferrer">View Project</a
				>
				<a
					href="https://github.com/willswats/react-pomodoro"
					target="_blank"
					rel="noopener noreferrer">View Repo</a
				>
			</section>
		</figure>

		<figure class="projects-card">
			<figcaption class="projects-card-content">
				<h2>React Weather</h2>
				<p>A weather application.</p>
			</figcaption>
			<section class="projects-card-anchors">
				<a
					href="https://react-weather-willswats.vercel.app"
					target="_blank"
					rel="noopener noreferrer">View Project</a
				>
				<a
					href="https://github.com/willswats/react-weather"
					target="_blank"
					rel="noopener noreferrer">View Repo</a
				>
			</section>
		</figure>

		<figure class="projects-card">
			<figcaption class="projects-card-content">
				<h2>React Calculator</h2>
				<p>A calculator application.</p>
			</figcaption>
			<section class="projects-card-anchors">
				<a
					href="https://react-calculator-willswats.vercel.app"
					target="_blank"
					rel="noopener noreferrer">View Project</a
				>
				<a
					href="https://github.com/willswats/react-calculator"
					target="_blank"
					rel="noopener noreferrer">View Repo</a
				>
			</section>
		</figure>
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
		margin-top: 5rem;
		font-size: 3rem;
	}

	#projects h2 {
		font-size: 2rem;
	}

	#projects p {
		font-size: 1.2rem;
	}

	#projects-grid {
		display: grid;
		grid-template-columns: 1fr 1fr;
		flex-grow: 1;
		gap: 2rem;
		margin: 1rem 8rem;
	}

	.projects-card {
		display: flex;
		flex-direction: column;
		text-align: center;
		height: 25rem;
		border: 1px solid #4a4a4a;
	}

	.projects-card-content {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100%;
	}

	.projects-card:nth-of-type(1) .projects-card-content {
		background-color: #0b1622;
	}

	.projects-card:nth-of-type(2) .projects-card-content {
		background-color: #000;
	}

	.projects-card:nth-of-type(3) .projects-card-content {
		background-color: #7e201d;
	}

	.projects-card:nth-of-type(4) .projects-card-content {
		background-color: #10161d;
	}

	.projects-card:nth-of-type(5) .projects-card-content {
		background-image: linear-gradient(#dc8c00, #2b2b2b);
		background-color: #2b2b2b;
	}

	.projects-card:nth-of-type(6) .projects-card-content {
		background-color: rgba(0, 0, 0, 0.5);
	}

	.projects-card-anchors {
		display: flex;
	}

	.projects-card-anchors a {
		text-align: center;
		width: 100%;
		color: #fff;
		background-color: #2a2a2a;
		border-top: 1px solid #4a4a4a;
		padding: 0.5rem;
		transition: background-color 0.1s;
		font-size: 1rem;
	}

	.projects-card-anchors a:hover {
		background-color: #3a3a3a;
	}

	.projects-card-anchors a:nth-of-type(1) {
		border-right: 1px solid #4a4a4a;
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
