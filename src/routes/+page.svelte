<main class="home">
	<section class="home__card">
		<section class="home__card-content">
			<h1>William Watson</h1>
			<h2>Web Developer</h2>
		</section>
		<section class="home__card-anchors">
			<a href="/about">About </a>
			<a href="/projects">Projects </a>
			<a href="/contact">Contact </a>
		</section>
	</section>
</main>

<style>
	.home {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: calc(100vh - 4rem); /* Account for Nav */
	}

	.home__card {
		display: flex;
		flex-direction: column;
		background-color: #2a2a2a;
		border: 1px solid #4a4a4a;
		margin: 2rem;
	}

	.home__card-content {
		display: flex;
		flex-direction: column;
		padding: 2rem;
	}

	.home__card-content h1 {
		font-size: 4rem;
	}

	.home__card-content h2 {
		font-size: 3rem;
	}

	.home__card-anchors {
		display: flex;
	}

	.home__card-anchors a {
		width: 100%;
		text-align: center;
		padding: 1rem;
		transition: background-color 0.1s;
		border-top: 1px solid #4a4a4a;
	}

	.home__card-anchors a {
		border-right: 1px solid #4a4a4a;
	}

	.home__card-anchors a:last-child {
		border-right: none;
	}

	.home__card-anchors a:hover {
		background-color: #4a4a4a;
	}

	@media screen and (max-width: 768px) {
		.home {
			height: calc(100vh - 8rem); /* Account for Nav and NavSocial */
		}

		.home__card-content h1 {
			font-size: 3rem;
		}

		.home__card-content h2 {
			font-size: 2rem;
		}

		.home__card-content {
			padding: 1rem;
		}
	}
</style>
