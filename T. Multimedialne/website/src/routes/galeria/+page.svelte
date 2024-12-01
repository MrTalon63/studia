<script lang="ts">
	import Nav from '$lib/Nav.svelte';
	import Footer from '$lib/Footer.svelte';
	import Page from '$lib/Page.svelte';

	export let images = [
		{
			thumb: 'imgs/thumb/IMG_0887.webp',
			src: 'imgs/full/IMG_0887.webp',
			alt: 'Maszt GSM na budynku Komagu',
			description: 'Maszt (GZB0025) przy ul. Łużyckiej 16 na budynku Komagu',
			title: 'Maszt BTS należacy do firmy Play',
			width: 800,
			height: 600
		},
		{
			thumb: 'imgs/thumb/IMG_0895.webp',
			src: 'imgs/full/IMG_0895.webp',
			alt: 'Maszt GSM na budynku wydziału AEiI Politechniki Śląskiej',
			description: 'Maszt przy ul. Akademickiej 16 na budynku wydziału AEiI PŚ',
			title: 'Maszt BTS będący częscią sieci NetWorkS!',
			width: 800,
			height: 600
		},
		{
			thumb: 'imgs/thumb/IMG_0898.webp',
			src: 'imgs/full/IMG_0898.webp',
			alt: 'Maszt GSM na budynku Rektoratu Politechniki Śląskiej',
			description: 'Maszt przy ul. Akademickiej 2 na budynku Rektoratu PŚ',
			title: 'Maszt BTS będący częscią sieci NetWorkS!',
			width: 800,
			height: 600
		},
		{
			thumb: 'imgs/thumb/IMG_0899.webp',
			src: 'imgs/full/IMG_0899.webp',
			alt: 'Maszt Jednostki Ratowniczo-Gaśniczej nr 1 w Gliwicach z dwoma antenami na pasmo VHF (149MHz)',
			description: 'Maszt z dwoma antenami na pasmo VHF',
			title: 'Maszt JRG nr 1 w Gliwicach',
			width: 800,
			height: 600
		},
		{
			thumb: 'imgs/thumb/IMG_0902.webp',
			src: 'imgs/full/IMG_0902.webp',
			alt: 'Maszt GSM na bloku mieszkalnym przy ul. Łużyckiej 2',
			description: 'Maszt przy ul. Łużyckiej 2 na bloku mieszkalnym',
			title: 'Maszt BTS będący częscią sieci NetWorkS!',
			width: 800,
			height: 600
		},

		{
			thumb: 'imgs/thumb/IMG_0922.webp',
			src: 'imgs/full/IMG_0922.webp',
			alt: 'Maszt GSM na budynku Komagu należący do firmy Plus',
			description: 'Maszt (BT24049) przy ul. Pszczyńskiej 37 na budynku Komagu',
			title: 'Maszt BTS należacy do firmy Plus',
			width: 800,
			height: 600
		},
		{
			thumb: 'imgs/thumb/IMG_0939.webp',
			src: 'imgs/full/IMG_0939.webp',
			alt: 'Maszt z możlwiością wejścia na niego. Na maszcie widać antenę wertykalną najpewniej na pasmo 174MHz. Pod nią na odskoczni widoczna jest o wiele mniejsza antena, najpewniej do systemu cyfrowego.',
			description:
				'Na szczycie widać antenę wertykalną na pasmo 174MHz, a pod nią antenę do systemu cyfrowego',
			title: 'Masz antenowy 3 komisariatu policji w Gliwicach z dwoma antenami',
			width: 800,
			height: 600
		},

		{
			thumb: 'imgs/thumb/IMG_0951.webp',
			src: 'imgs/full/IMG_0951.webp',
			alt: 'Dwie radiolinie firmy ubiquiti, AirFiber oraz najpewniej Loco M5. Na drugim maszcie obok widać antenę 5/8 na pasmo CB (27MHz) w nienajlepszym stanie',
			description:
				'Wyposażone w dwie radiolinie firmy ubiquiti - AirFiber oraz najpewniej Loco M5. Na drugim maszcie obok widać antenę 5/8 na pasmo CB (27MHz) w nienajlepszym stanie',
			title: 'Radiolinie firmy ubiquiti na pasmo 5GHz oraz antena 5/8 na pasmo CB',
			width: 800,
			height: 600
		},
		{
			thumb: 'imgs/thumb/IMG_0907.webp',
			src: 'imgs/full/IMG_0907.webp',
			alt: 'System wczesnego ostrzegania wyposażony w antenę typu zamkniętego dipola oraz syreny alarmowe',
			description: 'Wyposażony w antenę typu dipol oraz syreny alarmowe',
			title: 'System wczesnego ostrzegania na bydunku Wydziału Chemicznego PS',
			width: 800,
			height: 600
		},
		{
			thumb: 'imgs/thumb/IMG_0916.webp',
			src: 'imgs/full/IMG_0916.webp',
			alt: 'Instalacja antenowa na dachu bloku mieszkalnego. Anteny do użytku krótkofalarskiego, dwie anteny Yagi 3 elementowe najpewniej na pasmo 20m i 40m (14MHz i 7MHz). Widoczna jest jeszcze antena koolinearna, najewpniej Diamond X50',
			description:
				'Widoczne są 3 anteny, dwie anteny Yagi 3 elementowe najpewniej na pasmo 20m i 40m (14MHz i 7MHz) oraz antena koolinearna, najpewniej Diamond X50',
			title: 'Krótkofalarska instalacja antenowa na dachu bloku mieszkalnego',
			width: 800,
			height: 600
		},
		{
			thumb: 'imgs/thumb/IMG_0940.webp',
			src: 'imgs/full/IMG_0940.webp',
			alt: 'Instalacja antenowa na dachu bloku mieszkalnego. Anteny do użytku krótkofalarskiego, Yagi 6 elementowa na pasmo 2m (144MHz), QFH na pasmo 137MHz oraz antena koolinearna, najpewniej Diamond X200.',
			description:
				'Widoczne są 3 anteny, Yagi 6 elementowa na pasmo 2m (144MHz), QFH na pasmo 137MHz oraz antena koolinearna, najpewniej Diamond X200.',
			title: 'Krótkofalarska instalacja antenowa na dachu bloku mieszkalnego',
			width: 800,
			height: 600
		},
		{
			thumb: 'imgs/thumb/IMG_0957.webp',
			src: 'imgs/full/IMG_0957.webp',
			alt: 'Na maszcie widać dwie radiolinie firmy ubiquiti. Jedna to litebeam zapewne na 5GHz, a druga to Rocket 5AC z antena dookólną',
			description: 'Wyposażone w dwie radiolinie ubiquiti - litebeam oraz Rocket 5AC',
			title: 'Radiolinia na pasmo 5GHz zainstalowana na prywatnym maszcie',
			width: 800,
			height: 600
		}
	];

	let modalOpen = false;
	let selectedImage: { src: string; alt: string; description: string; title: string } | null = null;

	// Open the modal with the selected image
	function openModal(image: { src: string; alt: string; description: string; title: string }) {
		selectedImage = image;
		modalOpen = true;
		// Focus on the modal when it opens for accessibility
		setTimeout(() => {
			const modal = document.querySelector('.modal-content') as HTMLElement;
			if (modal) modal.focus();
		}, 100);
	}

	// Close the modal
	function closeModal() {
		modalOpen = false;
		selectedImage = null;
	}

	// Close modal when clicking outside or pressing Escape key
	function handleOverlayClick(event: MouseEvent) {
		if (event.target === event.currentTarget) {
			closeModal();
		}
	}

	function handleEscapeKey(e: KeyboardEvent) {
		if (e.key === 'Escape') closeModal();
	}
</script>

<svelte:head>
	<title>Galeria | Radiokomunikacja i jej zasotowania</title>
</svelte:head>

<Nav />

<Page>
	<div class="px-8">
		<h1 class="py-8 text-center text-2xl font-bold">Galeria</h1>

		<div class="p-6">
			<!-- Gallery Grid -->
			<div class="grid grid-cols-1 gap-6 sm:grid-cols-2 md:grid-cols-3">
				{#each images as { src, alt, description, thumb, title }}
					<div class="relative flex cursor-pointer flex-col">
						<button
							type="button"
							on:click={() => openModal({ src, alt, description, title })}
							on:keydown={(e) => e.key === 'Enter' && openModal({ src, alt, description, title })}
							class="relative cursor-pointer border-none bg-transparent p-0"
							aria-label="Open image modal"
						>
							<div class="relative">
								<img src={thumb} {alt} class="h-auto w-full rounded-lg object-cover shadow-lg" />
								<div
									class="absolute bottom-0 left-0 right-0 rounded-b-lg bg-black bg-opacity-75 p-2 text-sm text-white"
								>
									{title}
								</div>
							</div>
						</button>
					</div>
				{/each}
			</div>

			<!-- Modal for Full-Size Image -->
			{#if modalOpen}
				<div
					class="fixed inset-0 z-50 flex items-center justify-center bg-gray-900 bg-opacity-75"
					on:click={handleOverlayClick}
					on:keydown={handleEscapeKey}
					role="dialog"
					aria-modal="true"
					aria-labelledby="modal-title"
					aria-describedby="modal-description"
				>
					<div
						class="modal-content relative rounded-lg bg-white p-4 focus:outline-none"
						tabindex="-1"
					>
						<button
							on:click={closeModal}
							class="absolute right-2 top-1 text-6xl font-bold text-black"
							aria-label="Close modal"
						>
							&times;
						</button>
						{#if selectedImage}
							<div class="mx-auto w-full max-w-[90vw] sm:max-w-[80vw] lg:max-w-[75vw]">
								<img
									src={selectedImage.src}
									alt={selectedImage.alt}
									class="max-h-[80vh] w-full object-contain"
								/>
								<div class="mt-4 text-center">
									<h2 class="text-lg font-bold" id="modal-title">{selectedImage.title}</h2>
									<p class="mt-2 text-gray-700">{selectedImage.description}</p>
									<a
										class="mt-4 text-blue-700 hover:text-blue-950"
										href={selectedImage.src}
										target="_blank"
										rel="noopener noreferrer"
									>
										Otwórz w nowej karcie
									</a>
								</div>
							</div>
						{/if}
					</div>
				</div>
			{/if}
		</div>
	</div>
</Page>

<Footer />
