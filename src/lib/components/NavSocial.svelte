<script lang="ts">
	import SvgGitHub from '$lib/assets/svg/github.svg';
	import SvgCodeberg from '$lib/assets/svg/codeberg.svg';
	import SvgLinkedIn from '$lib/assets/svg/linkedin.svg';
	import SvgCv from '$lib/assets/svg/cv.svg';
</script>

<nav>
	<a target="_blank" rel="noopener noreferrer" href="https://github.com/willswats">
		<img alt="GitHub" src={SvgGitHub} />
	</a>
	<a target="_blank" rel="noopener noreferrer" href="https://codeberg.org/willswats">
		<img alt="Codeberg" src={SvgCodeberg} />
	</a>
	<a target="_blank" rel="noopener noreferrer" href="https://www.linkedin.com/in/willswats/">
		<img alt="LinkedIn" src={SvgLinkedIn} />
	</a>
	<a
		target="_blank"
		rel="noopener noreferrer"
		href="https://drive.google.com/file/d/1Vl1-7_JHQzl3BeTO-okZSHXxZaVd8b_E/view?usp=sharing"
	>
		<img alt="CV" src={SvgCv} />
	</a>
</nav>

<style>
	nav {
		z-index: 999;
		position: fixed;
		bottom: 0;
		left: 0;
		right: 0;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--color-surface);
		border-top: 1px solid var(--color-muted);
	}

	nav a {
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 1rem;
		transition: background-color 0.1s;
		border-left: 1px solid var(--color-muted);
	}

	nav a:last-child {
		border-right: 1px solid var(--color-muted);
	}

	nav a:hover {
		background-color: var(--color-highlight-med);
	}

	nav a img {
		width: 2rem;
		height: 2rem;
	}

	@media screen and (min-width: 768px) {
		nav {
			position: fixed;
			left: 0;
			flex-direction: column;
			justify-content: end;
			border-top: 0;
			border-right: 1px solid var(--color-muted);
			height: 100%;
			width: 4rem;
		}

		nav a {
			width: 100%;
			border-left: 0;
			border-top: 1px solid var(--color-muted);
		}

		nav a:last-child {
			border-right: 0;
		}
	}
</style>
