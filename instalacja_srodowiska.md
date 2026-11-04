# Przygotowanie środowiska do zajęć z informatyki: Python + VS Code

Ta instrukcja jest przeznaczona również dla osób, które **po raz pierwszy programują**. Przejdź przez kolejne kroki we własnym tempie. Nie musisz rozumieć wszystkich nowych pojęć od razu.

**Cel:** po zakończeniu instalacji potrafisz:

- otworzyć Visual Studio Code (VS Code),
- stworzyć, zapisać i uruchomić plik Pythona (`.py`),
- stworzyć, zapisać i uruchomić notatnik Jupyter (`.ipynb`),
- wybrać właściwego Pythona (interpreter) i **kernel** dla notatnika,
- uruchamiać kolejne komórki z zadaniami na zajęciach.

> **Nie musisz mieć konta Microsoft ani GitHub, aby korzystać z VS Code lokalnie.** Wszystkie potrzebne narzędzia są bezpłatne.

## 1. Co instalujemy?

| Narzędzie | Do czego służy? |
| --- | --- |
| **Python 3** | Wykonuje napisany przez nas kod. |
| **Visual Studio Code (VS Code)** | Program, w którym piszemy i uruchamiamy kod. |
| **Rozszerzenie Python** | Pozwala VS Code wygodnie pracować z Pythonem. |
| **Rozszerzenie Jupyter** | Pozwala otwierać i uruchamiać notatniki `.ipynb`. |

## 2. Zainstaluj Python 3

1. Otwórz [oficjalną stronę pobierania Pythona](https://www.python.org/downloads/).
2. Pobierz instalator dla swojego systemu (**Windows** lub **macOS**).
3. Uruchom instalator i przejdź przez kolejne kroki.

### Windows

Jeżeli instalator pokazuje pole **Add Python to PATH**, zaznacz je przed instalacją. W nowszych instalatorach ten ekran może wyglądać inaczej — to normalne.

**Sprawdź instalację:**

1. Otwórz menu Start, wpisz `cmd` i uruchom **Wiersz polecenia**.
2. Wpisz:

   ```powershell
   py -3 --version
   ```

Jeśli to polecenie nie działa, spróbuj:

   ```powershell
   python --version
   ```

### macOS

Otwórz pobrany plik `.pkg` i przejdź przez instalację.

**Sprawdź instalację:**

1. Otwórz aplikację **Terminal** (możesz wyszukać ją przez Spotlight).
2. Wpisz:

   ```bash
   python3 --version
   ```

**Oczekiwany wynik** na obu systemach wygląda podobnie do:

```text
Python 3.x.x
```

`x` oznacza numer wersji. Nie musi być identyczny u wszystkich.

> Jeśli terminal nie rozpoznaje polecenia, zamknij go, otwórz ponownie i spróbuj jeszcze raz. Jeśli problem nadal występuje, wróć do instalacji Pythona.

## 3. Zainstaluj Visual Studio Code

1. Przejdź na [stronę pobierania VS Code](https://code.visualstudio.com/download).
2. Pobierz instalator dla swojego systemu.
3. Zainstaluj program i go uruchom.

## 4. Zainstaluj rozszerzenia Python i Jupyter

1. W VS Code kliknij **Extensions** po lewej stronie (ikona z czterema kwadratami).
2. W wyszukiwarce wpisz `Python`.
3. Zainstaluj rozszerzenie **Python** autorstwa **Microsoft**.
4. Następnie wyszukaj `Jupyter`.
5. Zainstaluj rozszerzenie **Jupyter** autorstwa **Microsoft**.

Po instalacji najlepiej zamknąć i ponownie otworzyć VS Code.

## 5. Przygotuj folder na swoje pliki

1. Utwórz na komputerze folder o nazwie `informatyka`, np. w **Dokumentach**.
2. W VS Code wybierz **File → Open Folder** (Plik → Otwórz folder).
3. Wskaż folder `informatyka`.
4. Jeśli VS Code zapyta, czy ufasz plikom w folderze, możesz potwierdzić — to Twój własny folder.

Po lewej stronie, w panelu **Explorer**, powinna pojawić się nazwa folderu.

## 6. Pierwszy program: plik `.py`

### Utwórz plik

1. W panelu **Explorer** kliknij **New File** (kartka z plusem).
2. Wpisz nazwę `test.py` i naciśnij Enter.
3. Wklej do pliku:

   ```python
   a = 5
   b = 7
   print("Wynik dodawania:", a + b)
   ```

4. Zapisz plik: **Ctrl + S** (Windows) lub **Cmd + S** (macOS).

### Wybierz interpreter Pythona

**Interpreter** to program, który wykonuje kod z pliku `.py`.

1. Wciśnij **Ctrl + Shift + P** (Windows) lub **Cmd + Shift + P** (macOS).
2. Wpisz `Python: Select Interpreter` i wybierz tę komendę.
3. Z listy wybierz zainstalowanego **Pythona 3**.

### Uruchom program

Kliknij przycisk **▶ Run Python File** w prawym górnym rogu edytora. Na dole otworzy się **Terminal** z wynikiem:

```text
Wynik dodawania: 12
```

Jeśli widzisz te dwie linie, Twój pierwszy program działa.

## 7. Pierwszy notatnik: plik `.ipynb`

Notatnik Jupyter pozwala podzielić kod na mniejsze części, czyli **komórki** (*cells*). Każdą komórkę można uruchomić oddzielnie. Na zajęciach będziemy często korzystać właśnie z tego formatu.

### Utwórz notatnik

1. W panelu **Explorer** kliknij **New File**.
2. Nadaj plikowi nazwę `test_notebook.ipynb`.
3. Po otwarciu powinien pojawić się widok notatnika z komórkami.

Jeśli widok notatnika się nie otworzy, sprawdź, czy masz zainstalowane rozszerzenie **Jupyter**. Możesz też otworzyć paletę poleceń (**Ctrl/Cmd + Shift + P**), wyszukać `Create: New Jupyter Notebook`, a potem zapisać nowy notatnik jako `test_notebook.ipynb`.

### Wybierz kernel — ważny krok

**Kernel** to środowisko, które uruchamia kod w notatniku. Zwykle wystarczy wybrać zainstalowanego wcześniej Pythona 3.

1. W prawym górnym rogu notatnika kliknij **Select Kernel**.
2. Wybierz **Python 3** (jeśli jest widoczny).
3. Jeśli nie widzisz Pythona, wybierz **Select Another Kernel → Python Environments**, a następnie zainstalowanego **Pythona 3**.
4. Jeśli VS Code zaproponuje instalację pakietu **`ipykernel`**, zaakceptuj ją. Może to wymagać dostępu do Internetu.

> **Interpreter a kernel:** interpreter wybieramy do plików `.py`, a kernel do notatników `.ipynb`. W obu przypadkach na początek wybieramy Pythona 3, którego zainstalowaliśmy.

### Uruchom pierwszą komórkę

1. W komórce typu **Code** wpisz:

   ```python
   print("działa!")
   ```

2. Kliknij **▶** przy komórce lub naciśnij **Shift + Enter**.
3. Pod komórką powinien pojawić się wynik:

   ```text
   działa!
   ```

### Dodaj drugą komórkę

1. Kliknij **+ Code**.
2. Wpisz:

   ```python
   x = 10
   y = 20
   print(x + y)
   ```

3. Uruchom ją przez **Shift + Enter**.
4. Oczekiwany wynik: `30`.
5. Zapisz notatnik: **Ctrl + S** (Windows) lub **Cmd + S** (macOS).

Możesz także dodać komórkę **+ Markdown** — do zwykłego tekstu, notatek czy tytułów (nie do wykonywania kodu).

## 8. Jak pracować na zajęciach?

1. Otwórz VS Code i swój folder `informatyka`.
2. Otwórz lub utwórz notatnik `.ipynb`.
3. Sprawdź, czy po prawej stronie jest wybrany właściwy **kernel (Python 3)**.
4. Rozwiązuj zadania w kolejnych komórkach **Code**.
5. Uruchamiaj komórki przyciskiem **▶** lub skrótem **Shift + Enter**.
6. Sprawdzaj wyniki i regularnie zapisuj plik (**Ctrl/Cmd + S**).

**Uwaga na kolejność komórek.** Jeśli w pierwszej komórce wpiszesz i uruchomisz:

```python
liczba = 10
```

a w drugiej:

```python
print(liczba * 2)
```

...to wtedy zobaczysz `20`. Gdy uruchomisz drugą komórkę jako pierwszą po starcie kernela, pojawi się błąd, bo Python nie zna jeszcze zmiennej `liczba`. **Liczy się kolejność uruchamiania komórek, a nie tylko ich kolejność w pliku**

W razie potrzeby możesz wybrać **Restart Kernel**, a następnie uruchomić komórki ponownie, od góry.

## 9. Najczęstsze problemy

### „VS Code nie widzi Pythona”

- Zamknij i ponownie uruchom VS Code.
- Otwórz **Ctrl/Cmd + Shift + P → Python: Select Interpreter**.
- Wybierz zainstalowanego Pythona 3.
- Jeśli nie ma go na liście, sprawdź instalację z punktu 2.

### „Nie mogę uruchomić pliku `.ipynb`”

- Sprawdź, czy zainstalowane jest rozszerzenie **Jupyter**.
- Kliknij **Select Kernel** i wybierz środowisko Python 3.
- Jeśli VS Code prosi o instalację `ipykernel`, zaakceptuj ją.

### „Pojawia się błąd dotyczący `ipykernel`”

Najpierw skorzystaj z opcji instalacji proponowanej bezpośrednio przez VS Code. Jeśli to nie działa, otwórz w VS Code **Terminal → New Terminal** i spróbuj:

**Windows:**

```powershell
py -3 -m pip install ipykernel
```

**macOS:**

```bash
python3 -m pip install ipykernel
```

Potem ponownie wybierz kernel. Jeśli masz kilka środowisk Pythona, `ipykernel` musi zostać zainstalowany w tym, które wybierasz jako kernel.

### „Mam błąd w kodzie — czy coś źle zainstalowałem/zainstalowałam?”

Nie zawsze. Błąd może oznaczać zwykłą literówkę w kodzie. Na przykład:

```python
print("Hello"
```

nie zadziała, bo brakuje `)`. Poprawna wersja:

```python
print("Hello")
```

Komunikaty błędów są normalną częścią nauki programowania.

## 10. Lista kontrolna przed zajęciami

- [ ] Python 3 jest zainstalowany i pokazuje numer wersji.
- [ ] VS Code uruchamia się poprawnie.
- [ ] Rozszerzenia **Python** i **Jupyter** są zainstalowane.
- [ ] Mam folder `informatyka` otwarty w VS Code.
- [ ] Potrafię stworzyć i uruchomić plik `test.py` lub `test_notebook.ipynb`.
- [ ] Potrafię wybrać **kernel Python 3**.
- [ ] Potrafię zapisać plik.

**Jeśli wszystkie punkty są spełnione, środowisko jest przygotowane do zajęć.**

## 11. Oficjalne materiały pomocnicze

- [Python — pobieranie](https://www.python.org/downloads/)
- [Visual Studio Code — pobieranie](https://code.visualstudio.com/download)
- [Python w VS Code — samouczek](https://code.visualstudio.com/docs/python/python-tutorial)
- [Jupyter w VS Code — dokumentacja](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)
- [Zarządzanie kernelami Jupyter w VS Code](https://code.visualstudio.com/docs/datascience/jupyter-kernel-management)


## Alternatywa: Python bez instalacji

**Masz problem z instalacją, z którym nie jesteś sobie w stanie poradzić?** Zrób zrzut ekranu pokazujący komunikat błędu i przygotuj informację, czy korzystasz z Windows czy macOS i wyślij wiadomość na MS Teams z wyprzedzeniem.

### Alternatywnie...

Jeśli nie uda się Państwu zainstalować Pythona lub VS Code na własnym komputerze, można korzystać z narzędzi działających bezpośrednio w przeglądarce.

- **[Google Colab](https://colab.research.google.com/)** – zalecana alternatywa. Umożliwia tworzenie i uruchamianie notatników Jupyter (`.ipynb`) bez instalowania czegokolwiek na komputerze. Wymaga zalogowania na konto Google.

- **[Online Python](https://www.online-python.com/)** – prosty interpreter Pythona działający bezpośrednio w przeglądarce. Nie wymaga instalacji ani logowania. Nadaje się do pisania i uruchamiania krótkich programów w Pythonie.

**Na zajęcia polecam przede wszystkim Google Colab**, ponieważ pozwala pracować z notatnikami `.ipynb`, których będziemy używać podczas ćwiczeń.

Warto jednak docelowo skonfigurować lokalne środowisko Python + VS Code – przyda się ono szczególnie podczas przygotowywania projektu zaliczeniowego.