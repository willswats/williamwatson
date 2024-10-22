<script>
	import PageCentre from '$src/lib/PageCentre.svelte';
</script>

<svelte:head>
	<title>William Watson | Home</title>
</svelte:head>

<PageCentre>
	<section class="home-card">
		<section class="home-card-content">
			<h1>William Watson</h1>
			<h2>Software Engineering Student</h2>
		</section>
		<section class="home-card-anchors">
			<a href="/about">About </a>
			<a href="/projects">Projects </a>
			<a href="/contact">Contact </a>
			<a
				href="https://drive.google.com/file/d/1Vl1-7_JHQzl3BeTO-okZSHXxZaVd8b_E/view?usp=sharing"
				target="_blank"
				rel="noopener noreferrer">CV</a
			>
		</section>
	</section>
</PageCentre>

<style>
	.home-card {
		display: flex;
		flex-direction: column;
		background-color: #2a2a2a;
		border: 1px solid #4a4a4a;
	}

	.home-card-content {
		display: flex;
		flex-direction: column;
		padding: 2rem;
	}

	.home-card-content h1 {
		font-size: 4rem;
	}

	.home-card-content h2 {
		font-size: 2.5rem;
	}

	.home-card-anchors {
		display: flex;
	}

	.home-card-anchors a {
		width: 100%;
		text-align: center;
		padding: 1rem;
		transition: background-color 0.1s;
		border-top: 1px solid #4a4a4a;
	}

	.home-card-anchors a {
		font-size: 1.2rem;
		border-right: 1px solid #4a4a4a;
	}

	.home-card-anchors a:last-child {
		border-right: none;
	}

	.home-card-anchors a:hover {
		background-color: #4a4a4a;
	}

	@media screen and (max-width: 768px) {
		.home-card-content {
			padding: 1rem;
		}

		.home-card-content h1 {
			font-size: 3rem;
		}

		.home-card-content h2 {
			font-size: 2rem;
		}
	}
</style>
