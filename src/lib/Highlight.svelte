<script lang="ts">
	export let c: string;
	export let href: string | undefined = undefined;

	$: if (!c.startsWith('#')) c = '#' + c;
</script>

<svelte:element
	this={href ? 'a' : 'span'}
	class="hl"
	style:--color={c}
	{href}
	target={href ? '_blank' : undefined}
	rel={href ? 'noopener noreferrer' : undefined}
>
	<slot />
</svelte:element>

<style lang="postcss">
	.hl {
		@apply inline-block;
		color: var(--color);
	}
</style>
