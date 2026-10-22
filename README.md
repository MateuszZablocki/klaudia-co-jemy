# Klaudia, co jemy? 🐾
Zabawny wybór kolacji dla Klaudii z maltańczykiem w roli doradcy. Polska, responsywna strona bez frameworka i bez procesu budowania.

## Funkcje
- 18 propozycji jedzenia i filtry kuchni.
- Wybór ręczny albo losowanie w aktualnym filtrze.
- Animowany, autorski maltańczyk SVG i wirtualne smaczki.
- Potwierdzenie kolacji z konfetti; zapamiętanie decyzji na dany dzień w przeglądarce.
- Obsługa klawiatury, natywne okno dialogowe, respektowanie ograniczenia animacji.

## Uruchomienie
Z katalogu projektu: `python3 -m http.server 4173 --directory dist`, następnie otwórz http://localhost:4173.

## Wdrożenie
Cała gotowa strona znajduje się w `dist/`. Nie wymaga instalowania zależności.
- **Netlify:** konfiguracja w `netlify.toml`; wystarczy podłączyć repozytorium.
- **Cloudflare Pages:** framework None, komenda budowania pusta, katalog wyjściowy `dist`.
- **Vercel:** framework Other, katalog wyjściowy `dist`, bez komendy budowania.
- **GitHub Pages:** automatyczne wdrożenie po każdym pushu do `main` przez `.github/workflows/pages.yml`. Hosting jest skonfigurowany: https://mateuszzablocki.github.io/klaudia-co-jemy/.

Fonty pobierane są z Google Fonts; w trybie offline używany jest font systemowy. Dane decyzji pozostają lokalnie w przeglądarce. Strona niczego nie zamawia ani nie wysyła wyboru do drugiej osoby.
