<script>
	import projects from '../data/projects.json';
	import Project from '../components/Project.svelte';
</script>

<section>
	<div>
		{#each projects as project}
			<Project {project} />
		{/each}
	</div>
</section>
