<script lang="ts">
	import Nav from '$lib/Nav.svelte';
	import Footer from '$lib/Footer.svelte';
	import Page from '$lib/Page.svelte';
</script>

<svelte:head>
	<title>RSS | Radiokomunikacja i jej zasotowania</title>
</svelte:head>

<Nav />

<Page>
	<div class="flex-auto px-28">
		<h1 class="my-8 text-center text-3xl font-bold text-black">Kanały RSS</h1>
		<ul>
			<li>
				<a href="audio.rss" class="text-blue-700 hover:text-blue-950"
					>Kanał RSS dla materiałów audio</a
				>
			</li>
			<li>
				<a href="wideo.rss" class="text-blue-700 hover:text-blue-950"
					>Kanał RSS dla materiałów audio</a
				>
			</li>
		</ul>
	</div>
</Page>

<Footer />
