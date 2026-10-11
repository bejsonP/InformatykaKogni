---
marp: true
theme: default
paginate: true
header: "Informatyka 2026/2027"
style: |
  section {
    justify-content: flex-start;
    padding-top: 100px;
  }
  header {
    position: absolute;
    top: 25px;
    left: 50px;
    right: 50px;
    font-size: 18px;
    color: #666;
    border-bottom: 1px solid #ddd;
    padding-bottom: 10px;
  }
  section.center {
    justify-content: center;
    text-align: center;
  }
---
<!-- _class: center -->
<!-- _header: "" -->

# Informatyka

Computer Science · Kognitywistyka UJ
*2026/2027*

---

# Agenda

- Sprawy organizacyjne
- Plan ćwiczeń
- Warunki zaliczenia
- Główne środowisko pracy
- Zaczynamy...

---
<!-- _header: "Sprawy organizacyjne" -->

# Poznajmy się
Paweł Basoń
pawel.bason@doctoral.uj.edu.pl

Szkoła Doktorska Nauk Społecznych (CogNes), UJ
Katedra Kognitywistyki, UJ

performance monitoring · feedback processing · decision making · EEG methodology

---
<!-- _header: "Sprawy organizacyjne" -->

# Formuła zajęć
1. Na zajęciach:
    - przypomnienie zagadnień z poprzednich zajęć
    - krótki wykład wprowadzający
    - ćwiczenia realizowane indywidualnie lub w parach + konsultacje
    - wspólne omówienie ćwiczeń

2. Po zajęciach:
    - praca własna, przygotowanie do kolejnych zajęć

---
<!-- _header: "Sprawy organizacyjne" -->

# Warunki zaliczenia
- Projekt zaliczeniowy (20%)
- "Wejściówki" (40%)
- Kolokwium (40%)
- Aktywność (bonusowe max. +10%)

---
<!-- _header: "Sprawy organizacyjne" -->

## Projekt zaliczeniowy (20%)
- Do realizacji indywidualnie/w parach
    - jeżeli realizowany w parach - jasne wyszczególnienie odpowiedzialności za konkretne fragmenty
- Python
- Tematy zostaną podane w trakcie zajęć z Python
- Można realizować autorski pomysł (po konsultacji)
- Krótka "obrona" projektu - konsultacja dotycząca zawartości

---
<!-- _header: "Sprawy organizacyjne" -->

## "Wejściówki" (40%)
- Na samym początku zajęć (nie wszystkich)
- Domyślna forma: papier, sporadycznie komputer
- Liczba wejściówek zależna od prędkości realizacji zagadnień
- Możliwość "anulowania" wyniku jednej wejściówki
- Wejściówki z zajęć z nieobecnościami domyślnie oceniane na 0pkt, z możliwością nadrobienia

--- 
<!-- _header: "Sprawy organizacyjne" -->

## Kolokwium (40%)
- W ramach jednych z ostatnich zajęć
- Pytania teoretyczne + problemowe
- Możliwość korzystania z dokumentacji Pythona

---
<!-- _header: "Sprawy organizacyjne" -->

## Aktywność (bonusowe max. +10%)
- Do zebrania 10 pkt za aktywność
- Wyjście z inicjatywą w ramach zajęć (np. zgłoszenie się do rozwiązania ćwiczenia przed grupą, zaogniona dyskusja): +1 pkt
    - wywołanie kogoś przez prowadzącego nie wlicza się w aktywność
    - 3x w ramach jednych zajęć +2 pkt.
- Gdybym zapomniał to prosze przypomnijcie się pod koniec zajęć w danym dniu.
- Do oceny końcowej naliczają się po uwzględnieniu średniej z pozostałych elementów

---
<!-- _header: "Sprawy organizacyjne" -->

# Warunki zaliczenia


$$
Ocena =
\underbrace{
  0{,}2 \cdot \overline{P}
+ 0{,}4 \cdot \overline{W}
+ 0{,}4 \cdot K
}_{\text{wynik podstawowy}}
+ A
$$
gdzie:
- **P** — średnia z projektu zaliczeniowego (20%),
- **W** — średnia z wejściówek (40%),
- **K** — wynik kolokwium (40%),
- **A** — bonus za aktywność 

## Pytania?

---
<!-- _header: "Orientacyjny plan ćwiczeń" -->

- BLOK I. Podstawowe zagadnienia
- BLOK II. Podstawy programowania w języku Python
- BLOK III. Systemy operacyjne
- BLOK IV. Inne

---
<!-- _header: "Orientacyjny plan ćwiczeń. BLOK I" -->

## BLOK I. Podstawowe zagadnienia w informatyce
- Przygotowanie przestrzeni roboczej
- Systemy liczbowe
- Algorytmy, schematy blokowe i pseudokod

---
<!-- _header: "Orientacyjny plan ćwiczeń. BLOK II" -->

## BLOK II. Podstawy programowania w języku Python
- Wstęp do języka Python
- Podstawowe typy danych, operatory i operacje
- Instrukcje warunkowe
- Funkcje
- Klasy
- Moduły
- Operacje na plikach

---
<!-- _header: "Orientacyjny plan ćwiczeń. BLOK III" -->

## BLOK III. Systemy operacyjne
- Podstawy Linuxa
- Bash - podstawy

---
<!-- _header: "Orientacyjny plan ćwiczeń. BLOK IV" -->

## BLOK IV. Inne

- Inne jezyki programowania
- SQL

---
<!-- _header: "Sprawy organizacyjne" -->

# Obecności

- Dozwolone są **dwie nieobecności** z dowolnego powodu
- Wejściówki z nieobecności domyślnie liczą się jako 0 pkt, natomiast mozna je nadrobić


---
<!-- _header: "Sprawy organizacyjne" -->

# Obecności

W przypadku poważnych okoliczności (np. zdrowotnych), które wymagają
dostosowania toku studiów — takich jak:
- zwiększenie liczby dozwolonych nieobecności,
- przedłużenie terminów zaliczeń projektów,
- zmiana formy zaliczenia przedmiotu,
należy złożyć stosowną prośbę mailowo i/lub w sekretariacie.

---
<!-- _header: "Sprawy organizacyjne" -->

# Korzystanie z LLMów
Jak korzystać z LLMów:
- Używaj modeli LLM do wyjaśniania niejasnych koncepcji.
- Proś o wyjaśnienie błędów i tracebacku, gdy są dla Ciebie
niezrozumiałe, a następnie samodzielnie poprawiaj kod.
- Proś o wskazówki zamiast gotowych rozwiązań.
- Proś o uwagi dotyczące czytelności, nazewnictwa i zgodności z PEP 8.

---
<!-- _header: "Orientacyjny plan ćwiczeń. BLOK IV" -->

# Jak NIE korzystać z LLMów:
- Nie proś o gotowe, pełne rozwiązania.
- Nie opieraj się na informacjach ani API z modeli językowych
bez weryfikacji w dokumentacji.
- Nie usprawiedliwiaj się stwierdzeniem „bo tak powiedział LLM”.
- Nie “Vibe” koduj.

---
<!-- _header: "Orientacyjny plan ćwiczeń. BLOK IV" -->

# Główne środowisko pracy
- VS CODE
- https://www.python.org/downloads/