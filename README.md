### Opis ogólny
Przy każdym przypadku testowym należy wziąć pod uwagę następujące aspekty:

1. **Testowanie na różnych urządzeniach**: Upewnij się, że testujesz funkcjonalność na różnych typach urządzeń, takich jak komputery stacjonarne, laptopy, tablety i telefony. Sprawdź, czy wyniki są spójne na każdym z tych urządzeń.

2. **Testowanie na różnych systemach operacyjnych**: Testuj funkcjonalność na różnych systemach operacyjnych, takich jak Windows, macOS, Linux, Android i iOS, aby zapewnić pełną zgodność i działanie we wszystkich środowiskach.

3. **Responsywność**: Upewnij się, że aplikacja jest responsywna i dobrze się prezentuje na różnych rozmiarach ekranów. Sprawdź, czy interfejs użytkownika dostosowuje się do różnych rozdzielczości i orientacji ekranu.

4. **Testowanie na różnych przeglądarkach**: Testuj funkcjonalność na popularnych przeglądarkach, takich jak Google Chrome, Mozilla Firefox, Safari, Microsoft Edge, Opera, aby upewnić się, że wszystkie działają poprawnie i wyświetlają treści zgodnie z oczekiwaniami.

5. **Testowanie w różnych warunkach sieciowych**: Upewnij się, że aplikacja działa poprawnie w różnych warunkach sieciowych, takich jak szybkie i wolne połączenia internetowe, aby sprawdzić, czy nie występują problemy z ładowaniem lub wydajnością.

6. **Bezpieczeństwo aplikacji (SQL Injection)**: Testuj aplikację pod kątem podatności na ataki typu SQL Injection. Użyj różnych typów danych wejściowych, takich jak specjalne znaki (np. `' OR '1'='1`), aby upewnić się, że aplikacja jest odporna na takie ataki. Sprawdź, czy wprowadzenie złośliwego kodu nie wpływa na działanie bazy danych i czy odpowiedzi aplikacji są odpowiednio zabezpieczone.

### Kroki testowe:
- Otwórz stronę z listą NFT
- Wprowadź popularne słowo kluczowe (np. `BEER`) w pasek wyszukiwania
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Sprawdź, czy wyniki wyszukiwania zawierają NFT związane z wprowadzonym słowem kluczowym

### Oczekiwany rezultat:
Pasek wyszukiwania zwraca wyniki odpowiadające wprowadzonej frazie
