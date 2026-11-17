# twoj-kosmetolog

## Edycja aktualności i cennika

Treść komunikatu w polu `aktualnosciTekst` oraz ceny znajdują się w pliku [dane.js](./dane.js). Komunikat wpisuj między grawisami (`` ` ``); klawisz Enter tworzy nową linię. Grawis, ukośnik wsteczny oraz ciąg `${` w treści poprzedź ukośnikiem wstecznym. Nazwy i ceny zmieniaj w cudzysłowach, zachowując przecinki i nawiasy. Nie zmieniaj identyfikatorów kategorii ani oznaczeń grup laserowych. Warianty zabiegów znajdują się w tablicach `warianty`.

Lista galerii znajduje się w tablicy `certyfikaty` w [dane.js](./dane.js). Każdy wpis wymaga ścieżki `plik` do zdjęcia JPG, PNG lub WebP w folderze `certyfikaty/` oraz podpisu `tytul`. Opcjonalne pola `miniatura`, `tytulPodgladu` i `rodzaj` pozwalają wybrać mniejszy podgląd, inny tytuł powiększenia i rodzaj dokumentu. Jeśli nie podano miniatury, używany jest plik główny. Pusta tablica wyświetla informację o braku certyfikatów. Nowe zdjęcia umieszczaj w `certyfikaty/galeria/` i publikuj je razem ze stroną; pozostałe pliki w folderze `certyfikaty/` są domyślnie pomijane przez Git.

Bez JavaScriptu lub w razie błędu pliku danych strona wyświetla awaryjną wersję zapisaną w `index.html`; nie aktualizuje się ona automatycznie po edycji `dane.js`.