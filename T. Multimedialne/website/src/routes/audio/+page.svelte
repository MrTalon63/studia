<script lang="ts">
	import Nav from '$lib/Nav.svelte';
	import Footer from '$lib/Footer.svelte';
	import Page from '$lib/Page.svelte';
</script>

<svelte:head>
	<title>Audio | Radiokomunikacja i jej zasotowania</title>
</svelte:head>

<Nav />

<Page>
	<div class="px-8">
		<h1 class="py-8 text-center text-2xl font-bold">Materiały audio</h1>
		<div class="p-4 text-justify">
			<audio controls>
				<source src="odc1.opus" />
				Your browser does not support the audio element.
			</audio>
			<h2>Tytuł: Historia radiokomunikacji, działanie fal radiowych</h2>
			<p>Autor: Marcin Czop</p>
			<p>Czas trwania: 5:39</p>
			<p>Rozmiar pliku: 2.59MB</p>
			<p>Data publikacji: 01.12.2024 12:32:32</p>
			<a href="odc1.opus" class="text-blue-700 hover:text-blue-950" download>Pobierz plik</a>
		</div>
		<hr />
		<div class="p-4 text-justify">
			<audio controls>
				<source src="odc2.opus" />
				Your browser does not support the audio element.
			</audio>
			<h2>Tytuł: Działanie radioodbiorników oraz ich protokoły</h2>
			<p>Autor: Marcin Czop</p>
			<p>Czas trwania: 10:12</p>
			<p>Rozmiar pliku: 4.67MB</p>
			<p>Data publikacji: 01.12.2024 12:45:54</p>
			<a href="odc2.opus" class="text-blue-700 hover:text-blue-950" download>Pobierz plik</a>
		</div>
		<hr />
		<div class="p-4 text-justify">
			<audio controls>
				<source src="odc3.opus" />
				Your browser does not support the audio element.
			</audio>
			<h2>Tytuł: Zasady działania sieci GNSS oraz radiokomunikacji satelitarnej</h2>
			<p>Autor: Marcin Czop</p>
			<p>Czas trwania: 6:28</p>
			<p>Rozmiar pliku: 2.97MB</p>
			<p>Data publikacji: 01.12.2024 13:01:21</p>
			<a href="odc3.opus" class="text-blue-700 hover:text-blue-950" download>Pobierz plik</a>
		</div>
		<hr />
	</div>
</Page>

<Footer />
