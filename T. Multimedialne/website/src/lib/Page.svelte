<main>
	<div class="flex min-h-screen flex-col md:flex-row">
		<div class="w-full bg-white p-6 md:w-3/4">
			<slot />
		</div>

		<div class="mx-4 mt-20 h-full rounded-xl bg-gray-800 p-6 text-white md:w-1/4">
			<h2 class="mb-4 text-2xl font-semibold">Autor projektu</h2>
			<ul>
				<li class="mb-2">
					<strong>Imię i Nazwisko:</strong> Marcin Czop
				</li>
				<li class="mb-2">
					<strong>Grupa dziekańska: </strong> EiT/E1
				</li>
				<li class="mb-2">
					<strong>Nr. albumu: </strong> 315419
				</li>
			</ul>
		</div>
	</div>
</main>
