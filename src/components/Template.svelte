<script module>
	// module-level logic goes here
	// (you will rarely use this)
	import type { Snippet } from 'svelte';

	interface Props<T> {
		data?: T[];
		children?: Snippet;
		row?: Snippet<[T]>;
	}
</script>

<script lang="ts" generics="T">
	// instance-level logic goes here
	let { data, children, row }: Props<T> = $props();
</script>

{#if row && data}
	{#each data as d}
		{@render row(d)}
	{/each}
{:else if children}
	{@render children()}
{:else}
	fallback content
{/if}

<style>
	/* styles go here */
</style>