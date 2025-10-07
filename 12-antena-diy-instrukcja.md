# Budowa Anteny DIY - Instrukcje Krok po Kroku

## 🎯 O tym przewodniku

**Zawiera szczegółowe instrukcje budowy 3 anten:**
1. **Długi drut** (najłatwiejsza, ~30 zł, 1 godzina)
2. **Pętlowa AM** (średnia, ~50 zł, 2 godziny)
3. **Colinear ADS-B** (zaawansowana, ~20 zł, 1.5 godziny)

**Poziomy trudności:**
- 🟢 Łatwy - każdy da radę
- 🟡 Średni - potrzebne podstawowe umiejętności
- 🔴 Trudny - dla zaawansowanych

---

# 🔧 PROJEKT #1: Antena Długi Drut (End-Fed Long Wire)

**Poziom:** 🟢🟢 Łatwy  
**Koszt:** ~30 zł  
**Czas budowy:** 1 godzina  
**Zasięg:** Do 5x lepszy niż teleskopowa!  
**Dla pasm:** HF/SW (fale krótkie), częściowo MW

---

## 📋 Potrzebne materiały

### Lista zakupów:
- [ ] **Drut miedziany** 10-20 metrów (~20 zł)
  - Grubość: 0.5-2mm
  - Alternatywa: kabel elektryczny jednożyłowy (tańszy!)
- [ ] **Izolatory** x2 (~5 zł)
  - Ceramiczne lub plastikowe
  - Alternatywa: plastikowe słoiki, butelki
- [ ] **Przejściówka 3.5mm męska** z krokodylkami (~5 zł)
  - Lub przylutuj sam (gniazdo jack 3.5mm + kabel)
- [ ] **Linka nośna** (~10 zł) - opcjonalnie, jeśli drut ciężki
- [ ] **Zaciskarki/opaski** (~5 zł)

**RAZEM:** ~30-50 zł

### Narzędzia (najprawdopodobniej masz):
- Kombinerki / obcinaczki do drutu
- Taśma izolacyjna
- Linijka / miarka
- Opcjonalnie: lutownica (jeśli robisz przejściówkę sam)

---

## 📐 Projekt - schemat

```
                     ANTENA DŁUGI DRUT - WIDOK Z GÓRY
                     
   Punkt A                                                    Punkt B
  (balkon)                    Drut 10-20m                   (drzewo)
     |                                                          |
     |                                                          |
  Izolator ══════════════════════════════════════════════ Izolator
     ║                                                          
     ║ Przewód zniżkowy (1-2m)
     ║
     ▼
  ┌─────┐
  │ ATS │ ← Przejściówka 3.5mm
  │ Mini│
  └─────┘


                     WIDOK Z BOKU

         3-5m nad ziemią (im wyżej, tym lepiej!)
              │
    A ════════╪════════════════════════════════════ B
              │
              │ Przewód
              │ zniżkowy
              ▼
           Radio
```

---

## 🔨 Instrukcja montażu - krok po kroku

### KROK 1: Planowanie (10 min)

**Wybierz punkty mocowania:**
- **Punkt A:** Balkon, okno, rura na dachu
- **Punkt B:** Drzewo, słup, drugi budynek, maszt

**Zasady:**
- Odległość A-B: 10-20 metrów (im dłużej, tym lepiej dla HF!)
- Wysokość: **minimum 2-3m nad ziemią** (im wyżej, tym lepiej)
- **Nie nad osobami** (bezpieczeństwo)
- **Nie równolegle do linii elektrycznych** (zakłócenia!)

**Zmierz odległość:**
- Użyj taśmy mierniczej lub Google Maps (satellite view)
- Dodaj 1-2m zapasu na węzły

---

### KROK 2: Przygotowanie drutu (15 min)

**A. Odciągnij odpowiednią długość:**
- Długość główna (A-B): np. 15m
- Przewód zniżkowy: 1-2m
- **RAZEM:** 16-17m + zapas

**B. Przygotuj końce drutu:**

```
Koniec drutu (x2):
  
1. Odizoluj 3-5cm (jeśli kabel w izolacji)
   ═════════════════╪═════
                    └─ 5cm odsłonięte
                    
2. Zrób pętlę (do zaczepu w izolatorze)
          ┌─○─┐
   ═══════╪═══╪═════
          │   │
          └───┘ Pętla (~3cm średnicy)
          
3. Owiń końcem i zabezpiecz taśmą
          ┌─○─┐
   ═══════╪╳╳╳╪═════  ← Taśma izolacyjna
          │   │
          └───┘
```

**C. Przewód zniżkowy (1-2m):**
- Jeden koniec: pętla (jak wyżej)
- Drugi koniec: przygotuj do przejściówki 3.5mm

---

### KROK 3: Instalacja izolatorów (10 min)

**Co to jest izolator?**
Plastikowy/ceramiczny element, który:
- Trzyma drut naprężony
- Izoluje elektrycznie
- Zabezpiecza przed zwarciem

**Jak zamocować:**

```
OPCJA A: Izolator gotowy (ceramiczny)
   
   Punkt mocowania (hak, gałąź)
         │
         ○ ← Izolator ceramiczny
         │
    Pętla drutu


OPCJA B: DIY izolator (butelka PET)
   
   Punkt mocowania
         │
      ┌──┴──┐
      │     │ ← Butelka PET (0.5L)
      │  ○  │    Przewierć 2 dziury
      └──┬──┘
         │
    Pętla drutu
```

**Montaż:**
1. Załóż pętlę drutu na izolator
2. Izolator załóż na punkt A (balkon)
3. Powtórz dla punktu B (drzewo)

---

### KROK 4: Naciąganie drutu (15 min)

**⚠️ BEZPIECZEŃSTWO:**
- Nie rób tego podczas burzy!
- Nie naciągaj zbyt mocno (może się zerwać)
- Sprawdź czy nikt nie stoi pod drutem

**Procedura:**

1. **Zamocuj Punkt A** (np. balkon):
   - Izolator → hak/rura
   - Załóż pętlę drutu na izolator
   - Sprawdź mocowanie

2. **Rozciągnij drut** do punktu B:
   - Powoli, uważaj na przeszkody
   - Jeśli drzewo - użyj linki z obciążeniem (rzuć przez gałąź)

3. **Zamocuj Punkt B**:
   - Izolator → gałąź/słup
   - Pętla drutu na izolator
   - Naciągnij (nie za mocno!)

4. **Sprawdź naprężenie**:
   - Drut powinien być **naciągnięty, ale nie sztywny**
   - Może lekko zwisać (OK!)

---

### KROK 5: Przewód zniżkowy (10 min)

**Co to:** Krótki kawałek (1-2m) łączący drut główny z radiem

**Montaż:**

```
     Drut główny (poziomo)
    ═════════════╪═════════════
                 │
                 │ Połącz tutaj
                 │ (skręć + taśma)
                 │
                 ║ Przewód zniżkowy
                 ║ (1-2m, pionowo w dół)
                 ║
                 ║
                 ▼
              ┌─────┐
              │ 3.5 │ ← Przejściówka
              │ mm  │
              └─────┘
                 │
              ┌─────┐
              │ ATS │
              │ Mini│
              └─────┘
```

**Procedura:**
1. Znajdź miejsce na drucie (blisko okna/balkonu)
2. Odizoluj 5cm drutu głównego
3. Skręć przewód zniżkowy z drutem głównym
4. Owiń taśmą izolacyjną (wodoodpornie!)
5. Prowadź przewód zniżkowy do wnętrza (okno/drzwi)

---

### KROK 6: Przejściówka 3.5mm (10 min)

**OPCJA A: Gotowa z krokodylkami** (~5 zł)
```
Przewód zniżkowy ══════════╪══════ Krokodylek
                                   │
                                   ▼
                               ┌───┴───┐
                               │ 3.5mm │
                               │  jack │
                               └───────┘
                                   │
                               Do radia (ANT)
```
**Procedura:** Zaciśnij krokodylek na przewodzie → gotowe!

---

**OPCJA B: Lutowanie** (wymagana lutownica)
```
Przewód zniżkowy                    Kabel
       ║                              ║
       ║                              ║
       ╚══════════[LUTOWNICA]════════╝
                       │
                   Złącze 3.5mm
                   (masa = zewnętrzne)
                   (sygnał = środek)
```

**Procedura:**
1. Kup wtyk jack 3.5mm męski (~2 zł)
2. Przylutuj przewód do **środkowego pinu** (sygnał)
3. Masa (zewnętrzna) - zostaw odłączona lub uziemienie
4. Izoluj taśmą termokurczliwą

---

### KROK 7: Połączenie z radiem

1. **Włóż przejściówkę** w ATS Mini
   - ⚠️ Gniazdo **ANT** (nie słuchawki 🎧!)
2. Włącz radio
3. Wybierz tryb: **SW** (fale krótkie)
4. Ustaw częstotliwość: **7200 kHz**
5. Tryb: **USB**
6. **Słuchaj!**

**Efekt:** Powinno być **DUŻO lepiej** niż z teleskopową!

---

### KROK 8: Testowanie (15 min)

**Test porównawczy:**

| Antena | Częstotliwość | Tryb | Siła sygnału |
|--------|---------------|------|--------------|
| Teleskopowa | 7200 kHz | USB | S___ |
| **Długi drut** | 7200 kHz | USB | S___ |
| **Różnica:** | | | +___  |

**Jeśli długi drut daje +3-5 S → SUKCES!** 🎉

---

## ⚡ Optymalizacja

### Eksperymentuj z orientacją:
- **Poziomo** (jak instrukcja) - najlepsze dla HF/SW
- **Pod kątem 45°** (Inverted-L) - kompromis
- **Pionowo** (jeśli mało miejsca) - gorsze, ale działa

### Dodaj uziemienie (opcjonalnie, +20% zasięg):
```
    Drut główny
    ═════════════
         │
         │ Przewód zniżkowy
         ║
         ╬═══════════════════ Drugi drut do uziemienia
         ║                    (rura, pręt w ziemi)
         ▼
      Radio
```

**Jak zrobić:**
- Drugi drut (5-10m) podłącz do masy radia (zewnętrzna część jack 3.5mm)
- Drugi koniec do: rura grzewcza, pręt metalowy w ziemi (1m głębokości)

---

## ⚠️ BEZPIECZEŃSTWO - KRYTYCZNE!

### ❌ NIGDY:
- **Burza:** Odłącz antenę podczas burzy (ryzyko pioruna!)
- **Linie elektryczne:** Nie prowadź blisko linii wysokiego napięcia
- **Nad ludźmi:** Nie naciągaj nad miejscami, gdzie chodzą ludzie
- **Dotykanie:** Nie dotykaj drutu podczas słuchania (metalowy = przewodzi)

### ✅ ZAWSZE:
- Używaj izolatorów na obu końcach
- Odłączaj podczas burzy (wyciągnij jack z radia!)
- Sprawdzaj mocowania co 2-3 miesiące (korozja, zużycie)
- Jeśli uziemienie - pręt minimum 1m w ziemi

---

## 🐛 Troubleshooting

| Problem | Przyczyna | Rozwiązanie |
|---------|-----------|-------------|
| Brak poprawy vs teleskopowa | Za krótki drut | Wydłuż do 15-20m |
| Dużo szumów | Blisko linii elektrycznych | Przenieś antenę dalej |
| Drut spadł | Słabe mocowanie | Mocniejsze haki/izolatór |
| Bardzo słabe | Brak połączenia | Sprawdź skrętki (taśma!) |
| Działa, ale nie wow | Drut nisko | Podnieś wyżej (3-5m) |

---

## 📊 Oczekiwane wyniki

**Porównanie zasięgu (przybliżone):**

| Antena | HF/SW (7 MHz) | MW (1.5 MHz) | FM (100 MHz) |
|--------|---------------|--------------|--------------|
| Teleskopowa (20cm) | ⭐⭐ | ⭐ | ⭐⭐⭐⭐⭐ |
| **Długi drut 10m** | ⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ |
| **Długi drut 20m** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ |

**Typowa poprawa:** +3 do +7 jednostek S-meter!

---

## 💾 Backup - Alternatywy

### Jeśli nie masz balkonu:
- **Okno → słup uliczny** (jeśli blisko)
- **Wewnątrz mieszkania** wzdłuż ścian (gorsze, ale działa!)
- **Na strychu** (poziomo pod sufitem)

### Jeśli wynajmujesz / nie możesz montować:
- **Przenośna wersja:** Drut nawinięty na szpulę, rozwijany tylko podczas słuchania
- **Indoor:** Drut przyklejony taśmą do ściany (dyskretnie)

---

# 🔧 PROJEKT #2: Antena Pętlowa AM (Loop Antenna)

**Poziom:** 🟡🟡 Średni  
**Koszt:** ~50 zł  
**Czas budowy:** 2 godziny  
**Zasięg:** Świetny dla AM/MW, kierunkowa!  
**Dla pasm:** MW (fale średnie), częściowo SW

---

## 📋 Materiały

- [ ] **Drut miedziany grubszy** 2mm, 3 metry (~20 zł)
- [ ] **Rama** (30-50 cm średnicy):
  - Hula-hoop
  - Drewniany krzyż + sznurek
  - Plastikowa rurka
  - DIY z desek (~15 zł)
- [ ] **Kondensator zmienny** 200-500 pF (~30 zł) - opcjonalnie
  - Kupno: AliExpress "variable capacitor 500pF"
- [ ] **Przejściówka 3.5mm** (~5 zł)
- [ ] **Podstawa** (do postawienia anteny pionowo)

**RAZEM:** ~50-70 zł

---

## 📐 Projekt - schemat

```
         ANTENA PĘTLOWA - WIDOK Z PRZODU

              ╔═══════════════╗
             ╔╝               ╚╗
            ╔╝                 ╚╗
           ╔╝   RAMA (50cm)     ╚╗
           ║                     ║
           ║   10-15 zwojów      ║  ← Drut nawinięty
           ║   drutu             ║
           ╚╗                   ╔╝
            ╚╗                 ╔╝
             ╚╗               ╔╝
              ╚═══════════════╝
                     │ │
                     │ │ Końce drutu
                     ▼ ▼
              ┌─────────────┐
              │ Kondensator │ ← Opcjonalny (dostrajanie)
              │   zmienny   │
              └──────┬──────┘
                     │
                 ┌───┴───┐
                 │ 3.5mm │
                 └───────┘
                     │
                  Do radia
```

---

## 🔨 Instrukcja montażu

### KROK 1: Budowa ramy (30 min)

**OPCJA A: Hula-hoop** (najłatwiejsza!)
- Kup hula-hoop średnicy 50-70 cm (~10 zł)
- Gotowe do nawijania!

**OPCJA B: Drewniany krzyż**
```
      50 cm
    │◄────►│
    │      │
────┼──────┼──── Listwy drewniane
    │      │     (2x 50cm, krzyż)
    │      │
    └──────┘
    
Obwiąż sznurkiem tworząc okrąg/kwadrat
```

**OPCJA C: Rurka plastikowa (PVC)**
- Kup 3m rurki PVC (średnica 20-30mm)
- Zegnij w okrąg, sklej końce

---

### KROK 2: Nawijanie drutu (45 min)

**Procedura:**
1. **Zaznacz start** na ramie (np. taśmą)
2. **Nawijaj drut** równomiernie:
   - Ilość zwojów: **10-15**
   - Odstępy: równomierne (~1-2cm między zwojami)
   - Kierunek: nie ma znaczenia (bylezawsze ten sam!)

```
Widok z boku (rama + nawinięty drut):

   ═══ Zwój 1
  ═══  Zwój 2
 ═══   Zwój 3
═══    ...
 ═══   Zwój 10
  ═══  Zwój 11
   ═══ Zwój 12

Końce drutu schodzą w dół →
```

3. **Zabezpiecz** zwoje:
   - Taśma co 10cm (żeby nie zsunęły się)
   - Klej gorący (best!)
   - Opaski plastikowe

4. **Końce drutu** (dolne):
   - Zostaw 20-30 cm luźne
   - To będą podłączenia do kondensatora/radia

---

### KROK 3: Kondensator zmienny (30 min) - OPCJONALNIE

**Dlaczego?** Dostrajanie - obracasz kondensator, zmienia się rezonans pętli → słyszysz lepiej konkretne częstotliwości.

**Montaż:**
```
Końce drutu z pętli
    │         │
    ▼         ▼
   (A)       (B) Końcówki kondensatora
    └────┬────┘
         │
    ┌────┴────┐
    │ Pokrętło│ ← Obracasz = dostrajanie
    │    ◉    │
    └────┬────┘
         │
    ┌────┴────┐
    │  3.5mm  │
    └─────────┘
```

**Bez kondensatora:**
Połącz końce drutu bezpośrednio z 3.5mm jack (prostsza wersja, nie przestrajna)

---

### KROK 4: Podstawa (15 min)

Antena musi stać **pionowo** i móc się **obracać**.

**OPCJA A: Podstawa DIY z deski**
```
       ║ Pętla
       ║
    ───╫─── Oś (śruba długa)
       ║
   ┌───┴───┐
   │ Deska │ ← Ciężka podstawa
   └───────┘
```

**OPCJA B: Statyw fotograficzny**
- Jeśli masz statyw - przymocuj taśmą
- Można obracać + łatwa regulacja

---

### KROK 5: Testowanie

1. Postaw antenę pionowo
2. Podłącz do ATS Mini (gniazdo ANT)
3. Tryb: **AM** lub **MW**
4. Częstotliwość: **1602 kHz** (Radio Maryja - łatwy test)
5. **Obracaj pętlę** powoli 360°

**Efekt:** Sygnał się zmienia! Najsilniejszy gdy płaszczyzna pętli jest prostopadła do nadajnika.

**To jest zaleta pętli - możesz "celować" w stację i tłumić zakłócenia!**

---

## ⚡ Zastosowanie praktyczne

### Kiedy używać pętli?
- **Słabe stacje MW/AM** - pętla wzmacnia
- **Zakłócenia** - obróć pętlę, żeby stłumić źródło zakłóceń (np. LED)
- **Kierunkowość** - szukasz skąd nadaje stacja

### Najlepsze ustawienie:
- **Pionowo** (dla MW)
- **Możliwość obrotu** (musisz móc kręcić!)
- **Daleko od metalu** (zdestrój, kabelbłyszcz)

---

## 💾 Troubleshooting

| Problem | Rozwiązanie |
|---------|-------------|
| Słabe vs teleskopowa | Więcej zwojów (do 20), większa średnica |
| Szumy | Odsuń od elektroniki |
| Nie ma kierunkowości | Sprawdź czy pętla pionowo |
| Zwoje zsuwają się | Lepsze mocowanie (klej gorący) |

---

# 🔧 PROJEKT #3: Antena Colinear 1090 MHz (ADS-B)

**Poziom:** 🔴🔴🔴 Zaawansowany  
**Koszt:** ~20 zł  
**Czas budowy:** 1.5 godziny  
**Zasięg:** 200-300 km dla samolotów!  
**Dla:** RTL-SDR + ADS-B (śledzenie samolotów)

⚠️ **To dla zaawansowanych!** Wymaga precyzji (długości ±2mm!) i lutownicy.

---

## 📋 Materiały

- [ ] **Kabel koncentryczny RG-6** 75Ω, 50 cm (~10 zł)
  - TV SAT cable (tani w sklepach budowlanych)
- [ ] **Złącze SMA męskie** (~5 zł)
  - Do przylutowania
- [ ] **Rurka PVC** 20mm średnica, 50 cm (~5 zł)
  - Obudowa/sztywność
- [ ] Nóż ostry, obcinaczki, lutownica
- [ ] Taśma izolacyjna
- [ ] Linijka precyzyjna (milimetry!)

---

## 📐 Wymiary KRYTYCZNE (dla 1090 MHz)

**Obliczenia:**
```
Długość fali: λ = 300 / 1090 MHz = 27.5 cm
Dipol (λ/2): 27.5 / 2 = 13.75 cm
Quarter-wave (λ/4): 27.5 / 4 = 6.875 cm
```

**Konstrukcja Colinear (4 elementy):**
```
         Złącze SMA
             │
    ─────────┴─────────  7.3 cm (rdzeń + ekran)
             │
    ╌╌╌╌╌╌╌╌╌│╌╌╌╌╌╌╌╌╌  4.8 cm (brak ekranu - tylko rdzeń)
             │
    ─────────┼─────────  7.3 cm (rdzeń + ekran)
             │
    ╌╌╌╌╌╌╌╌╌│╌╌╌╌╌╌╌╌╌  4.8 cm (brak ekranu - tylko rdzeń)
             │
    ─────────┴─────────  7.3 cm (rdzeń + ekran)
           KONIEC

Łącznie: ~50 cm długości
```

---

## 🔨 Instrukcja (bardzo skrócona - zobacz YouTube!)

1. **Zmierz i zaznacz** odcinki na kablu (dokładność ±2mm!)
2. **Obróbka kabla:**
   - Sekcje z ekranem: zostaw rdzeń + ekran
   - Sekcje bez ekranu: usuń ekran, zostaw tylko rdzeń (dielektryk)
3. **Przylutuj złącze SMA** na początku
4. **Włóż w rurkę PVC** (sztywność)
5. **Zamocuj pionowo** (np. na maszcie, przy oknie)

**UWAGA:** To skomplikowane - **szukaj na YouTube:**
- "DIY 1090 MHz collinear antenna"
- "ADS-B antenna RG6 colinear"

---

## 📊 Oczekiwane wyniki

**Zasięg ADS-B:**
- Fabryczna antena RTL-SDR: ~50-100 km
- **DIY Colinear:** 200-300 km! (5x lepiej!)

**Jeśli widzisz 30+ samolotów jednocześnie → SUKCES!**

---

## 📚 Podsumowanie wszystkich projektów

| Antena | Trudność | Koszt | Czas | Dla pasm |
|--------|----------|-------|------|----------|
| **Długi drut** | 🟢🟢 Łatwy | ~30 zł | 1h | HF/SW ⭐⭐⭐⭐⭐ |
| **Pętlowa** | 🟡🟡 Średni | ~50 zł | 2h | MW/AM ⭐⭐⭐⭐⭐ |
| **Colinear** | 🔴🔴🔴 Trudny | ~20 zł | 1.5h | ADS-B 1090 MHz ⭐⭐⭐⭐⭐ |

**Rekomendacja dla początkujących:** Zacznij od **długiego drutu** - najłatwiejszy, najtańszy, najlepszy efekt!

---

## 🎓 Co dalej?

1. ✅ Przeczytałeś instrukcje DIY
2. ➡️ **Wybierz projekt** (polecam długi drut!)
3. Kup materiały (max 50 zł)
4. Zarezerwuj sobotnie popołudnie (2-3h)
5. **ZBUDUJ!**
6. Testuj i notuj wyniki w dzienniku

**Po zbudowaniu pierwszej anteny - poczujesz się jak prawdziwy radiooperator!** 🛠️📻

---

*"Antena zbudowana własnymi rękami daje 2x więcej satysfakcji niż kupiona!"*