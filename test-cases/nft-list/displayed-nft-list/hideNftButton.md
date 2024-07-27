---
id: #NFTTOGGLE001
title: Sprawdź ukrywanie konkretnego NFT
description: Testy funkcjonalności ukrywania konkretnego NFT przy użyciu ikonki
test Scenario: Weryfikacja poprawności działania ikonki ukrywania NFT
Test Steps:
  - Sprawdzenie poprawności działania ikonki ukrywania
  - Testowanie na różnych przeglądarkach i urządzeniach
Prerequisites: Strona z listą NFT zawierającą ikonkę ukrywania jest dostępna
Expected/Intended Results: Ikonka ukrywania NFT działa poprawnie, ukrywa wybrane NFT i wyświetla odpowiednie komunikaty
---

## Przypadek: 1a: Sprawdź poprawność działania ikonki ukrywania NFT

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wybierz dowolne NFT z listy
- Kliknij ikonkę ukrywania przy wybranym NFT
- Sprawdź, czy wybrane NFT zostało ukryte
- Sprawdź, czy ikonka zmieniła stan (np. z "ukryj" na "odkryj")

**Oczekiwany rezultat:** Wybrane NFT jest ukryte, a ikonka zmienia stan

## Przypadek: 1b: Sprawdź ponowne odkrywanie ukrytego NFT

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Ukryj dowolne NFT używając ikonki ukrywania
- Kliknij ponownie ikonkę odkrywania przy ukrytym NFT
- Sprawdź, czy wybrane NFT zostało ponownie odkryte
- Sprawdź, czy ikonka zmieniła stan (np. z "odkryj" na "ukryj")

**Oczekiwany rezultat:** Ukryte NFT jest ponownie odkryte, a ikonka zmienia stan

## Przypadek: 1c: Sprawdź ukrywanie i odkrywanie NFT na różnych przeglądarkach

**Warunek wstępny:** Strona z listą NFT i ikonką ukrywania jest dostępna

**Kroki testowe:**

- Otwórz stronę z listą NFT w przeglądarce Chrome
- Ukryj dowolne NFT używając ikonki ukrywania
- Sprawdź, czy wybrane NFT zostało ukryte
- Odkryj ukryte NFT używając ikonki odkrywania
- Sprawdź, czy wybrane NFT zostało odkryte
- Powtórz test w przeglądarkach Firefox, Safari i Edge

**Oczekiwany rezultat:** Funkcjonalność ukrywania i odkrywania NFT działa poprawnie we wszystkich testowanych przeglądarkach

## Przypadek: 1d: Sprawdź ukrywanie i odkrywanie NFT na różnych urządzeniach

**Kroki testowe:**

- Otwórz stronę z listą NFT na komputerze
- Ukryj dowolne NFT używając ikonki ukrywania
- Sprawdź, czy wybrane NFT zostało ukryte
- Odkryj ukryte NFT używając ikonki odkrywania
- Sprawdź, czy wybrane NFT zostało odkryte
- Powtórz test na tablecie i telefonie

**Oczekiwany rezultat:** Funkcjonalność ukrywania i odkrywania NFT działa poprawnie na wszystkich testowanych urządzeniach

## Przypadek: 1e: Sprawdź stabilność ukrywania NFT przy słabym połączeniu internetowym

**Warunek wstępny:** Strona z listą NFT i ikonką ukrywania jest dostępna

**Kroki testowe:**

- Otwórz stronę z listą NFT przy słabym połączeniu internetowym (np. symulując 3G)
- Ukryj dowolne NFT używając ikonki ukrywania
- Sprawdź, czy wybrane NFT zostało ukryte
- Odkryj ukryte NFT używając ikonki odkrywania
- Sprawdź, czy wybrane NFT zostało odkryte

**Oczekiwany rezultat:** Funkcjonalność ukrywania i odkrywania NFT działa poprawnie, nawet przy słabym połączeniu internetowym

## Przypadek: 1f: Sprawdź, czy ikonka ukrywania działa poprawnie przy dużej liczbie NFT

**Warunek wstępny:** Strona z listą NFT zawierającą dużą liczbę NFT jest dostępna

**Kroki testowe:**

- Otwórz stronę z listą zawierającą dużą liczbę NFT (np. 1000 NFT)
- Ukryj dowolne NFT używając ikonki ukrywania
- Sprawdź, czy wybrane NFT zostało ukryte
- Odkryj ukryte NFT używając ikonki odkrywania
- Sprawdź, czy wybrane NFT zostało odkryte

**Oczekiwany rezultat:** Funkcjonalność ukrywania i odkrywania NFT działa poprawnie, nawet przy dużej liczbie NFT
