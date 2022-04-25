<script>
	export let project;
</script>

<div class="text-left mb-4 pb-4 bottom-separator">
	<div class="text-center">
		{#if project.website}
			<a href={project.website} rel="external" target="_blank" class="underline text-2xl"
				>{project.name}</a
			>
		{:else}
			<span class="text-indigo-500 text-2xl">{project.name}</span>
		{/if}
	</div>

	<div class="flex justify-end mt-4">
		<div class="text-sm text-right text-indigo-400">
			{project.start}
			/ {project.end}
		</div>
	</div>

	<div class="mt-4 text-sm text-justify">
		{#each project.description as description}
			<div class="mb-2">- {description}</div>
		{/each}
	</div>

	<div class="w-full flex flex-wrap">
		{#each project.tech as tech}
			<div
				class="bg-slate-700 font-bold rounded-sm py-0.5 px-1 text-xs mr-2 mt-2 whitespace-nowrap"
			>
				{tech}
			</div>
		{/each}
	</div>
</div>
