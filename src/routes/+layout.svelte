<script lang="ts">
	import Topnav from "../lib/Topnav.svelte";
</script>

<Topnav />
<main>
	<slot />
</main>

<style>
	:global(*) {
		font-family: 'Courier New', Courier, monospace;
	}
	main {
		padding: 5svh 15svw;
	}
</style>
