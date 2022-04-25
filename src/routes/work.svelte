<script>
	import experiences from '../data/experiences.json';
	import Work from '../components/Work.svelte';
</script>

<section>
	<div>
		{#each experiences as work}
			<Work {work} />
		{/each}
	</div>
</section>
