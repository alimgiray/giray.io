<script>
	import { page } from '$app/stores';
	import info from '../data/info.json';

	$: currentPage = $page.url.pathname;
</script>

<nav>
	<h1 class="text-3xl bottom-separator px-8 py-4">
		<a href="/" class="font-bold"
			><abbr title="Made with ❤️ in Anatolia 🐎" class="no-underline"
				>{info.name.toLocaleLowerCase()}</abbr
			></a
		>:${currentPage}
	</h1>
</nav>
