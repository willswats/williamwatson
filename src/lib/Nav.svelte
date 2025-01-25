<script lang="ts">
	import { page } from '$app/state';

	let navMobileActive: boolean = false;

	const toggleNavMobile = () => {
		navMobileActive = !navMobileActive;
	};
</script>

<button
	class="nav-overlay"
	class:nav-overlay-enabled={navMobileActive}
	onclick={toggleNavMobile}
	aria-label="Nav overlay"
></button>

<nav>
	<a class="nav-logo" href="https://williamwatson.dev"><span>williamwatson.dev</span></a>
	<button class="nav-menu" class:nav-menu-enabled={navMobileActive} onclick={toggleNavMobile}>
		<a href="/" class:nav-menu-a-enabled={page.url.pathname == '/'}>Home</a>
		<a href="/about" class:nav-menu-a-enabled={page.url.pathname == '/about'}>About</a>
		<a href="/projects" class:nav-menu-a-enabled={page.url.pathname == '/projects'}>Projects</a>
		<a href="/contact" class:nav-menu-a-enabled={page.url.pathname == '/contact'}>Contact</a>
	</button>

	<button onclick={toggleNavMobile}>
		<img alt="Burger Menu" src="svg/menu.svg" />
	</button>
</nav>

<style>
	nav {
		position: fixed;
		top: 0;
		z-index: 1;
		display: flex;
		width: 100%;
		height: 4rem;
		background-color: #2a2a2a;
		border-bottom: 1px solid #4a4a4a;
		overflow: hidden;
	}

	.nav-logo {
		display: flex;
		align-items: center;
		font-size: 1.5rem;
		width: 100%;
		transition: background-color 0.1s;
	}

	.nav-logo:hover {
		background-color: #3a3a3a;
	}

	.nav-logo span {
		padding: 1rem;
	}

	.nav-menu {
		display: flex;
		text-wrap: nowrap;
	}

	.nav-menu a {
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 1rem;
		font-size: 1.2rem;
		border-left: 1px solid #4a4a4a;
		transition: background-color 0.1s;
	}

	.nav-menu a:hover {
		background-color: #3a3a3a;
	}

	.nav-menu-a-enabled {
		background-color: #3a3a3a;
	}

	nav img {
		display: none;
	}

	.nav-overlay {
		position: fixed;
		width: 100%;
		height: 100%;
		top: -10000px;
		left: 0;
		right: 0;
		bottom: 0;
		background-color: rgba(0, 0, 0, 0.5);
	}

	@media screen and (min-width: 768px) {
		.nav-menu {
			margin-right: 4rem; /* Account for NavSocial */
		}
	}

	@media screen and (max-width: 768px) {
		.nav-menu {
			flex-direction: column;
			position: fixed;
			top: -10000px;
			width: 100%;
		}

		.nav-menu-enabled {
			top: 4rem;
		}

		.nav-menu a {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			flex-grow: 1;
			width: 100%;
			background-color: #2a2a2a;
			border: none;
			border-bottom: 1px solid #4a4a4a;
		}

		nav img {
			display: block;
			cursor: pointer;
			padding: 1rem;
			transition: background-color 0.1s;
			border-left: 1px solid #4a4a4a;
		}

		nav img:hover {
			background-color: #3a3a3a;
		}

		.nav-overlay-enabled {
			top: 0;
		}
	}
</style>
