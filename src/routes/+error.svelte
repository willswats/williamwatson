<script>
	import { page } from '$app/state';
	import PageH1 from '$lib/components/PageH1.svelte';
	import PageCentre from '$lib/components/PageCentre.svelte';
</script>

<svelte:head>
	<title>William Watson | {page.status}</title>
</svelte:head>

<PageCentre>
	<PageH1>{page.status} - {page.error ? page.error.message : ''}</PageH1>
</PageCentre>
