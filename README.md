# Dziennik Brzuszka

Prosta aplikacja na telefon do zapisywania, co jadło dziecko, jak się czuło i kiedy bolał je brzuch.

**Strona:** https://struzikmarcin-coder.github.io/dziennikbrzuszka/

## Co potrafi

- **Dzień:** pięć posiłków (śniadanie, II śniadanie, obiad, przekąski, kolacja). Każdy posiłek i każde danie usuniesz osobno, a przycisk „Nie był w przedszkolu” usuwa cały dzień z importu.
- **Import:** wgraj PDF z jadłospisem przedszkola. Przed zapisem odznaczysz posiłki, których dziecko nie jadło. Alergeny (A 1, 3, 7, 9…) są odczytywane.
- **Suplementy:** żelazo, Equazen, Hitaxa, witamina D 1000 i własne.
- **Samopoczucie i zdarzenia:** ocena 1–5 i zdarzenia typu afera w przedszkolu, kłótnia, zmęczenie.
- **Ból brzucha:** godzina, natężenie, czas trwania, miejsce, objawy.
- **Wnioski:** orientacyjna ocena diety (bez gramatur), co może brakować, oraz co częściej poprzedza ból: produkty, grupy, alergeny, emocje i zdarzenia.

## Dane i synchronizacja

Wpisy zapisują się w pamięci telefonu. Żeby widzieć je na kilku urządzeniach, włącz w zakładce Wnioski „Synchronizację między telefonami”: dane trafiają do pliku `dane/dziennik.json` w osobnym, **prywatnym** repo (np. `dziennikbrzuszka-dane`). Każde urządzenie łączy się tokenem fine-grained z uprawnieniem tylko „Contents: Read and write” do tego jednego repo.

To repo z aplikacją jest publiczne i nie zawiera żadnych danych.

Dodaj stronę do ekranu głównego (Safari: Udostępnij → Do ekranu początkowego; Chrome: menu → Dodaj do ekranu głównego). W zakładce Wnioski możesz też pobrać kopię JSON albo tabelę CSV.

Wyniki to wskazówki do rozmowy z pediatrą, a nie diagnoza.

## Technicznie

Jeden plik `index.html` bez budowania. PDF czyta biblioteka pdf.js ładowana z cdnjs przy pierwszym imporcie.
