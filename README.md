# Maze Tanks Mobile

Gra w czołgi na telefon i tablet, widok z góry, sterowanie dwoma joystickami. Jedź przez labirynt, strzelaj z rykoszetu i pokonaj boty.

**Zagraj online:** https://mjwawa.github.io/maze_tanks_mobile/

Na komputer z klawiaturą (także dla 2 graczy) jest osobna wersja: [Maze Tanks](https://mjwawa.github.io/maze_tanks_web/).

## Jak grać

- **Joystick jazdy** (domyślnie z lewej): pokaż palcem kierunek, czołg obróci się i pojedzie. Kierunek za czołgiem oznacza cofanie.
- **Joystick strzału** (domyślnie z prawej): przytrzymaj, żeby strzelać prosto. Przeciągnij, żeby wycelować: czołg obróci się i strzeli.
- Strony joysticków można zamienić w ustawieniach (np. dla leworęcznych).
- Przycisk **II** w prawym górnym rogu to pauza.
- Widok jest powiększony: widać 1/4 mapy, a kamera jedzie za Twoim czołgiem.
- Minimapa w lewym górnym rogu pokazuje całą planszę, Twój czołg (z kierunkiem jazdy), widocznych przeciwników i fragment widoczny na ekranie.
- Grasz sam przeciw 1–3 botom. Najlepiej trzymać urządzenie poziomo.

## Mapy i poziomy

- Trzy poziomy botów: łatwy, normalny, trudny
- Mapy (labirynt losuje się w każdej rundzie):
  - **Las** – kłody, świerki, dęby
  - **Pole** – kamienne murki, bele siana
  - **Miasto** – ceglane mury, beczki, pachołki, kosze, latarnie
  - **Noc w mieście** – miasto po zmroku, światło latarni i reflektorów czołgów
  - **Pustynia** – mury z gliny, kaktusy, głazy
  - **Zima** – zaspy, ośnieżone choinki, bałwany
  - **Baza wojskowa** – worki z piaskiem, beczki paliwa, skrzynie, opony
  - **Księżyc** – metalowe panele, skały, anteny, kratery

## Zasady specjalne map

Każda mapa ma swoją zasadę specjalną. Jej nazwa pojawia się na początku rundy, a opis – w ustawieniach pod wyborem mapy:

| Mapa | Zasada |
|---|---|
| Las | **Kryjówki w krzakach** – przez krzaki można przejechać i się w nich schować, pociski przez nie przelatują |
| Pole | **Wiatr** – znosi pociski; kierunek i siłę pokazuje strzałka u góry |
| Miasto | **Płonące samochody** – żar wraków parzy od razu po wjechaniu i zabiera 1 punkt pancerza co 0,6 s |
| Noc w mieście | **Ciemno** – widać tylko to, co jest w świetle; strzał zdradza pozycję |
| Pustynia | **Grząski piasek** – po długiej jeździe czołg grzęźnie; postój lub cofanie uwalnia |
| Zima | **Ślisko** – czołgi ślizgają się, na zamarzniętych kałużach jeszcze bardziej |
| Baza wojskowa | **Skrzynie z amunicją** – wybuchają po najechaniu lub trafieniu; worki z piaskiem pochłaniają pociski |
| Księżyc | **Nieważkość** – czołgi dryfują; pociski lecą wolniej, ale odbijają się 2 razy więcej |

## Zasady

- Pociski odbijają się od ścian i drzew. Uważaj, własny rykoszet też zabiera życie.
- Rundę wygrywa ostatni czołg na polu bitwy.
- Kto pierwszy wygra 5 rund (albo 3 lub 7, do wyboru w menu), zdobywa **złoty medal**. Medale zbierają się w gablocie.

## Rodzaje czołgów

| | Lis (lekki) | Wilk (średni) | Niedźwiedź (ciężki) |
|---|---|---|---|
| Prędkość | szybki | średni | wolny |
| Pancerz | 3 | 5 | 8 |
| Siła rażenia | 1 | 2 | 3 |
| Tempo strzałów | bardzo szybkie | średnie | wolne |
| Pociski naraz | 6 | 4 | 2 |
| Odbicia pocisku | 3 | 3 | 2 |

## Zainstaluj jako aplikację

- **iPad / iPhone (Safari):** Udostępnij → *Dodaj do ekranu początkowego*
- **Android (Chrome):** przycisk *Zainstaluj jako aplikację* w menu gry albo ⋮ → *Zainstaluj aplikację*

Po pierwszym uruchomieniu gra działa offline, także w samolocie czy w samochodzie. Nowe wersje z GitHuba pobierają się same przy starcie, gdy jest internet.

## Technicznie

Cała gra to jeden plik `index.html` (HTML + JavaScript z wbudowanymi czcionkami, rysowanie na canvasie, dźwięki generowane przez Web Audio API). Nie potrzebuje serwera ani instalacji.

Pliki aplikacji: `manifest.webmanifest` (nazwa, ikony), `sw.js` (praca offline), ikony `icon-512.png`, `icon-maskable-512.png`, `favicon-*.png`, `favicon.svg`, `apple-touch-icon.png`.
