# Plan pracy — chappie-bot

## Status audytu
AUDYT ZAKOŃCZONY — 2026-09-12.

## Stan faktyczny
Historyczny bot Python uruchamiany w Docker/Heroku. README zawiera dużą listę komend ze stanami `OK`, `ERROR`, `BUG`, `?` i wymaganiami API key. Dokumentacja wskazuje wiele funkcji multimedialnych, społecznościowych i administracyjnych.

## Ryzyka
- wiele funkcji ma niezweryfikowany lub jawnie błędny status;
- stare ścieżki wdrożeniowe i zależności;
- brak formalnego modelu uprawnień i testów kontraktowych widocznych w README;
- część komend może wykonywać operacje na danych użytkowników lub grup.

## Priorytet
ŚREDNI.

## Kolejność prac
1. Zmapować faktyczne moduły i entrypoint.
2. Usunąć nieaktualne komendy z dokumentacji albo oznaczyć je jako historyczne.
3. Wprowadzić konfigurację sekretów przez środowisko.
4. Zdefiniować permission model dla operacji grupowych.
5. Dodać testy jednostkowe i smoke test bota.
6. Zmodernizować runtime i deployment.
7. Spolonizować dokumentację.

## Kryterium zakończenia
Dokumentacja odpowiada rzeczywistemu kodowi, wszystkie aktywne komendy mają testy lub jasno zdefiniowany kontrakt, a operacje administracyjne są autoryzowane.
