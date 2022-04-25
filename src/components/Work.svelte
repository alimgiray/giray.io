<script>
	export let work;
</script>

<div class="text-left mb-4 pb-4 bottom-separator">
	<div class="text-center">
		{#if work.website}
			<a href={work.website} rel="external" target="_blank" class="underline text-2xl"
				>{work.company}</a
			>
		{:else}
			<span class="text-indigo-500 text-2xl">{work.company}</span>
		{/if}
	</div>

	<div class="flex justify-between mt-4">
		<div class="font-bold">{work.role}</div>
		<div class="text-sm text-right text-indigo-400">
			{work.start}
			/ {work.end}
		</div>
	</div>

	<div class="mt-4 text-sm text-justify">
		{#each work.description as description}
			<div class="mb-2">- {description}</div>
		{/each}
	</div>

	<div class="w-full flex flex-wrap">
		{#each work.tech as tech}
			<div
				class="bg-slate-700 font-bold rounded-sm py-0.5 px-1 text-xs mr-2 mt-2 whitespace-nowrap"
			>
				{tech}
			</div>
		{/each}
	</div>
</div>
