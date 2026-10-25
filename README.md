# Dziennik Brzuszka

Prosta aplikacja na telefon do zapisywania, co jadło dziecko, jak się czuło i kiedy bolał je brzuch.

**Strona:** https://struzikmarcin-coder.github.io/dziennikbrzuszka/

## Co potrafi

- **Dzień:** pięć posiłków (śniadanie, II śniadanie, obiad, przekąski, kolacja). Każdy posiłek i każde danie usuniesz osobno, a przycisk „Nie był w przedszkolu” usuwa cały dzień z importu.
- **Import:** wgraj PDF z jadłospisem przedszkola. Przed zapisem odznaczysz posiłki, których dziecko nie jadło. Alergeny (A 1, 3, 7, 9…) są odczytywane.
- **Suplementy:** witamina D, DHA, probiotyk, żelazo i inne, także własne.
- **Samopoczucie i zdarzenia:** ocena 1–5 i zdarzenia typu afera w przedszkolu, kłótnia, zmęczenie.
- **Ból brzucha:** godzina, natężenie, czas trwania, miejsce, objawy.
- **Wnioski:** orientacyjna ocena diety (bez gramatur), co może brakować, oraz co częściej poprzedza ból: produkty, grupy, alergeny, emocje i zdarzenia.

## Dane

Na GitHub Pages wpisy są zapisywane tylko w pamięci przeglądarki na danym telefonie. Dodaj stronę do ekranu głównego (Safari: Udostępnij → Do ekranu początkowego; Chrome: menu → Dodaj do ekranu głównego) i co jakiś czas pobieraj kopię w zakładce Wnioski.

Wyniki to wskazówki do rozmowy z pediatrą, a nie diagnoza.

## Technicznie

Jeden plik `index.html` bez budowania. PDF czyta biblioteka pdf.js ładowana z cdnjs przy pierwszym imporcie.
