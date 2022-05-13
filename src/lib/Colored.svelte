<script lang="ts">
	export let c: string;

	$: if (!c.startsWith('#')) c = '#' + c;
</script>

<span style:--color={c}>
	<slot />
</span>

<style lang="postcss">
	span {
		@apply inline-block;
		color: var(--color);
	}
</style>
