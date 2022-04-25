<script>
	import entries from '../data/education.json';
	import Education from '../components/Education.svelte';
</script>

<section>
	<div>
		{#each entries as education}
			<Education {education} />
		{/each}
	</div>
</section>
