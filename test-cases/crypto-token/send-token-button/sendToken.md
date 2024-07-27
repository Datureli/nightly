---
id: #SENDTOKEN005
title: Sprawdź funkcjonalność przycisku "Next"
description: Testy przycisku "Next" przechodzącego do następnego etapu po wypełnieniu pól input "Send to" i "amount"
test Scenario: Weryfikacja działania przycisku "Next"
Test Steps:
  - Wypełnij pole "Send to"
  - Wypełnij pole "amount"
  - Kliknij przycisk "Next"
  - Sprawdź, czy użytkownik został przeniesiony do następnego etapu
Prerequisites: Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna
Expected/Intended Results: Po wypełnieniu pól i kliknięciu przycisku "Next" użytkownik zostaje przeniesiony do następnego etapu
---

## Przypadek: 5a: Sprawdź działanie przycisku "Next" przy poprawnym wypełnieniu pól

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. `recipient@example.com`)
- Wprowadź poprawne dane w pole "amount" (np. `100`)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"

## Przypadek: 5b: Sprawdź działanie przycisku "Next" przy niepełnym wypełnieniu pól

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. `recipient@example.com`)
- Pozostaw pole "amount" puste
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o konieczności wypełnienia wszystkich pól

## Przypadek: 5c: Sprawdź działanie przycisku "Next" przy wypełnieniu pól niepoprawnymi danymi

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź niepoprawne dane w pole "Send to" (np. `invalid-email`)
- Wprowadź poprawne dane w pole "amount" (np. `100`)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o błędnych danych

## Przypadek: 5d: Sprawdź działanie przycisku "Next" przy wypełnieniu pola "Send to" znakami specjalnymi

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź dane w pole "Send to" zawierające znaki specjalne (np. `recipient@ex@mple.com`)
- Wprowadź poprawne dane w pole "amount" (np. `100`)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o błędnych danych

## Przypadek: 5e: Sprawdź działanie przycisku "Next" przy wypełnieniu pola "amount" wartością ujemną

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. `recipient@example.com`)
- Wprowadź wartość ujemną w pole "amount" (np. `-100`)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o błędnych danych

## Przypadek: 5f: Sprawdź działanie przycisku "Next" przy wypełnieniu pola "amount" wartością zmiennoprzecinkową

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. `recipient@example.com`)
- Wprowadź wartość zmiennoprzecinkową w pole "amount" (np. `100.50`)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"

## Przypadek: 5g: Sprawdź działanie przycisku "Next" po usunięciu wprowadzonych danych

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. `recipient@example.com`)
- Wprowadź poprawne dane w pole "amount" (np. `100`)
- Usuń dane z pola "Send to" i "amount"
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o konieczności wypełnienia wszystkich pól

## Przypadek: 5h: Sprawdź działanie przycisku "Next" przy wypełnieniu pól z maksymalną ilością danych

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź dane w pole "Send to" z maksymalną ilością znaków (np. 255 znaków)
- Wprowadź dane w pole "amount" z maksymalną ilością cyfr (np. 9999999999)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"

## Przypadek: 5i: Sprawdź działanie przycisku "Next" przy wypełnieniu pól z minimalną ilością danych

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź dane w pole "Send to" z minimalną ilością znaków (np. `a@b.c`)
- Wprowadź dane w pole "amount" z minimalną ilością cyfr (np. `1`)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"

## Przypadek: 5j: Sprawdź działanie przycisku "Next" przy wypełnieniu pól z danymi mieszanymi

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź dane w pole "Send to" z mieszanymi znakami (np. `Recipient+Test@example.com`)
- Wprowadź dane w pole "amount" z mieszanymi znakami (np. `100.00`)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"

## Przypadek: 5k: Sprawdź zmiany stanu konta po wysłaniu kryptowalut

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna, a użytkownik jest zalogowany i ma aktywne konto z pewnym saldem

**Kroki testowe:**

1. Wprowadź dane w pole "Send to" (np. `recipient@example.com`)
2. Wprowadź dane w pole "amount" (np. `100`)
3. Kliknij przycisk "Next"
4. Potwierdź transakcję, jeśli to wymagane (np. klikając przycisk "Confirm")
5. Sprawdź, czy saldo konta użytkownika zostało zaktualizowane o kwotę podaną w polu "amount" (np. saldo powinno zmniejszyć się o 100)

**Oczekiwany rezultat:** Po wysłaniu kryptowalut saldo konta użytkownika zmienia się o wartość podaną w polu "amount". Na przykład, jeśli początkowe saldo wynosiło `500` i wysłano `100`, nowe saldo powinno wynosić `400`.

## Przypadek: 5l: Sprawdź, czy wysłane kryptowaluty trafiły do właściwego użytkownika

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna, a użytkownik jest zalogowany i ma aktywne konto z pewnym saldem. Odbiorca posiada również aktywne konto, do którego mogą być wysyłane kryptowaluty.

**Kroki testowe:**

1. Wprowadź dane w pole "Send to" (np. `recipient@example.com`)
2. Wprowadź dane w pole "amount" (np. `100`)
3. Kliknij przycisk "Next"
4. Potwierdź transakcję, jeśli to wymagane (np. klikając przycisk "Confirm")
5. Sprawdź saldo konta użytkownika, którego adres został podany w polu "Send to", aby upewnić się, że saldo zostało zwiększone o wartość podaną w polu "amount" (np. saldo powinno wzrosnąć o 100)

**Oczekiwany rezultat:** Saldo konta użytkownika, którego adres został podany w polu "Send to", wzrosło o wartość podaną w polu "amount". Na przykład, jeśli konto odbiorcy miało początkowo saldo `300` i wysłano mu `100`, nowe saldo powinno wynosić `400`.

## Przypadek: 5m: Sprawdź, czy wysłanie jednej kryptowaluty nie wpływa na saldo konta w innych kryptowalutach

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna. Użytkownik jest zalogowany i posiada konto z saldami w różnych kryptowalutach.

**Kroki testowe:**

1. **Sprawdź początkowe saldo** w różnych kryptowalutach na koncie użytkownika. Zanotuj salda dla wszystkich kryptowalut (np. Bitcoin, Ethereum, Litecoin).
2. Wprowadź dane w pole "Send to" (np. `recipient@example.com`)
3. Wprowadź dane w pole "amount" dla wybranego rodzaju kryptowalut (np. `100 BTC`)
4. Kliknij przycisk "Next"
5. Potwierdź transakcję, jeśli to wymagane (np. klikając przycisk "Confirm")
6. **Sprawdź saldo** konta użytkownika w kryptowalutach, które nie były użyte w transakcji (np. Ethereum i Litecoin). Upewnij się, że salda pozostały bez zmian.
7. **Sprawdź saldo** konta użytkownika w kryptowalucie, która została użyta w transakcji (np. Bitcoin) i upewnij się, że saldo zostało zaktualizowane o wartość wysłaną.

**Oczekiwany rezultat:** Wysyłając kryptowaluty jednego rodzaju (np. Bitcoin), saldo konta użytkownika w innych kryptowalutach (np. Ethereum, Litecoin) pozostaje bez zmian. Saldo konta w kryptowalucie, która została użyta w transakcji, powinno zostać zaktualizowane o wartość wysłaną.

## Przypadek: 1a: Brak ochrony przed podwójnym kliknięciem

**Opis:** Użytkownik może wielokrotnie kliknąć przycisk "Wyślij", co może prowadzić do podwójnych transakcji.

**Warunek wstępny:** Strona z formularzem wysyłania tokenów jest dostępna, a użytkownik jest zalogowany.

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. `recipient@example.com`)
- Wprowadź poprawną kwotę w pole "amount" (np. `100`)
- Kliknij przycisk "Wyślij"
- Natychmiast po kliknięciu przycisku, kliknij go ponownie wielokrotnie w krótkim okresie czasu (np. 5 razy w ciągu 1 sekundy)
- Sprawdź, czy aplikacja obsługuje wielokrotne kliknięcia bez generowania podwójnych transakcji
- Sprawdź, czy przycisk "Wyślij" zostaje dezaktywowany po pierwszym kliknięciu lub jeśli aplikacja wyświetla komunikat o błędzie

**Oczekiwany rezultat:** Przy pierwszym kliknięciu przycisk "Wyślij" zostaje dezaktywowany, lub aplikacja obsługuje wielokrotne kliknięcia w sposób zapobiegający podwójnym transakcjom.

## Przypadek: 1b: Problemy z dokładnością kwoty

**Opis:** Kwota wpisana w polu numerycznym może być zaokrąglana w sposób, który prowadzi do błędów w transakcjach.

**Warunek wstępny:** Strona z formularzem wysyłania tokenów jest dostępna, a użytkownik jest zalogowany.

**Kroki testowe:**

- Wprowadź różne formaty kwot w pole "amount" (np. `100`, `100.1`, `100.123456`)
- Kliknij przycisk "Wyślij"
- Sprawdź, jak aplikacja zaokrągla wprowadzone kwoty i jak są one wyświetlane w potwierdzeniu transakcji
- Weryfikuj, czy aplikacja wykonuje transakcje zgodnie z dokładnie wprowadzoną kwotą

**Oczekiwany rezultat:** Kwoty są poprawnie zaokrąglane i wyświetlane zgodnie z wprowadzeniem, a transakcje są realizowane zgodnie z dokładną kwotą podaną przez użytkownika.
