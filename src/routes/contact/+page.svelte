<main class="contact">
	<section class="contact__card">
		<h1>Contact</h1>
		<p>Email: <a href="mailto:william@williamwatson.dev">william@williamwatson.dev</a></p>
		<p>
			GitHub: <a target="_blank" rel="noopener noreferrer" href="https://github.com/willswats"
				>github.com/willswats</a
			>
		</p>
		<p>
			LinkedIn: <a
				target="_blank"
				rel="noopener noreferrer"
				href="https://www.linkedin.com/in/willswats/">linkedin.com/in/willswats</a
			>
		</p>
	</section>
</main>

<style>
	p {
		font-size: 1.2rem;
	}

	.contact {
		display: flex;
		flex-direction: column;
		align-items: center;
		height: calc(100vh - 4rem); /* Account for Nav */
		margin: 0 2rem;
	}

	.contact__card {
		display: flex;
		flex-direction: column;
		width: 100%;
		background-color: #2a2a2a;
		border: 1px solid #4a4a4a;
		margin: 2rem;
		padding: 2rem;
	}

	.contact__card h1 {
		font-size: 3rem;
	}

	.contact__card p {
		font-size: 1.2rem;
	}

	.contact__card a {
		color: rgba(255, 165, 0, 1);
		transition: color 0.1s;
	}

	.contact__card a:hover {
		color: rgba(255, 165, 0, 0.8);
	}

	@media screen and (max-width: 768px) {
		.contact {
			height: calc(100vh - 8rem); /* Account for Nav and NavSocial */
		}
	}
</style>
