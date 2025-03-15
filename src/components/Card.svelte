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

<div class="p-8 bg-[#FFFDFD] rounded-lg flex flex-col flex-grow justify-center items-center text-center">
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
</style>