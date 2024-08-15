<script>
	// const overlay = document.querySelector('.overlay');
	// const navSvg = document.querySelector('.nav-svg');
	// const navMenu = document.querySelector('.nav-menu');
	//
	// const toggleNavMenu = () => {
	// 	if (window.innerWidth <= 768) {
	// 		navMenu.classList.toggle('enable');
	// 		overlay.classList.toggle('enable');
	// 	}
	// };
	//
	// const removeNavMenu = () => {
	// 	navMenu.classList.remove('enable');
	// 	overlay.classList.remove('enable');
	// };
	//
	// const resizeHandler = () => {
	// 	if (window.innerWidth > 768) {
	// 		removeNavMenu();
	// 	}
	// };
	//
	// navSvg.addEventListener('click', toggleNavMenu);
	// navMenu.addEventListener('click', toggleNavMenu);
	// overlay.addEventListener('click', removeNavMenu);
	// window.addEventListener('resize', resizeHandler);
</script>

<nav>
	<a id="nav-logo" href="https://williamwatson.dev"><span>williamwatson.dev</span></a>
	<section id="nav-menu">
		<a href="/">Home</a>
		<a href="/projects">Projects</a>
	</section>

	<img alt="Burger Menu" id="nav-svg" src="svg/menu.svg" />
</nav>

<style>
	nav {
		position: fixed;
		top: 0;
		z-index: 2;
		display: flex;
		width: 100%;
		height: 4rem;
		background-color: #2a2a2a;
		border-bottom: 1px solid #4a4a4a;
	}

	#nav-logo {
		display: flex;
		align-items: center;
		font-size: 1.5rem;
		width: 100%;
		transition: background-color 0.1s;
	}

	#nav-logo:hover {
		background-color: #3a3a3a;
	}

	#nav-logo span {
		padding: 1rem;
	}

	#nav-menu {
		display: flex;
	}

	#nav-menu a {
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 1rem;
		font-size: 1.5rem;
		border-left: 1px solid #4a4a4a;
		transition: background-color 0.1s;
	}

	#nav-menu a:hover {
		background-color: #3a3a3a;
	}

	nav img {
		display: none;
	}

	@media screen and (min-width: 768px) {
		#nav-menu {
			margin-right: 4rem;
		}
	}

	@media screen and (max-width: 768px) {
		#nav-menu {
			flex-direction: column;
			position: fixed;
			top: -10000px;
			width: 100%;
		}

		/* #nav-menu.enable { */
		/* 	top: 4rem; */
		/* } */

		#nav-menu a {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			flex-grow: 1;
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
	}
</style>
