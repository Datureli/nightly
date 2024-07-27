---
id: #PAGINATION001
title: Sprawdź paginację w długich listach NFT
description: Testowanie paginacji lub ładowania "na żądanie" dla dużych list NFT, aby upewnić się, że aplikacja efektywnie zarządza dużą liczbą elementów i nie ma problemów z wydajnością.
test Scenario: Weryfikacja paginacji lub ładowania "na żądanie" dla dużych list NFT
Test Steps:
  - Otwórz stronę z długą listą NFT (np. zawierającą więcej niż 100 elementów)
  - Sprawdź, czy lista jest podzielona na strony lub ładowane są dodatkowe elementy w miarę przewijania (jeśli stosowane jest ładowanie "na żądanie")
  - Przejdź do różnych stron lub przewiń do końca listy, aby upewnić się, że wszystkie elementy są poprawnie ładowane
  - Zwróć uwagę na wydajność i czas ładowania, obserwując, czy aplikacja działa płynnie
  - Sprawdź, czy nie występują błędy, takie jak zamrożenie aplikacji, długie czasy oczekiwania, lub problemy z ładowaniem danych
Prerequisites: Strona z dużą listą NFT jest dostępna i zaimplementowana paginacja lub ładowanie "na żądanie"
Expected/Intended Results: Aplikacja poprawnie zarządza dużą liczbą elementów poprzez paginację lub ładowanie "na żądanie", wydajność jest akceptowalna, a błędy są minimalne
---

## Przypadek: 1a: Sprawdź paginację dla długiej listy NFT

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Sprawdź, czy lista jest podzielona na strony (np. 10 elementów na stronę)
- Kliknij przyciski nawigacyjne do różnych stron (np. "Następna", "Poprzednia", numery stron)
- Sprawdź, czy elementy są poprawnie ładowane na każdej stronie i nawigacja działa bez błędów

**Oczekiwany rezultat:** Lista NFT jest poprawnie paginowana, a nawigacja między stronami działa płynnie. Wydajność jest akceptowalna, a błędy są minimalne.

## Przypadek: 1b: Sprawdź ładowanie "na żądanie" w przypadku długiej listy NFT

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Przewiń listę do końca
- Sprawdź, czy nowe elementy są automatycznie ładowane w miarę przewijania
- Upewnij się, że ładowanie nowych elementów jest płynne i nie występują błędy

**Oczekiwany rezultat:** Nowe elementy są automatycznie ładowane w miarę przewijania listy. Proces ładowania jest płynny, a wydajność jest akceptowalna.

## Przypadek: 1c: Sprawdź wydajność aplikacji przy dużej liczbie elementów

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Sprawdź czas ładowania listy oraz responsywność aplikacji
- Zmieniaj strony lub przewijaj listę i obserwuj, czy aplikacja działa płynnie

**Oczekiwany rezultat:** Aplikacja działa płynnie i responsywnie, a czas ładowania i wydajność są w granicach akceptowalnych wartości.

## Przypadek: 1d: Sprawdź stabilność aplikacji przy dużej liczbie elementów

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Sprawdź, czy wszystkie elementy są poprawnie ładowane i wyświetlane
- Upewnij się, że nie występują błędy podczas ładowania danych (np. błędy 404, błędy serwera)

**Oczekiwany rezultat:** Wszystkie elementy są poprawnie ładowane bez błędów. Aplikacja działa stabilnie i nie ulega awarii podczas ładowania dużej liczby elementów.
