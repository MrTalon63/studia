<script lang="ts">
	import Nav from '$lib/Nav.svelte';
	import Footer from '$lib/Footer.svelte';
	import Page from '$lib/Page.svelte';
</script>

<svelte:head>
	<title>Wideo | Radiokomunikacja i jej zasotowania</title>
</svelte:head>

<Nav />

<Page>
	<div class="px-8">
		<h1 class="py-8 text-center text-2xl font-bold">Materiały wideo</h1>
		<div class="p-4 text-justify">
			<video controls class="max-h-96">
				<source src="odc1.webm" type="video/webm" />
				Your browser does not support the audio element.
			</video>
			<h2>Tytuł: Historia radiokomunikacji, działanie fal radiowych</h2>
			<p>Autor: Marcin Czop</p>
			<p>Czas trwania: 5:39</p>
			<p>Rozmiar pliku: 25.1MB</p>
			<p>Data publikacji: 01.12.2024 12:33:34</p>
			<a href="odc1.webm" class="text-blue-700 hover:text-blue-950" download>Pobierz plik</a>
		</div>
		<hr />
		<div class="p-4 text-justify">
			<video controls class="max-h-96">
				<source src="odc2.webm" type="video/webm" />
				Your browser does not support the audio element.
			</video>
			<h2>Tytuł: Działanie radioodbiorników oraz ich protokoły</h2>
			<p>Autor: Marcin Czop</p>
			<p>Czas trwania: 10:12</p>
			<p>Rozmiar pliku: 40.9MB</p>
			<p>Data publikacji: 01.12.2024 12:52:45</p>
			<a href="odc2.webm" class="text-blue-700 hover:text-blue-950" download>Pobierz plik</a>
		</div>
		<hr />
		<div class="p-4 text-justify">
			<video controls class="max-h-96">
				<source src="odc3.webm" type="video/webm" />
				Your browser does not support the audio element.
			</video>
			<h2>Tytuł: Zasady działania sieci GNSS oraz radiokomunikacji satelitarnej</h2>
			<p>Autor: Marcin Czop</p>
			<p>Czas trwania: 6:28</p>
			<p>Rozmiar pliku: 23.2MB</p>
			<p>Data publikacji: 01.12.2024 13:10:19</p>
			<a href="odc3.webm" class="text-blue-700 hover:text-blue-950" download>Pobierz plik</a>
		</div>
		<hr />
	</div>
</Page>

<Footer />
