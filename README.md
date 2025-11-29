# AI HTML Generator - Zadanie Rekrutacyjne

![Project Status](https://img.shields.io/badge/Status-Completed-success)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o-green)

Projekt zrealizowany jako rozwiązanie zadania rekrutacyjnego dla firmy **Oxido**. Jest to narzędzie automatyzujące proces przetwarzania treści artykułów do formatu HTML przy użyciu sztucznej inteligencji.

## 💡 O projekcie

Celem zadania było stworzenie skryptu w języku Python, który łączy się z API OpenAI, aby przetworzyć surowy tekst artykułu na kod HTML. Aplikacja nie tylko formatuje tekst, ale również inteligentnie sugeruje miejsca na grafiki, tworząc dla nich odpowiednie tagi i opisy.

## 🚀 Funkcjonalności

Zgodnie z wymaganiami zadania, aplikacja realizuje następujące funkcje:
* **Integracja z GPT-4o:** Wykorzystuje model językowy do analizy i strukturyzacji tekstu.
* **Generowanie tagów HTML:** Tworzy kod ograniczony do zawartości sekcji `<body>` (bez `<html>` czy `<head>`).
* **Inteligentne obrazowanie:** Wstawia tagi `<img src="image_placeholder.jpg">` w miejscach, gdzie grafika wzbogaciłaby treść.
* **Generowanie opisów alt:** Tworzy precyzyjne prompty w atrybucie `alt`, które mogą posłużyć do wygenerowania grafik przez AI.
* **Podpisy pod zdjęciami:** Dodaje odpowiednie podpisy (`<figcaption>`) pod każdą grafiką.

## 🛠️ Wymagania

* Python 3.x
* Biblioteka `openai`
* Klucz API OpenAI

## 📦 Instalacja

1.  Sklonuj repozytorium:
    ```bash
    git clone https://github.com/AntekKozlowski/openai-html-generator.git
    cd openai-html-generator
    ```

2.  Zainstaluj wymagane zależności:
    ```bash
    pip install openai
    ```

## ⚙️ Konfiguracja

1.  Otwórz plik `htmlGenerator.py`.
2.  Wprowadź swój klucz API w odpowiednim miejscu:
    ```python
    openai.api_key = 'TWOJ_KLUCZ_API'
    ```

## ▶️ Uruchomienie (Instrukcja)

1.  Upewnij się, że w katalogu znajduje się plik **`artykulTekst.txt`** z treścią artykułu do przetworzenia.
2.  Uruchom program:
    ```bash
    python htmlGenerator.py
    ```
3.  Po wyświetleniu komunikatu *"Zakonczono sukcesem"*, sprawdź wynik w nowo utworzonym pliku **`artykul.html`**.
4.  (Opcjonalnie) Aby zobaczyć sformatowany podgląd, możesz wykorzystać załączony plik `szablon.html` lub `podglad.html`.

## 📂 Struktura plików

* `htmlGenerator.py` - Kod źródłowy aplikacji (Python).
* `artykulTekst.txt` - Plik wejściowy z artykułem.
* `artykul.html` - Wynik działania programu (wygenerowany kod HTML).
* `szablon.html` / `podglad.html` - Pliki pomocnicze do wizualizacji wyniku w przeglądarce.

---
*Autor: Antoni Kozłowski*
