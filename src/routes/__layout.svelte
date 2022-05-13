<script>
	import '../app.css';
</script>

<main>
	<slot />
</main>

<style lang="postcss">
	main {
		@apply w-screen h-screen overflow-hidden;
		@apply bg-gradient-to-br from-[#030407] to-[#0e030e];
	}
</style>
