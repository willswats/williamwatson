<main>
	<section id="home-card">
		<section id="home-card-content">
			<h1>William Watson</h1>
			<h2>Web Developer</h2>
		</section>
		<section id="home-card-anchors">
			<a
				class="home-card-anchor"
				href="https://drive.google.com/file/d/1Vl1-7_JHQzl3BeTO-okZSHXxZaVd8b_E/view?usp=sharing"
				target="_blank"
				rel="noopener noreferrer">CV</a
			>
			<a class="home-card-anchor" href="mailto:williamstuwatson@gmail.com">Contact </a>
		</section>
	</section>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: calc(100vh - 4rem);
		border-bottom: 1px solid #4a4a4a;
	}

	h1 {
		font-size: 4rem;
	}

	h2 {
		font-size: 3rem;
	}

	#home-card {
		display: flex;
		flex-direction: column;
		background-color: #2a2a2a;
		border: 1px solid #4a4a4a;
		margin: 2rem;
	}

	#home-card-content {
		display: flex;
		flex-direction: column;
		padding: 2rem;
	}

	#home-card-anchors {
		display: flex;
	}

	#home-card-anchors a {
		width: 100%;
		text-align: center;
		padding: 1rem;
		transition: background-color 0.1s;
		border-top: 1px solid #4a4a4a;
	}

	#home-card-anchors a:nth-child(1) {
		border-right: 1px solid #4a4a4a;
	}

	#home-card-anchors a:hover {
		background-color: #4a4a4a;
	}

	@media screen and (max-width: 768px) {
		h1 {
			font-size: 3rem;
		}

		h2 {
			font-size: 2rem;
		}

		#home-card-content {
			padding: 1rem;
		}
	}
</style>
