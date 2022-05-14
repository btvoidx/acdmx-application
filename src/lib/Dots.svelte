<script lang="ts">
	export let w: number = 10;
	export let h: number = w;
	export let x: string = '0px';
	export let y: string = '0px';
	export let color: string = 'white';
</script>

<table style:--x={x} style:--y={y} class="dots" style:--color={color}>
	{#each Array(h) as _}
		<tr>
			{#each Array(w) as _}
				<td>
					<i />
				</td>
			{/each}
		</tr>
	{/each}
</table>

<style lang="postcss">
	.dots {
		@apply fixed -z-10 opacity-30;
		left: var(--x);
		top: var(--y);
	}

	tr,
	td,
	i {
		@apply pointer-events-none;
	}

	tr:first-child > td:first-child,
	tr:last-child > td:last-child {
		@apply opacity-0;
	}

	i {
		@apply block w-1 h-1 m-1.5 rounded;
		background-color: var(--color);
	}
</style>
