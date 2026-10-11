---
marp: true
theme: default
paginate: true
header: "Systemy liczbowe"
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

# Systemy liczbowe

15.10.2026 · Kognitywistyka UJ

---

# Podział systemów

1) **Systemy pozycyjne** – wartość, jaką cyfra wnosi do liczby, zależy od:
   - wartości samej cyfry
   - miejsca, które zajmuje w liczbie
   - podstawy systemu
   - przykład: *system dziesiętny*
2) **Systemy addytywne** (niepozycyjne) – wartość liczby to suma wartości wszystkich użytych w niej znaków, bez względu na ich położenie
   - przykład: *system rzymski*

---
<!-- _header: "Systemy liczbowe" -->

# Systemy addytywne

---
<!-- _header: "Systemy addytywne" -->

## System jedynkowy
Jedna linia = +1 do liczby
Przykłady:
- | = 1
- ||| = 3
- |||||||||| = 10
- |||||||||||||||||||||||||||||||||| = 34

---
<!-- _header: "Systemy addytywne" -->

## System rzymski*
Każdy symbol ma przypisaną wartość. Wartości dodajemy, a w określonych przypadkach odejmujemy.

- I = 1, V = 5, X = 10, L = 50, C = 100, D = 500, M = 1000

Przykłady:
- III = 1 + 1 + 1 = 3
- LXVI = 50 + 10 + 5 + 1 = 66
- XXIV* = 10 + 10 - 1 + 5 = 24


*System oparty na zasadzie addytywnej - w parach IV, IX, XL, XC, CD i CM występuje również odejmowanie

---
<!-- _header: "Systemy liczbowe" -->

# Systemy pozycyjne

---
<!-- _header: "System dziesiętny" -->

# System dziesiętny

## Podstawa: 10
## Cyfry: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9

---
<!-- _header: "System dziesiętny" -->
<style scoped>
li {font-size: 18px}
</style>

$$ \sum_{i=-m}^{n} a_i \cdot 10^i $$

gdzie:
- $a_i$ — cyfra na pozycji $i$, gdzie $a_i \in \{0,1,2,\ldots,9\}$.
- $i$ — numer pozycji względem przecinka:
  - $i = 0$ — jedności,
  - $i = 1$ — dziesiątki,
  - $i = 2$ — setki,
  - $i = -1$ — części dziesiąte,
  - $i = -2$ — części setne.
- $n$ — najwyższy numer pozycji w części całkowitej (ta część ma $n+1$ cyfr).
- $m$ — liczba cyfr po przecinku (dla $m>0$ ostatnia z nich ma pozycję $-m$).
- $10$ — podstawa systemu dziesiętnego.
- $10^i$ — waga przypisana cyfrze $a_i$.

---

## Przykład

$$
123{,}45_{(10)} = \sum_{i=-2}^{2} a_i \cdot 10^i
$$

Cyfry i ich pozycje:

$$
a_2=1,\quad a_1=2,\quad a_0=3,\quad a_{-1}=4,\quad a_{-2}=5
$$

Najwyższa pozycja to $n=2$, a liczba cyfr po przecinku to $m=2$.

$$
\begin{aligned}
123{,}45_{(10)}
&= 5 \cdot 10^{-2}
 + 4 \cdot 10^{-1}
 + 3 \cdot 10^0
 + 2 \cdot 10^1
 + 1 \cdot 10^2 \\
&= 0{,}05 + 0{,}4 + 3 + 20 + 100
\end{aligned}
$$

---

## Przykład 2

$$
72954_{(10)} = \sum_{i=0}^{4} a_i \cdot 10^i
$$

Cyfry i ich pozycje:

$$
a_0=4,\quad a_1=5,\quad a_2=9,\quad a_3=2,\quad a_4=7
$$

Najwyższa pozycja to $n=4$, a liczba cyfr po przecinku to $m=0$.

$$
\begin{aligned}
72954_{(10)}
&= 4 \cdot 10^{0}
 + 5 \cdot 10^{1}
 + 9 \cdot 10^2
 + 2 \cdot 10^3
 + 7 \cdot 10^4 \\
&= 4 + 50 + 900 + 2000 + 70000
\end{aligned}
$$

---
<!-- _header: "System binarny" -->

# System binarny (dwójkowy)

## Podstawa: 2
## Cyfry: 0, 1

---
<!-- _header: "System binarny" -->
<style scoped>
li {font-size: 18px}
</style>

$$
\sum_{i=-m}^{n} a_i \cdot 2^i
$$

gdzie:

- $a_i \in \{0,1\}$ — cyfra binarna (bit) na pozycji $i$,
- $i$ — numer pozycji względem przecinka; jedności zaczynają się od pozycji $0$,
- $2$ — podstawa systemu binarnego,
- $n$ — najwyższy numer pozycji w części całkowitej,
- $m$ — liczba cyfr po przecinku,
- $2^i$ — waga pozycji $i$.

---

## Przykład: konwersja BIN - DEC

$$
10101{,}01_{(2)} = \sum_{i=-2}^{4} a_i \cdot 2^i
$$

Cyfry i ich pozycje:

$$
a_4=1,\quad a_3=0,\quad a_2=1,\quad a_1=0,\quad a_0=1,\quad a_{-1}=0,\quad a_{-2}=1
$$

Najwyższa pozycja to $n=4$, a liczba cyfr po przecinku to $m=2$.

$$
\begin{aligned}
10101{,}01_{(2)}
&= 1 \cdot 2^{-2}
 + 0 \cdot 2^{-1}
 + 1 \cdot 2^0
 + 0 \cdot 2^1
 + 1 \cdot 2^2
 + 0 \cdot 2^3
 + 1 \cdot 2^4 \\
&= 1 \cdot (\frac{1}{2})^2
 + 0 \cdot (\frac{1}{2})^1
 + 1 \cdot 2^0
 + 0 \cdot 2^1
 + 1 \cdot 2^2
 + 0 \cdot 2^3
 + 1 \cdot 2^4 \\
&= 0{,}25 + 0 + 1 + 0 + 4 + 0 + 16\\
&= 21{,}25_{(10)}

\end{aligned}
$$

---

## Przykład 2: konwersja BIN - DEC

$$
111101_{(2)} = \sum_{i=0}^{5} a_i \cdot 2^i
$$

Cyfry i ich pozycje:

$$
a_5=1,\quad a_4=1,\quad a_3=1,\quad a_2=1,\quad a_1=0,\quad a_0=1
$$

Najwyższa pozycja to $n=5$, a liczba cyfr po przecinku to $m=0$.

$$
\begin{aligned}
111101_{(2)}
&= 1 \cdot 2^0
 + 0 \cdot 2^1
 + 1 \cdot 2^2
 + 1 \cdot 2^3
 + 1 \cdot 2^4
 + 1 \cdot 2^5 \\
&= 1 + 0 + 4 + 8 + 16 + 32\\
&= 61_{(10)}

\end{aligned}
$$

---

## Konwersja DEC - BIN
- Dzielimy nieujemną liczbę całkowitą przez 2 z resztą
- Zapisujemy resztę z dzielenia (0 lub 1)
- Iloraz całkowity ponownie dzielimy przez 2
- Powtarzamy aż iloraz całkowity będzie równy 0
- Odczytujemy reszty od końca

$$
\begin{aligned}
25 &= 12 \cdot 2 + 1 \quad \text{reszta } 1 \\
12 &= 6 \cdot 2 + 0 \quad \text{reszta } 0 \\
6  &= 3 \cdot 2 + 0 \quad \text{reszta } 0 \\
3  &= 1 \cdot 2 + 1 \quad \text{reszta } 1 \\
1  &= 0 \cdot 2 + 1 \quad \text{reszta } 1
\end{aligned}
$$

$$(25)_{10} = (11001)_2$$

---

## Konwersja DEC - BIN (część ułamkowa)
- mnożymy część ułamkową przez 2
- zapisujemy część całkowitą wyniku (0 lub 1)
- kontynuujemy mnożenie pozostałej części ułamkowej
- powtarzamy aż część ułamkowa będzie równa 0 lub uzyskamy ustaloną liczbę cyfr
- odczytujemy zapisane cyfry od początku

$$
\begin{aligned}
0{,}625 \cdot 2 &= 1{,}25 \quad \text{zapisujemy } 1 \\
0{,}25 \cdot 2 &= 0{,}5 \quad \text{zapisujemy } 0 \\
0{,}5 \cdot 2 &= 1{,}0 \quad \text{zapisujemy } 1
\end{aligned}
$$

$$(0{,}625)_{10} = (0{,}101)_2$$

---
<!-- _header: "System szesnastkowy" -->

# System szesnastkowy (HEX)

## Podstawa: 16
## Cyfry: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F

$$
A=10,\quad B=11,\quad C=12,\quad D=13,\quad E=14,\quad F=15
$$

---
<!-- _header: "System szesnastkowy" -->
<style scoped>
li {font-size: 18px}
</style>

$$
\sum_{i=-m}^{n} a_i \cdot 16^i
$$

gdzie:

- $a_i \in \{0,1,2,\ldots,15\}$ — wartość cyfry szesnastkowej na pozycji $i$,
- wartości od $10$ do $15$ zapisujemy cyframi $A, B, C, D, E, F$,
- $i$ — numer pozycji względem przecinka; jedności zaczynają się od pozycji $0$,
- $16$ — podstawa systemu szesnastkowego,
- $n$ — najwyższy numer pozycji w części całkowitej,
- $m$ — liczba cyfr po przecinku,
- $16^i$ — waga pozycji $i$.

---

## Przykład: konwersja HEX - DEC

$$
2A{,}C_{(16)} = \sum_{i=-1}^{1} a_i \cdot 16^i
$$

Cyfry i ich pozycje:

$$
a_1=2,\quad a_0=10\ (A),\quad a_{-1}=12\ (C)
$$

Najwyższa pozycja to $n=1$, a liczba cyfr po przecinku to $m=1$.

$$
\begin{aligned}
2A{,}C_{(16)}
&= 12 \cdot 16^{-1}
 + 10 \cdot 16^0
 + 2 \cdot 16^1 \\
&= 12 \cdot \frac{1}{16}
 + 10 \cdot 1
 + 2 \cdot 16 \\
&= 0{,}75 + 10 + 32\\
&= 42{,}75_{(10)}

\end{aligned}
$$

---

## Przykład 2: konwersja HEX - DEC

$$
2AF_{(16)} = \sum_{i=0}^{2} a_i \cdot 16^i
$$

Cyfry i ich pozycje:

$$
a_2=2,\quad a_1=10\ (A),\quad a_0=15\ (F)
$$

Najwyższa pozycja to $n=2$, a liczba cyfr po przecinku to $m=0$.

$$
\begin{aligned}
2AF_{(16)}
&= 15 \cdot 16^0
 + 10 \cdot 16^1
 + 2 \cdot 16^2 \\
&= 15 + 160 + 512\\
&= 687_{(10)}

\end{aligned}
$$

---

## Konwersja DEC - HEX
- Dzielimy nieujemną liczbę całkowitą przez 16 z resztą
- Zapisujemy resztę z dzielenia (od 0 do 15, wartości 10–15 jako A–F)
- Iloraz całkowity ponownie dzielimy przez 16
- Powtarzamy aż iloraz całkowity będzie równy 0
- Odczytujemy reszty od końca

$$
\begin{aligned}
687 &= 42 \cdot 16 + 15 \quad \text{reszta } 15 = F \\
42 &= 2 \cdot 16 + 10 \quad \text{reszta } 10 = A \\
2 &= 0 \cdot 16 + 2 \quad \text{reszta } 2
\end{aligned}
$$

$$(687)_{10} = (2AF)_{16}$$

---

## Konwersja DEC - HEX (część ułamkowa)
- mnożymy część ułamkową przez 16
- zapisujemy część całkowitą wyniku (wartości 10–15 jako A–F)
- kontynuujemy mnożenie pozostałej części ułamkowej
- powtarzamy aż część ułamkowa będzie równa 0 lub uzyskamy ustaloną liczbę cyfr
- odczytujemy zapisane cyfry od początku

$$
\begin{aligned}
0{,}671875 \cdot 16 &= 10{,}75 \quad \text{zapisujemy } A \\
0{,}75 \cdot 16 &= 12{,}0 \quad \text{zapisujemy } C
\end{aligned}
$$

$$(0{,}671875)_{10} = (0{,}AC)_{16}$$

---

## Konwersja HEX - BIN
- Każdą cyfrę szesnastkową zamieniamy na 4 cyfry binarne
- Łączymy otrzymane grupy w tej samej kolejności
- Zachowujemy położenie przecinka
- Możemy pominąć zera na początku części całkowitej

$$
\begin{aligned}
2_{(16)} &= 0010_{(2)} \\
A_{(16)} &= 1010_{(2)} \\
F_{(16)} &= 1111_{(2)}
\end{aligned}
$$

$$(2AF)_{16} = (0010\ 1010\ 1111)_2 = (1010101111)_2$$

---

## Konwersja HEX - BIN (część ułamkowa)
- Każdą cyfrę po przecinku zamieniamy na 4 cyfry binarne
- Łączymy otrzymane grupy w tej samej kolejności
- Możemy pominąć zera na końcu części ułamkowej

$$
\begin{aligned}
A_{(16)} &= 1010_{(2)} \\
C_{(16)} &= 1100_{(2)}
\end{aligned}
$$

$$(0{,}AC)_{16} = (0{,}1010\ 1100)_2 = (0{,}101011)_2$$

---

## Konwersja BIN - HEX
- Dzielimy część całkowitą na grupy po 4 cyfry, zaczynając od prawej strony
- Jeśli ostatnia grupa z lewej ma mniej niż 4 cyfry, uzupełniamy ją zerami z lewej
- Każdą grupę zamieniamy na jedną cyfrę szesnastkową

$$
1010101111_{(2)} = (0010\ 1010\ 1111)_2
$$

$$
\begin{aligned}
0010_{(2)} &= 2_{(16)} \\
1010_{(2)} &= A_{(16)} \\
1111_{(2)} &= F_{(16)}
\end{aligned}
$$

$$(1010101111)_2 = (2AF)_{16}$$

---

## Konwersja BIN - HEX (część ułamkowa)
- Dzielimy część ułamkową na grupy po 4 cyfry, zaczynając od przecinka w prawo
- Jeśli ostatnia grupa ma mniej niż 4 cyfry, uzupełniamy ją zerami z prawej
- Każdą grupę zamieniamy na jedną cyfrę szesnastkową

$$
0{,}101011_{(2)} = (0{,}1010\ 1100)_2
$$

$$
\begin{aligned}
1010_{(2)} &= A_{(16)} \\
1100_{(2)} &= C_{(16)}
\end{aligned}
$$

$$(0{,}101011)_2 = (0{,}AC)_{16}$$
