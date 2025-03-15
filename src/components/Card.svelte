<script module>
	import type { Snippet } from 'svelte';

	interface Props<T> {
		data?: T[];
		children?: Snippet;
		row?: Snippet<[T]>;
	}
</script>

<script lang="ts" generics="T">
	let { data, children, row }: Props<T> = $props();
</script>

<div class="card p-8 flex flex-col items-center text-center">
	{#if row && data}
		{#each data as d}
			{@render row(d)}
		{/each}
	{:else if children}
		{@render children()}
	{:else}
		fallback content
	{/if}
</div>

<style>
	.card {
		margin: 8px;
		background-color: #FFFDFD;
		border-radius: 8px;
		flex: 1;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
</style>