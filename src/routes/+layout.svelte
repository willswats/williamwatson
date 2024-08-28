<script lang="ts">
	import '$src/global.css';
	import Nav from '$lib/Nav.svelte';
	import NavSocial from '$lib/NavSocial.svelte';
</script>

<Nav />
<slot />
<NavSocial />
