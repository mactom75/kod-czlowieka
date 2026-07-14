# 🏗️ Architektura systemu — Kod Człowieka

## Human Code Project — System Architecture

Projekt **Kod Człowieka (Human Code Project)** zakłada stworzenie otwartego, bezpiecznego i długoterminowego ekosystemu dla przyszłej ucieleśnionej sztucznej inteligencji — **Embodied AI**.

System ma łączyć fizyczne platformy sensoryczne, lokalne przetwarzanie danych, prywatność od początku projektowania oraz długoterminową infrastrukturę badawczą.

---

## 1. Główna zasada architektury

Najważniejsza zasada projektu brzmi:

> **Surowe dane prywatne pozostają lokalnie.  
> Do dalszej analizy trafiają wyłącznie bezpieczne reprezentacje badawcze.**

Projekt nie zakłada wysyłania do chmury:

- prywatnych nagrań audio,
- prywatnych nagrań wideo,
- treści rozmów,
- zdjęć twarzy,
- danych umożliwiających bezpośrednią identyfikację człowieka.

System powinien działać zgodnie z zasadami:

- Privacy by Design,
- Edge AI,
- minimalizacji danych,
- anonimizacji lub pseudonimizacji,
- długoterminowej wartości badawczej,
- bezpieczeństwa człowieka.

---

## 2. Warstwy systemu

Architektura projektu składa się z kilku głównych warstw:

```text
+-------------------------------------------------------------+
|  Warstwa 1: Fizyczna platforma sensoryczna                  |
|  Robot / zabawka / cyfrowy towarzysz / urządzenie domowe    |
+------------------------------+------------------------------+
                               |
                               v
+-------------------------------------------------------------+
|  Warstwa 2: Lokalne przetwarzanie Edge AI                   |
|  Analiza sygnałów, filtrowanie, anonimizacja, alarmy        |
+------------------------------+------------------------------+
                               |
                               v
+-------------------------------------------------------------+
|  Warstwa 3: Anonimowe reprezentacje badawcze                |
|  Wektory cech, statystyki, wzorce, modele interakcji        |
+------------------------------+------------------------------+
                               |
                               v
+-------------------------------------------------------------+
|  Warstwa 4: Bezpieczna infrastruktura badawcza              |
|  Chmura, repozytoria danych, modele Embodied AI             |
+------------------------------+------------------------------+
                               |
                               v
+-------------------------------------------------------------+
|  Warstwa 5: Ekosystem naukowy i społeczny                   |
|  Uczelnie, laboratoria, instytucje, partnerzy, Open Source  |
+-------------------------------------------------------------+
```

---

## 3. Warstwa fizyczna

Fizyczna platforma sensoryczna może przyjmować różne formy:

- miękka zabawka sensoryczna,
- robot opiekuńczy,
- robot rozwojowy,
- urządzenie domowe,
- platforma senioralna,
- cyfrowy towarzysz z elementami fizycznymi,
- prototyp laboratoryjny.

Celem urządzenia nie jest zastąpienie człowieka, rodzica, lekarza ani opiekuna.

Celem jest:

- zbieranie bezpiecznych danych sensorycznych,
- wspieranie bezpieczeństwa,
- obserwacja interakcji,
- analiza rozwoju,
- tworzenie długoterminowych reprezentacji doświadczenia,
- budowanie fundamentów dla Embodied AI.

---

## 4. Możliwe sensory

Pierwsze wersje urządzeń mogą wykorzystywać różne grupy czujników.

### Sensory ruchu

- IMU,
- akcelerometr,
- żyroskop,
- magnetometr,
- czujniki orientacji,
- czujniki położenia.

### Sensory dotyku

- czujniki nacisku,
- sensory haptyczne,
- tekstylne czujniki dotyku,
- matryce nacisku,
- czujniki zgięcia.

### Sensory odległości i przestrzeni

- ToF,
- LiDAR,
- czujniki podczerwieni,
- kamery głębi,
- czujniki zbliżeniowe.

### Sensory audio

System nie powinien zapisywać treści rozmów.

Może analizować wyłącznie cechy akustyczne, takie jak:

- natężenie dźwięku,
- tempo,
- ton,
- dynamika,
- poziom hałasu,
- sygnały stresu w otoczeniu.

### Sensory środowiskowe

- temperatura,
- wilgotność,
- jakość powietrza,
- lotne związki organiczne,
- dym,
- czad,
- zalanie,
- światło,
- mikroklimat.

---

## 5. Warstwa Edge AI

Warstwa Edge AI działa lokalnie na urządzeniu.

Jej zadaniem jest:

- analiza sygnałów w czasie rzeczywistym,
- odrzucanie danych surowych,
- anonimizacja,
- wykrywanie zdarzeń,
- reakcja alarmowa,
- tworzenie wektorów cech,
- ograniczenie ilości danych wysyłanych dalej.

Możliwe platformy techniczne:

- Raspberry Pi z akceleratorem AI,
- NVIDIA Jetson,
- Google Coral,
- moduły NPU,
- mikrokontrolery z akceleracją AI,
- przyszłe układy neuromorficzne.

---

## 6. Dane lokalne a dane badawcze

System rozróżnia dwa typy danych.

### Dane surowe

Dane surowe to między innymi:

- obraz z kamery,
- dźwięk z mikrofonu,
- treść rozmowy,
- twarz,
- głos,
- identyfikujące szczegóły otoczenia.

Te dane powinny pozostawać lokalnie i być usuwane po analizie, jeśli nie istnieje wyraźna, uzasadniona i zgodna z prawem potrzeba ich zachowania.

### Dane badawcze

Dane badawcze to anonimowe lub pseudonimizowane reprezentacje, takie jak:

- wektory ruchu,
- wektory dotyku,
- statystyki interakcji,
- wzorce zachowania,
- cechy środowiskowe,
- modele rozwoju w czasie,
- abstrakcyjne reprezentacje relacji człowiek–robot,
- sygnały bezpieczeństwa.

To właśnie te dane są długoterminową wartością projektu.

---

## 7. Tryb bezpieczeństwa i alarmów

System może działać jako dodatkowa warstwa wczesnego ostrzegania.

Możliwe wykrywane zdarzenia:

- upadek,
- bezruch,
- możliwy bezdech,
- możliwe zadławienie,
- czad,
- dym,
- pożar,
- zalanie,
- gwałtowna zmiana zachowania,
- nietypowy wzorzec ruchu,
- sytuacja wymagająca sprawdzenia przez człowieka.

System nie stawia diagnozy medycznej.

Każdy alarm powinien być traktowany jako:

> **sygnał wymagający sprawdzenia przez człowieka, a nie pewna diagnoza.**

---

## 8. Warstwa chmury badawczej

Chmura badawcza nie powinna przechowywać prywatnych surowych nagrań.

Jej zadaniem jest:

- przechowywanie anonimowych reprezentacji badawczych,
- analiza długoterminowych trendów,
- uczenie modeli Embodied AI,
- wspieranie badań naukowych,
- tworzenie statystyk rozwojowych,
- umożliwienie współpracy między instytucjami.

Dostęp do danych powinien być kontrolowany, audytowany i zgodny z zasadami etycznymi projektu.

---

## 9. Ciągłość danych

Największą wartością projektu jest ciągłość.

Dane zbierane przez dzień mają ograniczoną wartość.  
Dane zbierane przez lata mogą ujawnić procesy, których nie da się zobaczyć w krótkim eksperymencie.

Ciągłość danych może pomóc badać:

- rozwój dziecka,
- dojrzewanie,
- zmiany zachowania,
- starzenie się,
- samotność,
- relacje społeczne,
- wpływ środowiska,
- wczesne sygnały ryzyka,
- skutki pozytywnych i negatywnych doświadczeń.

---

## 10. Architektura partnerstw

Projekt może współpracować z:

- uczelniami,
- instytutami badawczymi,
- państwem,
- samorządami,
- spółkami państwowymi,
- firmami technologicznymi,
- firmami ubezpieczeniowymi,
- bankami,
- fundacjami,
- organizacjami społecznymi,
- partnerami przemysłowymi.

Partnerzy mogą wspierać:

- finansowanie,
- produkcję,
- badania,
- infrastrukturę,
- bezpieczeństwo,
- prototypowanie,
- wdrożenia pilotażowe.

Partnerzy nie mogą kupować dostępu do prywatnych danych człowieka.

---

## 11. Model rozwoju systemu

Projekt powinien rozwijać się etapami:

1. dokumentacja,
2. prototyp cyfrowy,
3. model danych,
4. prototyp sprzętowy,
5. testy laboratoryjne,
6. pilotaże z dorosłymi uczestnikami,
7. badania z udziałem instytucji,
8. finansowanie grantowe,
9. rozwój w Polsce,
10. rozwój w Europie,
11. otwarty ekosystem globalny.

---

## 12. Zasada końcowa

> **Architektura systemu musi być podporządkowana człowiekowi.  
> Technologia, dane i modele AI są narzędziami — nie celem samym w sobie.**
