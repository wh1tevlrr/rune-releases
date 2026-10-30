# Rune dla DaVinci Resolve

Wyszukiwarka i skróty do własnych presetów w DaVinci Resolve: adjustment clipów, Text+, solidów i kompozycji Fusion. Wstawiasz je jednym skrótem, a do tego zmieniasz zaznaczone klipy z klawiatury i tworzysz markery z listy poprawek.

## Instalacja

**[Pobierz RuneSetup.exe](https://github.com/wh1tevlrr/rune-releases/releases/latest/download/RuneSetup.exe)** (najnowsza wersja)

### Wymagania
- Windows 10 lub 11
- DaVinci Resolve **Studio** (testowane na wersji 21.0.4)

Python ani uprawnienia administratora nie są potrzebne.

### Krok po kroku

1. **Włącz skrypty w Resolve.** Wejdź w **Preferences → System → General** i ustaw **External scripting using** na **Local**. Bez tego Rune nie połączy się z Resolve.
2. **Uruchom `RuneSetup.exe`** i kliknij **Zainstaluj**. Plik nie ma podpisu cyfrowego, więc Windows może pokazać ostrzeżenie. Wybierz wtedy **Więcej informacji → Uruchom mimo to**.
3. **Zrestartuj Resolve.** Polecenia Rune pojawią się w **Workspace → Scripts → Edit → Rune**. Rune działa w tle jako pomarańczowa ikona **ᚱ** w zasobniku systemowym; jeśli jej nie widzisz, sprawdź ukryte ikony przy zegarze.
4. **Ustaw skrót wyszukiwarki.** Kliknij ikonę **ᚱ** prawym przyciskiem, wybierz **Skróty…** i naciśnij wybraną kombinację, np. `Shift+Space`.
5. **Zarejestruj szablon adjustment clipa** (tylko raz, potem działa w każdym projekcie):
   1. Przeciągnij **Effects → Toolbox → Effects → Adjustment Clip** na oś czasu.
   2. Przeciągnij ten klip z osi do **Media Pool** i zaznacz go tam.
   3. Wybierz **Workspace → Scripts → Edit → Rune → Rune - Zarejestruj szablon adjustment**.

Gotowe. Otwórz wyszukiwarkę skrótem i wpisz `adj`, żeby wstawić adjustment clip nad zaznaczonym klipem.

## Pierwszy preset

1. Przygotuj na osi klip z efektami, np. adjustment clip z animacją w Fusion, i zaznacz go.
2. Otwórz wyszukiwarkę, wpisz `zapisz` i zatwierdź.
3. Nadaj nazwę i kliknij **Zapisz**.

Od teraz znajdziesz ten preset w wyszukiwarce w każdym projekcie. Wpisz `>`, żeby zobaczyć wszystkie polecenia.

## Aktualizacje

Rune samo sprawdza nowe wersje i pokazuje dymek, gdy jakaś się pojawi. Instalujesz ją, wpisując `aktualizuj` w wyszukiwarce albo z menu ikony **ᚱ**. Rune zamknie się na kilka sekund i uruchomi ponownie, a presety i ustawienia zostaną.

## Odinstalowanie

Wejdź w **Ustawienia Windows → Aplikacje → Rune** albo uruchom `RuneSetup.exe` i wybierz **Odinstaluj**. Presety i ustawienia zostają w `%APPDATA%\RuneResolve`. Jeśli ich nie potrzebujesz, usuń ten folder ręcznie.

## Gdy coś nie działa

| Problem | Co zrobić |
|---|---|
| Rune nie łączy się z Resolve | Sprawdź, czy Resolve jest uruchomione i czy **External scripting using** to **Local** (krok 1). |
| W menu Resolve nie ma poleceń Rune | Zrestartuj Resolve po instalacji. |
| Komunikat o braku szablonu | Zarejestruj szablon adjustment clipa (krok 5). |
| Skrót nie działa | Inny program mógł go zająć. Wybierz inny w **Skróty…**. |
| Nic z tego nie pomaga | Log jest w menu ikony **ᚱ** → **Otwórz log**. |
