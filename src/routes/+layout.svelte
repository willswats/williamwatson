<script lang="ts">
	import '$src/global.css';
	import Nav from '$lib/components/Nav.svelte';
	import NavSocial from '$lib/components/NavSocial.svelte';
</script>

<Nav />
<slot />
<NavSocial />
