<script>
	import { page } from '$app/stores';
	import PageH1 from '$lib/PageH1.svelte';
</script>

<svelte:head>
	<title>William Watson | {$page.status}</title>
</svelte:head>

<main>
	<PageH1>{$page.status} - {$page.error ? $page.error.message : ''}</PageH1>
</main>
