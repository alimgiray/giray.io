<script>
	export let stack;
	export let first;
	export let last;
</script>

{#if last}<span>&nbsp;and </span>{:else if !first}<span>, </span>{/if}
<a href={stack.url} rel="external" target="_blank" class="whitespace-nowrap"
	><img src={stack.logo} alt={stack.name} class="inline w-4 h-4 mr-1" />{stack.name}</a
>{#if last}.{/if}
