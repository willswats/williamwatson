<script lang="ts">
	let active: boolean = false;
</script>

<nav class="nav">
	<button
		class="nav__overlay"
		class:nav__overlay--enabled={active}
		on:click={() => (active = !active)}
	></button>

	<a class="nav__logo" href="https://williamwatson.dev"><span>williamwatson.dev</span></a>
	<button class="nav__menu" class:nav__menu--enabled={active} on:click={() => (active = !active)}>
		<a href="/">Home</a>
		<a href="/about">About</a>
		<a href="/projects">Projects</a>
		<a href="/contact">Contact</a>
	</button>

	<button on:click={() => (active = !active)}>
		<img alt="Burger Menu" class="nav__svg" src="svg/menu.svg" />
	</button>
</nav>

<style>
	.nav {
		position: fixed;
		top: 0;
		z-index: 3;
		display: flex;
		width: 100%;
		height: 4rem;
		background-color: #2a2a2a;
		border-bottom: 1px solid #4a4a4a;
		overflow: hidden;
	}

	.nav__logo {
		display: flex;
		align-items: center;
		font-size: 1.5rem;
		width: 100%;
		transition: background-color 0.1s;
	}

	.nav__logo:hover {
		background-color: #3a3a3a;
	}

	.nav__logo span {
		padding: 1rem;
	}

	.nav__menu {
		display: flex;
		text-wrap: nowrap;
	}

	.nav__menu a {
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 1rem;
		font-size: 1.5rem;
		border-left: 1px solid #4a4a4a;
		transition: background-color 0.1s;
	}

	.nav__menu a:hover {
		background-color: #3a3a3a;
	}

	.nav img {
		display: none;
	}

	@media screen and (min-width: 768px) {
		.nav__menu {
			margin-right: 4rem; /* Account for NavSocial */
		}
	}

	@media screen and (max-width: 768px) {
		.nav__menu {
			flex-direction: column;
			position: fixed;
			top: -10000px;
			width: 100%;
			z-index: 2;
		}

		.nav__menu--enabled {
			top: 4rem;
		}

		.nav__menu a {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			flex-grow: 1;
			background-color: #2a2a2a;
			border: none;
			border-bottom: 1px solid #4a4a4a;
		}

		.nav img {
			display: block;
			cursor: pointer;
			padding: 1rem;
			transition: background-color 0.1s;
			border-left: 1px solid #4a4a4a;
		}

		.nav img:hover {
			background-color: #3a3a3a;
		}

		.nav__overlay {
			position: fixed;
			width: 100%;
			height: 100%;
			top: -10000px;
			left: 0;
			right: 0;
			bottom: 0;
			z-index: 1;
			background-color: rgba(0, 0, 0, 0.5);
		}

		.nav__overlay--enabled {
			top: 0;
		}
	}
</style>
