<script lang="ts">
	import Nav from '$lib/components/Nav.svelte';
	import NavSocial from '$lib/components/NavSocial.svelte';
</script>

<Nav />
<slot />
<NavSocial />

<style>
	:root {
		--color-base: #191724;
		--color-surface: #1f1d2e;
		--color-overlay: #26233a;
		--color-muted: #6e6a86;
		--color-subtle: #908caa;
		--color-text: #e0def4;
		--color-love: #eb6f92;
		--color-gold: #f6c177;
		--color-rose: #ebbcba;
		--color-pine: #31748f;
		--color-foam: #9ccfd8;
		--color-iris: #c4a7e7;
		--color-highlight-low: #21202e;
		--color-highlight-med: #403d52;
		--color-highlight-high: #524f67;

		--border-radius-normal: 6px;
		--border-radius-large: 12px;
	}

	:global {
		@font-face {
			font-family: 'JetBrainsMono-Regular';
			src: url('/fonts/JetBrains_Mono/JetBrainsMono-VariableFont_wght.ttf');
		}

		* {
			margin: 0;
			padding: 0;
			box-sizing: border-box;
			font-family: JetBrainsMono-Regular, sans-serif;
			scroll-behavior: smooth;
		}

		body {
			color: var(--color-text);
			background-color: var(--color-base);
			/* Accout for the Nav */
			margin-top: 4rem;
		}

		a {
			text-decoration: none;
			color: inherit;
		}

		button,
		input[type='submit'],
		input[type='reset'] {
			background: none;
			color: inherit;
			border: none;
			padding: 0;
			font: inherit;
			outline: inherit;
		}

		@media screen and (min-width: 768px) {
			body {
				/* Account for the NavSocial */
				margin-left: 4rem;
			}
		}

		@media screen and (max-width: 768px) {
			body {
				/* Account for the NavSocial */
				margin-bottom: 4rem;
			}

			html {
				font-size: 10px;
			}
		}
	}
</style>
