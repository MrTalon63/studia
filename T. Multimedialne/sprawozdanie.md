# 1. Wymagania

## 1.1. Techniczne

-   Zgodność z zasadami WCAG 2.1
-   Obsługa urządzeń mobilnych
-   Obsługa wszystkich powrzechnie używanych przez użytkowników przeglądarek (Chromium, Firefox)
-   Wykorzystanie dysku na poziomie 90-95%
-   Udostępenienie 2 kanałów RSS/Atom, dla odopowiednio materiałów audio i wideo

## 1.2. Multimedialne

-   Galeria zawierająca 12 zdjęć cyfrowych, z obsługą miniatur oraz pełnego rozmiaru.
-   3 filmy wideo, 5 minut każdy, z obsługą odtwarzania wideo w przeglądarce.
-   3 pliki audio, 5 minut każdy, z obsługą odtwarzania dźwięku w przeglądarce.
-   Materiały multimedialne mają zostać poddane obróbce, tak aby spełniały wymagania techniczne.

# 2. Realizacja

## 2.1. Techniczna

### 2.1.1. Budowa strony

-   Do budowy strony wykorzystano framework SvelteKit w wersji 5, razem z TailwindCSS w wersji 2.
-   Strona została podzielona na 3 główne sekcje: `header`, `Page`, `footer`, które rozdzielone są w poszczególne komponenty.
-   Projekt został wyeksportowany do statycznych plików HTML, CSS oraz JS za pomocą komendy `pnpm run build`
-   Technologie te zostały wybrane ze względu na ilość miejsca jakie zajmują na dysku oraz moją znajomość tych technologii.

## 2.2. Multimedialna

### 2.2.1. Galeria

-   Komponent galerii został własnoręcznie napisany i otwiera modal który pokazuje pełną wersję zdjęcia oraz opis.
-   Zdjęcia zostały poddane obróbce w programie Darktable.
-   Zdjęcia zostały wykonane aparatem Canon EOS R50 z obiektywami Canon RF 18-55mm f/2.8 oraz Tamron 70-200mm f/2.8.
-   Zdjęcia zostały wykonane w formacie RAW, a następnie wyeksportowane do formatu WebP w jakości 90% dla pełnych wersji i 75% dla wersji miniatur, które zostały zmniejszone do 20% oryginału.

### 2.2.2 Audio

-   Wykorzystano ścieżkę audio z materiałów wideo
-   Ścieżki audio skompresowano do formatu Opus programem Audacity używając współczynnik jakości na poziomie 4, 1 kanał (mono) oraz prędkość próbkowania na poziomie 48kHz
-   Pliki audio zostały również poddane obróbce w programie Audacity, wycięto fragmenty niepotrzebne oraz zredukowano szumy

### 2.2.3 Wideo

-   Materiały zostały nagrane aparatem Canon R50 z obiektywem Canon RF 18-55mm f/2.8 oraz mikrofonem kierunkowym o charakterystyce superkardioidalnej, w formacie 1080p 50kl/s
-   Materiały zostały zmontowane w programie Sony Vegas Pro 19 i wyekspotowane w formacie H.264 w jakości 90% oraz prędkości 50Mb/s
-   Następnie zostały one skompresowane w programie Handbrake do formatu WebM, przy użyciu enkodowania AV1 ze współczynnkiem jakości na poziomie 30 z VBR. Ilość klatek została zmniejszona do 25kl/s, a audio skompresowane do 64kb/s w formacie Opus z jednym kanałem (mono).
-   Format enkodowania AV1 został wybrany z powodu jego lepszej kompresji w porównaniu do H.264 czy VP9. W porównaniu do H.265 jest on jest o wiele szerzej wspierany przez przeglądarki internetowe, nie wspominając o kwestiach licencyjnych.

# 3. Inwentaryzacja

Przy zakończeniu projektu stan dysku wynosi ok. 109MB, co stanowi niemalże 91% zajętości dysku. Gdzie poszczególne elementy zajmują:

-   Zdjęcia: 8.2MB pełne, 440kB miniatury
-   Audio: 10.3MB
-   Wideo: 89.5MB

# 4. Wnioski

Projekt spełnia wszystkie wymagania techniczne oraz multimedialne. Wszystkie materiały zostały poddane obróbce, a strona została zbudowana zgodnie z zasadami WCAG 2.1. Projekt został zakończony zgodnie z harmonogramem oraz z wykorzystaniem dysku w przedziale 90-95%.
Projekt jako strona statyczna o ile łatwy w utrzymaniu, wymaga większej ilości pracy przy dodawaniu nowych materiałów multimedialnych. W przyszłości warto byłoby rozważyć wykorzystanie systemu zarządzania treścią, bądź dopisać serwerową stronę (backend) do dodawania nowych materiałów.

01.12.2024
Marcin Czop
