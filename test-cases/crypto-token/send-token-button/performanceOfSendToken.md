---
id: #SENDTOKEN004
title: Sprawdź wydajność systemu podczas równoczesnego wysyłania tokenów przez wielu użytkowników
description: Testy wydajnościowe przycisku "Next" oraz procesu wysyłania tokenów, gdy wielu użytkowników jednocześnie wykonuje tę operację
test Scenario: Weryfikacja wydajności systemu pod dużym obciążeniem
Test Steps:
  - Uruchom skrypt symulujący wielu użytkowników wysyłających tokeny jednocześnie
  - Monitoruj wydajność systemu i czas odpowiedzi
  - Sprawdź, czy system poprawnie obsługuje równoczesne operacje
Prerequisites: Skrypt do symulacji wielu użytkowników oraz narzędzia do monitorowania wydajności są dostępne
Expected/Intended Results: System poprawnie obsługuje równoczesne operacje wysyłania tokenów bez znaczących opóźnień i błędów
---

## Przypadek: 6a: Sprawdź wydajność przy równoczesnym wysyłaniu tokenów przez 100 użytkowników

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna, skrypt symulujący 100 użytkowników jest gotowy

**Kroki testowe:**

- Uruchom skrypt symulujący 100 użytkowników wysyłających tokeny jednocześnie
- Monitoruj wydajność systemu, w tym czas odpowiedzi i obciążenie serwera
- Sprawdź, czy system poprawnie obsługuje wszystkie operacje bez błędów

**Oczekiwany rezultat:** System poprawnie obsługuje równoczesne operacje wysyłania tokenów bez znaczących opóźnień i błędów przy 100 użytkownikach

## Przypadek: 6b: Sprawdź wydajność przy równoczesnym wysyłaniu tokenów przez 500 użytkowników

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna, skrypt symulujący 500 użytkowników jest gotowy

**Kroki testowe:**

- Uruchom skrypt symulujący 500 użytkowników wysyłających tokeny jednocześnie
- Monitoruj wydajność systemu, w tym czas odpowiedzi i obciążenie serwera
- Sprawdź, czy system poprawnie obsługuje wszystkie operacje bez błędów

**Oczekiwany rezultat:** System poprawnie obsługuje równoczesne operacje wysyłania tokenów bez znaczących opóźnień i błędów przy 500 użytkownikach

## Przypadek: 6c: Sprawdź wydajność przy równoczesnym wysyłaniu tokenów przez 1000 użytkowników

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna, skrypt symulujący 1000 użytkowników jest gotowy

**Kroki testowe:**

- Uruchom skrypt symulujący 1000 użytkowników wysyłających tokeny jednocześnie
- Monitoruj wydajność systemu, w tym czas odpowiedzi i obciążenie serwera
- Sprawdź, czy system poprawnie obsługuje wszystkie operacje bez błędów

**Oczekiwany rezultat:** System poprawnie obsługuje równoczesne operacje wysyłania tokenów bez znaczących opóźnień i błędów przy 1000 użytkownikach

## Przypadek: 6d: Sprawdź wydajność przy równoczesnym wysyłaniu tokenów przez 5000 użytkowników

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna, skrypt symulujący 5000 użytkowników jest gotowy

**Kroki testowe:**

- Uruchom skrypt symulujący 5000 użytkowników wysyłających tokeny jednocześnie
- Monitoruj wydajność systemu, w tym czas odpowiedzi i obciążenie serwera
- Sprawdź, czy system poprawnie obsługuje wszystkie operacje bez błędów

**Oczekiwany rezultat:** System poprawnie obsługuje równoczesne operacje wysyłania tokenów bez znaczących opóźnień i błędów przy 5000 użytkownikach

## Przypadek: 6e: Sprawdź stabilność systemu przy długotrwałym obciążeniu

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna, skrypt symulujący stałe obciążenie jest gotowy

**Kroki testowe:**

- Uruchom skrypt symulujący stałe obciążenie przez dłuższy czas (np. kilka godzin)
- Monitoruj wydajność systemu, w tym czas odpowiedzi i obciążenie serwera
- Sprawdź, czy system zachowuje stabilność i nie występują błędy

**Oczekiwany rezultat:** System zachowuje stabilność i poprawnie obsługuje operacje wysyłania tokenów przez dłuższy czas pod stałym obciążeniem
