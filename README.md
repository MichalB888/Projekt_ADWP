# Analiza danych – studenci

Zespołowy projekt eksploracyjnej analizy danych przygotowywany w ramach kursu
Analiza danych w Pythonie. Analiza będzie oparta na zbiorze danych dotyczącym
studentów.

## Współpraca

1. Właściciel repozytorium dodaje koleżankę w GitHub: **Settings → Collaborators**.
   Nie udostępniajcie sobie haseł ani tokenów.
2. Każda osoba pobiera repozytorium i tworzy własną gałąź do pracy:

   ```powershell
   git clone https://github.com/MichalB888/Projekt_ADWP.git
   cd Projekt_ADWP
   git switch -c feat/opis-zmiany
   ```

3. Róbcie małe, opisowe commity. Po zakończeniu pracy wypchnijcie gałąź i otwórzcie
   Pull Request do `main`; druga osoba powinna go przejrzeć przed scaleniem.
4. Nie commitujcie haseł, tokenów ani danych, których nie wolno udostępniać.

## Dane

Zbiór leży w `data/raw/`. Na dysku plik nazywa się `Dane_studentci.xlsx`
(literówka w nazwie; notatnik przyjmuje też `Dane_studenci.xlsx`).
W notatniku opiszcie źródło danych, zakres i ograniczenia zbioru.

Trzymajcie pliki po przetworzeniu w `data/processed/` i nie nadpisujcie danych
źródłowych.

## Uruchomienie

Wymagany jest Python 3.10 lub nowszy. W PowerShell, w katalogu repozytorium:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

W VS Code wybierzcie interpreter z `.venv` i otwórzcie
`notebooks/analiza_studentow.ipynb`. Cała analiza jest w tym jednym notatniku,
z opisami i wynikami. Nie dodawajcie obok osobnych mini-skryptów.

## Plan analizy

Końcowy notatnik powinien obejmować:

- wprowadzenie do danych i pytania badawcze,
- diagnostykę, czyszczenie i porządkowanie danych,
- 4–5 wizualizacji z krótką interpretacją,
- 2–3 analizy opisowe z interpretacją,
- wnioski i ograniczenia analizy.

Są to sekcje zgodne z wymaganiami projektu końcowego kursu AWDP.
