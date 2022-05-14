<script>
	import '../app.css';
</script>

<main>
	<slot />
</main>

<style lang="postcss">
	main {
		@apply min-w-full min-h-screen z-0;
		@apply bg-gradient-to-br to-[#030407] from-[#0a020a];
	}
</style>
