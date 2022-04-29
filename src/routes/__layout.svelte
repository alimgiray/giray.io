<script>
	import info from '../data/info.json';

	import '../app.css';
	import Header from '../components/Header.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<svelte:head>
	<title>{info.name}</title>
	<meta name="description" content={info.content} />
</svelte:head>

<div class="flex flex-col justify-between min-h-screen">
	<div>
		<Header />
		<main class="p-8 pt-4">
			<slot />
		</main>
	</div>
	<Footer />
</div>
