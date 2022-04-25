<script>
	import '../app.css';
	import Header from '../components/Header.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<svelte:head>
	<title>Giray</title>
	<meta name="description" content="Alim Giray Aytar - Fullstack Developer" />
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
