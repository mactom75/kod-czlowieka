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
