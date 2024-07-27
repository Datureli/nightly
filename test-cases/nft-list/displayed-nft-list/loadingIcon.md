---
id: #NFTLOADING001
title: Sprawdź czas ładowania listy NFT
description: Testy czasu ładowania listy NFT oraz poprawności wyświetlania animacji ładowania
test Scenario: Weryfikacja czasu ładowania oraz poprawności wyświetlania animacji ładowania
Test Steps:
  - Mierzenie czasu ładowania listy NFT
  - Sprawdzenie, czy ikonka ładowania wyświetla się poprawnie
  - Testowanie na różnych przeglądarkach i urządzeniach
Prerequisites: Strona z listą NFT i animacją ładowania jest dostępna
Expected/Intended Results: Lista NFT ładuje się w akceptowalnym czasie, ikonka ładowania wyświetla się poprawnie, a testy działają na różnych przeglądarkach i urządzeniach
---

## Przypadek: 1a: Sprawdź czas ładowania listy NFT

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Zmierz czas od momentu otwarcia strony do momentu pełnego załadowania listy NFT
- Powtórz pomiar kilkukrotnie i oblicz średni czas ładowania

**Oczekiwany rezultat:** Lista NFT ładuje się w akceptowalnym czasie (np. poniżej 5 sekund)

---

## Przypadek: 1b: Sprawdź poprawność wyświetlania ikonki ładowania

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Sprawdź, czy ikonka ładowania pojawia się od razu po otwarciu strony
- Sprawdź, czy ikonka ładowania znika po pełnym załadowaniu listy NFT
- Powtórz test kilkukrotnie

**Oczekiwany rezultat:** Ikonka ładowania pojawia się natychmiast i znika po pełnym załadowaniu listy NFT

---

## Przypadek: 1c: Sprawdź wyświetlanie ikonki ładowania na różnych przeglądarkach

**Warunek wstępny:** Strona z listą NFT i animacją ładowania jest dostępna

**Kroki testowe:**

- Otwórz stronę z listą NFT w przeglądarce Chrome
- Sprawdź, czy ikonka ładowania pojawia się i znika poprawnie
- Powtórz test w przeglądarkach Firefox, Safari i Edge

**Oczekiwany rezultat:** Ikonka ładowania wyświetla się i znika poprawnie we wszystkich testowanych przeglądarkach

---

## Przypadek: 1d: Sprawdź wyświetlanie ikonki ładowania na różnych urządzeniach

**Warunek wstępny:** Strona z listą NFT i animacją ładowania jest dostępna

**Kroki testowe:**

- Otwórz stronę z listą NFT na komputerze
- Sprawdź, czy ikonka ładowania pojawia się i znika poprawnie
- Powtórz test na tablecie i telefonie

**Oczekiwany rezultat:** Ikonka ładowania wyświetla się i znika poprawnie na wszystkich testowanych urządzeniach

---

## Przypadek: 1e: Sprawdź stabilność wyświetlania ikonki ładowania przy słabym połączeniu internetowym

**Warunek wstępny:** Strona z listą NFT i animacją ładowania jest dostępna

**Kroki testowe:**

- Otwórz stronę z listą NFT przy słabym połączeniu internetowym (np. symulując 3G)
- Sprawdź, czy ikonka ładowania pojawia się i znika poprawnie
- Zmierz czas ładowania listy NFT

**Oczekiwany rezultat:** Ikonka ładowania wyświetla się i znika poprawnie, czas ładowania listy NFT jest dłuższy, ale system działa stabilnie

---

## Przypadek: 1g: Sprawdź wyświetlanie ikonki ładowania po odświeżeniu strony

**Warunek wstępny:** Strona z listą NFT i animacją ładowania jest dostępna

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Odśwież stronę
- Sprawdź, czy ikonka ładowania pojawia się i znika poprawnie

**Oczekiwany rezultat:** Ikonka ładowania wyświetla się i znika poprawnie po odświeżeniu strony
