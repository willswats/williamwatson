<main class="about">
	<section class="about__card">
		<h1>About</h1>
		<p>
			I'm currently a student at the University of Portsmouth studying Software Engineering. I've
			built projects in my free time, as well as for Work Experience, College and University. You
			can view some of these projects on the <a href="/projects">Projects page</a>, and you can view
			all of them on my
			<a
				target="_blank"
				rel="noopener noreferrer"
				href="https://github.com/willswats?tab=repositories">GitHub</a
			>. If you would like to read more about me, you can read my
			<a
				href="https://drive.google.com/file/d/1Vl1-7_JHQzl3BeTO-okZSHXxZaVd8b_E/view?usp=sharing"
				target="_blank"
				rel="noopener noreferrer">CV</a
			>. If you would like to contact me, you can find my details on the
			<a href="/contact">Contact page</a>.
		</p>
	</section>
</main>

<style>
	.about {
		display: flex;
		flex-direction: column;
		align-items: center;
		height: calc(100vh - 4rem); /* Account for Nav */
	}

	.about__card {
		display: flex;
		flex-direction: column;
		background-color: #2a2a2a;
		border: 1px solid #4a4a4a;
		margin: 2rem;
		padding: 2rem;
	}

	.about__card h1 {
		font-size: 3rem;
	}

	.about__card p {
		font-size: 1.2rem;
	}

	.about__card a {
		color: rgba(255, 165, 0, 1);
		transition: color 0.1s;
	}

	.about__card a:hover {
		color: rgba(255, 165, 0, 0.8);
	}

	@media screen and (max-width: 768px) {
		.about {
			height: calc(100vh - 8rem); /* Account for Nav and NavSocial */
		}
	}
</style>
