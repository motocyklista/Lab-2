#  Program: Przelicznik walut (PLN → USD)

Prosty program napisany w języku C, który przelicza kwotę w złotówkach (PLN) na dolary amerykańskie (USD) na podstawie podanego kursu walutowego.

---

##  Informacje techniczne

- **Język:** C  
- **Edytor:** Microsoft Visual Studio Code  
- **Kompilator:** `clang-cl` (z pakietu LLVM / Visual Studio)  
- **System:** Windows  

---

##  Kompilacja

Aby skompilować program, uruchom w terminalu polecenie:

```bash
clang-cl waluty.c
````

> 💡 **Uwaga:** Kompilator może wyświetlić ostrzeżenia dotyczące funkcji `scanf`.
> Jest to normalne w środowisku Visual Studio — można je pominąć lub użyć `scanf_s`.
> Jeśli chcesz wyłączyć ostrzeżenie, możesz dodać na początku pliku:
>
> ```c
> #define _CRT_SECURE_NO_WARNINGS
> ```

---

##  Uruchomienie programu

Po udanej kompilacji uruchom plik wykonywalny:

```bash
waluty.exe
```

---

###  Przykład działania

```
Podaj kwote w PLN: 10
Podaj kurs USD/PLN: 3.64
Kwota w dolarach USD: 2.75
```

---

##  Opis działania programu

1. Program wczytuje od użytkownika:

   * **amountPLN** – kwotę w złotówkach (PLN)
   * **rate** – kurs dolara (USD/PLN)

2. Oblicza **kwotę w dolarach** według wzoru:

   ```
   amountUSD = amountPLN / rate
   ```

3. Wynik jest zapisywany w zmiennej `amountUSD` i wyświetlany na ekranie z dokładnością do dwóch miejsc po przecinku:

   ```
   Kwota w dolarach USD: X.XX
   ```

4. Program kończy działanie po wyświetleniu wyniku.

---

## 👤 Autor

* **Imię / Pseudonim:** Piotr
* **Rok:** 2025
* **Środowisko:** Visual Studio Code + clang

---
