<script>
	import experiences from '../data/experiences.json';
	import projects from '../data/projects.json';
	import entries from '../data/education.json';

	import Work from '../components/Work.svelte';
	import Project from '../components/Project.svelte';
	import Education from '../components/Education.svelte';
</script>

<section>
	<div>
		{#each experiences as work}
			<Work {work} />
		{/each}
	</div>
	<!-- <div>
		{#each projects as project}
			<Project {project} />
		{/each}
	</div>
	<div>
		{#each entries as education}
			<Education {education} />
		{/each}
	</div> -->
</section>
