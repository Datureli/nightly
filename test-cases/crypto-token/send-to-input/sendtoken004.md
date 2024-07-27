---
id: #SENDTOKEN003
title: Sprawdź, czy wielkość liter ma znaczenie w polu input "Send to"
description: Testy funkcji wysyłania tokenu z uwagi na wielkość liter w polu input "Send to"
test Scenario: Weryfikacja traktowania liter dużych i małych
Test Steps:
  - Wprowadź dane z literami dużymi
  - Wprowadź dane z literami małymi
  - Wprowadź dane z mieszanką liter dużych i małych
  - Sprawdź, czy dane są traktowane jako różne lub takie same
  - Porównaj wyniki w różnych scenariuszach

Prerequisites: Strona z polem input "Send to" jest dostępna
Expected/Intended Results: System prawidłowo obsługuje i rozróżnia wielkość liter w polu input
---

## Warunki wstępne
Strona z polem input "Send to" jest dostępna.

## Przypadek: 4a: Sprawdź akceptację liter dużych

**Kroki testowe:**

- Wprowadź string `HELLO` w pole input "Send to"
- Sprawdź, czy wartość została poprawnie zaakceptowana i przechowana
- Wprowadź string `hello` ponownie i porównaj wyniki

**Oczekiwany rezultat:**
Pole input akceptuje litery duże i przechowuje je poprawnie.

## Przypadek: 4b: Sprawdź akceptację liter małych

**Kroki testowe:**

- Wprowadź string `hello` w pole input "Send to"
- Sprawdź, czy wartość została poprawnie zaakceptowana i przechowana
- Wprowadź string `hello` ponownie i porównaj wyniki

**Oczekiwany rezultat:**
Pole input akceptuje litery małe i przechowuje je poprawnie.

## Przypadek: 4c: Sprawdź akceptację mieszanki liter dużych i małych

**Kroki testowe:**

- Wprowadź string `HeLLo` w pole input "Send to"
- Sprawdź, czy wartość została poprawnie zaakceptowana i przechowana
- Wprowadź string `HeLLo` ponownie i porównaj wyniki

**Oczekiwany rezultat:**
Pole input akceptuje mieszankę liter dużych i małych i przechowuje je poprawnie.

## Przypadek: 4d: Sprawdź, czy wielkość liter wpływa na funkcjonalność

**Kroki testowe:**

- Wprowadź różne kombinacje liter dużych i małych (np. `TEST`, `test`, `TeSt`)
- Wykonaj operację, która zależy od wartości (np. wysyłanie tokenu, porównanie danych)
- Sprawdź, czy operacja traktuje różne wielkości liter jako różne wartości lub jako te same

**Oczekiwany rezultat:**
System prawidłowo rozróżnia lub ignoruje różnice w wielkości liter w zależności od specyfikacji aplikacji.

## Przypadek: 4e: Sprawdź obsługę wielkości liter w walidacji

**Kroki testowe:**

- Wprowadź dane, które powinny powodować błąd walidacji, używając różnych wielkości liter (np. zbyt krótki lub zbyt długi string)
- Sprawdź, czy komunikaty o błędach są zgodne z oczekiwaniami, niezależnie od wielkości liter

**Oczekiwany rezultat:**
Komunikaty o błędach są prawidłowe, niezależnie od wielkości liter.
