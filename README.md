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

Lokalny plik `Dane_studentci.xlsx` jest celowo wykluczony z Git. Zanim dane
studentów trafią do GitHuba, potwierdźcie, że są zanonimizowane i możecie je
udostępniać. Jeśli nie, uzgodnijcie bezpieczny sposób przekazania ich w zespole.

Docelowo trzymajcie plik źródłowy w `data/raw/`, a pliki po przetworzeniu
w `data/processed/`. Nie nadpisujcie danych źródłowych.

## Uruchomienie

Wymagany jest Python 3.10 lub nowszy. W PowerShell, w katalogu repozytorium:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

W VS Code wybierzcie interpreter z `.venv` i otwórzcie notatnik Jupyter
z katalogu `notebooks/`.

## Plan analizy

Końcowy notatnik powinien obejmować:

- wprowadzenie do danych i pytania badawcze,
- diagnostykę, czyszczenie i porządkowanie danych,
- 4–5 wizualizacji z krótką interpretacją,
- 2–3 analizy opisowe z interpretacją,
- wnioski i ograniczenia analizy.

Są to sekcje zgodne z wymaganiami projektu końcowego kursu AWDP.
