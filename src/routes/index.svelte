<script context="module">
	export const prerender = true;
</script>

<script>
	import info from '../data/info.json';

	import Stack from '../components/Stack.svelte';
</script>

<section class="mt-4 text-justify w-full md:w-1/3 mx-auto">
	<h1 class="text-2xl text-center">
		I'm <a href="/">{info.name}</a>, a {info.role} from {info.country}
	</h1>
	<p class="mt-8">
		I build <a href="/work" class="underline">{info.work}</a>
		{@html info.description}
	</p>
	<p class="mt-4">
		My current stack is
		{#each info.stack as stack, i}
			<Stack {stack} first={i === 0} last={info.stack.length === i + 1} />
		{/each}
	</p>
	<p class="mt-4">
		Check out my <a href="projects" class="underline">projects</a> and
		<a href="education" class="underline">education</a>.
	</p>
</section>
