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

### 2.1.1. CMS

-   Wykorzystano system zarządzania treścią Grav z szabloenm Quark.
-   Wdrożono pluginy:
    -   Admin Panel
    -   Form
    -   Problems
    -   Feed
    -   Email
    -   Error
    -   Flex Objects
    -   Login
    -   Markdown Notices
    -   Shortcode Core
    -   Shortcode Gallery++

## 2.2. Multimedialna

### 2.2.1. Galeria

-   Wykorzystano plugin Shortcode Gallery++ do obsługi galerii.
-   Zdjęcia zostały poddane obróbce w programie Adobe Lightroom.
-   Zdjęcia zostały wykonane aparatem Canon EOS R50 z obiektywami Canon RF 18-55mm f/2.8 oraz Tamron 70-200mm f/2.8.
-   Zdjęcia zostały wykonane w formacie RAW, a następnie wyeksportowane do formatu WebP.

### 2.2.2 Audio

-   Wykorzystano ścieżkę audio z materiałów wideo
-   Ścieżki audio skompresowano do formatu Opus programem Audacity do bitrateu 64kbps z 1 kanałem (mono) oraz prędkością próbowania na poziomie 48kHz

### 2.2.3 Wideo

-   Materiały zostały nagrane aparatem Canon R50 z obiektywem Canon RF 18-55mm f/2.8 oraz mikrofonem kierunkowym o charakterystyce superkardioidalnej, w formacie 1080p 25kl/s
-   Materiały zostały zmontowane w programie Sony Vegas Pro 18, a następnie skompresowane kodekiem AV1 do bitrateu 1Mbps programem Handbrake
