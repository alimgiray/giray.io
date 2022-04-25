<script>
	export let education;
</script>

<div class="text-left mb-4 pb-4 bottom-separator">
	<div class="text-center">
		<span class="text-indigo-500 text-2xl">{education.name}</span>
	</div>

	<div class="flex justify-between mt-4">
		<div>
			{education.degree}, {education.field}
		</div>
		<div class="text-sm text-right text-indigo-400 whitespace-nowrap">
			{education.start}
			/ {education.end}
		</div>
	</div>
</div>
