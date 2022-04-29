<script>
	import info from '../data/info.json';
</script>

<footer class="px-8 py-4 text-sm flex justify-between border-t border-dashed border-indigo-300">
	{#each info.links as link}
		<a href={link.url} rel="external" target="_blank">{link.name}</a>
	{/each}
</footer>
