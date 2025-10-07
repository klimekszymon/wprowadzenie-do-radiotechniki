# RTL-SDR - Software Defined Radio dla Początkujących

## 🤔 Co to jest SDR?

### Tradycyjne radio (jak ATS Mini):
```
Antena → [Elektronika analogowa] → Głośnik
         (filtry, mieszacze,
          wzmacniacze fizyczne)
```

### SDR:
```
Antena → [Prosty odbiornik] → USB → Komputer → Głośnik
                                    (cała magia
                                     dzieje się
                                     w software!)
```

### Prosta analogia
**Tradycyjne radio** = stare radio tranzystorowe - wszystko sprzętowe, nie zmienisz.

**SDR** = smartfon - sprzęt prosty, ale aplikacje robią wszystko!

---

## 🎯 Dlaczego SDR jest rewolucyjny?

### 1. Widzisz wszystko naraz!
**Tradycyjne radio:** Słuchasz jednej częstotliwości  
**SDR:** Widzisz **cały zakres** na ekranie jednocześnie (jak spektrogram)

**Analogia:** To jak różnica między patrzeniem przez słomkę (jedno radio) a panoramą (SDR).

### 2. Software = elastyczność
Chcesz dekodować:
- ADS-B (samoloty)?
- NOAA (satelity pogodowe)?
- POCSAG (pagery)?
- DAB+ (radio cyfrowe)?

**Jedna sztuka sprzętu** + różne aplikacje = wszystko możliwe!

### 3. Analiza i nauka
Widzisz:
- Jak wygląda sygnał FM vs AM
- Gdzie są zakłócenia
- Jak propagacja się zmienia w czasie rzeczywistym
- Waterfall (historia sygnałów)

**To najlepsze narzędzie do NAUKI radiotechniki.**

---

## 💰 RTL-SDR vs ATS Mini - porównanie

| Cecha | ATS Mini | RTL-SDR |
|-------|----------|---------|
| **Zakres częstotliwości** | 0.5-108 MHz | 24-1766 MHz* |
| **Pasma** | LW, MW, HF, FM | VHF, UHF (bez HF!) |
| **Przenośność** | ✅ Kieszonkowy | ⚠️ Wymaga komputera |
| **Bateria** | ✅ Wbudowana | ❌ Przez USB z laptopa |
| **Wizualizacja** | Mały ekran | ✅✅ Pełny waterfall |
| **Tryby** | AM, FM, SSB | Wszystko + cyfrowe! |
| **Cena** | ~100-150 zł | ~100-150 zł |
| **Funkcje zaawansowane** | ❌ | ✅ Dekodowanie, nagrywanie |
| **Łatwość użycia** | ✅ Włącz i działa | ⚠️ Wymaga konfiguracji |

*Z konwerterem Up-converter można dodać HF (0-30 MHz)

### Wniosek:
**ATS Mini i RTL-SDR to IDEALNA PARA!**
- ATS Mini → HF/SW (fale krótkie, świat)
- RTL-SDR → VHF/UHF (lotnictwo, służby, PMR, ADS-B)

**Razem pokrywają 0.5-1766 MHz = prawie wszystko!**

---

## 🛒 Który SDR kupić? (Rekomendacje)

### 🥇 Najlepsza opcja dla początkujących:
**RTL-SDR Blog V4**  
- Cena: ~150-180 zł (AliExpress/Allegro)
- Zakres: 500 kHz - 1766 MHz (tak, ma trochę HF!)
- Stabilny, dobra jakość
- Bias-Tee (zasilanie anteny aktywnej)
- Filtry przeciwzakłóceniowe

**Gdzie kupić:**
- AliExpress: "RTL-SDR Blog V4"
- Allegro: szukaj "RTL2832U R820T2"
- Oficjalny sklep: rtl-sdr.com (wysyłka USA)

### 🥈 Alternatywa budżetowa:
**RTL-SDR Blog V3**  
- Cena: ~100-130 zł
- Zakres: 24-1766 MHz (bez HF)
- Świetny stosunek cena/jakość

### 🥉 Najtańsza (ale gorsza):
**Generyczny RTL2832U**  
- Cena: ~40-60 zł
- Jakość losowa (Chińskie klony)
- Może działać źle lub wcale

**Ostrzeżenie:** Za te ~50 zł różnicy kup Blog V3/V4 - będziesz zadowolony!

---

## 📦 Co dostaniesz w zestawie?

Typowy zestaw RTL-SDR Blog V4:
- Stick USB (sam SDR)
- 3x anteny:
  - Teleskopowa (dla VHF/UHF)
  - Dipol (dla VHF)
  - Mała do ADS-B
- Kabel USB przedłużacz
- Przejściówki SMA
- Instrukcja (po angielsku)

---

## 💻 Oprogramowanie - co zainstalować?

### Dla Windows:

#### 1. SDR# (SDR Sharp) - PODSTAWA
**Co to:** Najpopularniejsza aplikacja SDR  
**Gdzie:** airspy.com/download  
**Funkcje:**
- Waterfall (widmo częstotliwości)
- FM, AM, USB, LSB, WFM
- Nagrywanie
- Pluginy (rozszerzenia)

**Trudność:** ⭐⭐ Średnia (trzeba zainstalować sterowniki)

#### 2. HDSDR
**Co to:** Alternatywa dla SDR#  
**Gdzie:** hdsdr.de  
**Funkcje:** Podobne do SDR#, inna estetyka

#### 3. CubicSDR
**Co to:** Nowoczesny, ładny interfejs  
**Gdzie:** cubicsdr.com  
**Funkcje:** Multiplatforma (Windows, Mac, Linux)

---

### Dla Linux/Mac:

#### GQRX
**Gdzie:** gqrx.dk  
**Funkcje:** Jak SDR#, ale dla Linux/Mac  
**Trudność:** ⭐ Łatwa (instalacja z repozytorium)

---

### Aplikacje specjalistyczne:

| Aplikacja | Do czego służy | Gdzie pobrać |
|-----------|----------------|--------------|
| **dump1090** | ADS-B (samoloty) | github.com/flightaware |
| **WXtoImg** | NOAA (satelity pogodowe) | wxtoimgrestored.xyz |
| **Unitrunker** | Trunking (służby cyfrowe) | unitrunker.com |
| **DSD+** | DMR/P25 (radio cyfrowe) | dsdplus.com |
| **SDRangel** | Zaawansowane SDR (dla geeks) | github.com/f4exb |

---

## 🚀 Pierwsze kroki z RTL-SDR

### KROK 1: Instalacja sterowników (Windows)

#### Metoda automatyczna (polecana):
1. Pobierz **Zadig** - zadig.akeo.ie
2. Podłącz RTL-SDR do USB
3. Uruchom Zadig
4. Options → List All Devices
5. Z listy wybierz: "Bulk-in, Interface (Interface 0)"
6. Zainstaluj driver: **WinUSB** (klik "Replace Driver")
7. Czekaj 1-2 minuty

**Efekt:** Windows teraz "widzi" RTL-SDR jako urządzenie SDR.

---

### KROK 2: Pierwsze uruchomienie SDR#

1. Pobierz SDR# (airspy.com)
2. Rozpakuj do folderu (np. `C:\SDR`)
3. Uruchom: `SDRSharp.exe`
4. Góra: Wybierz **"RTL-SDR (USB)"**
5. Klik: **Play (▶)** - górny lewy róg

**Jeśli działa:** Zobaczysz waterfall (kolorową wizualizację)!

---

### KROK 3: Pierwsza stacja FM (15 min)

#### Ustawienia:
- **Radio:** RTL-SDR (USB)
- **Tryb:** WFM (Wideband FM)
- **Częstotliwość:** 88600000 Hz (88.6 MHz - PR Katowice)
- **Gain:** Auto (na początku)
- **Antena:** Teleskopowa pionowo, pełna długość

#### Strojenie:
- **Kółko myszy** - zmiana częstotliwości (gruba)
- **Klik w waterfall** - szybkie strojenie
- **Strzałki** - precyzyjne (0.1 MHz)

**Czy słyszysz muzykę/mowę?** ✅ Gratulacje! SDR działa!

---

### KROK 4: Eksploracja widma (30 min)

#### Ćwiczenie 1: Zobacz wszystkie FM jednocześnie
1. Ustaw: **87.5 MHz**
2. Patrz na waterfall
3. Zobacz **pionowe linie** - każda to stacja FM!
4. Klik na linię → słuchasz tej stacji

**To jest magia SDR - widzisz wszystko naraz!**

#### Ćwiczenie 2: Znajdź lotnisko
1. Tryb: **AM**
2. Częstotliwość: **118-137 MHz** (pasmo lotnicze)
3. Zobacz aktywność na waterfall
4. Klik na sygnał
5. Słuchaj rozmów pilot-wieża

**To legalne i fascynujące!**

---

## 🎨 Rozumienie waterfall (spektrogramu)

### Jak wygląda waterfall?
```
Oś X (poziomo) = Częstotliwość
Oś Y (pionowo) = Czas (przeszłość na górze, teraz na dole)
Kolory = Siła sygnału (niebieski = słaby, żółty/czerwony = mocny)
```

### Co widzisz?

#### Sygnał FM:
```
    ████████      <-- Szerokie pasmo (200 kHz)
    ████████
    ████████
```
**Dlaczego szerokie?** FM potrzebuje dużo miejsca dla dobrej jakości.

#### Sygnał AM:
```
      ██          <-- Wąskie (10 kHz)
      ██
      ██
```

#### Radioamator SSB:
```
     ██           <-- Bardzo wąskie (3 kHz)
     ██
     ██
```

#### Szum (brak sygnału):
```
  . . . .         <-- Kropki, bez struktury
  . . .
  . .
```

---

## 📡 Konfiguracja anten dla SDR

### Co dostaniesz w zestawie:

#### 1. Teleskopowa (15-50 cm)
**Dla:** FM radio, VHF ogólne  
**Użycie:** Pionowo, pełna długość

#### 2. Dipol (V-shape)
**Dla:** VHF/UHF (136-470 MHz)  
**Użycie:** Rozłóż na V (120° kąt)

#### 3. Mała ADS-B
**Dla:** 1090 MHz (samoloty)  
**Użycie:** Na oknie, pionowo

### Ulepszone anteny (do kupienia później):

#### Dla ADS-B (śledzenie samolotów):
- **FlightAware Prostick Plus** (~100 zł) - best in class
- **DIY Colinear** (~20 zł) - sam zrobisz z kabla

#### Dla VHF/UHF:
- **Discone 25-1300 MHz** (~150 zł) - wszystko w jednym
- **Nagoya UT-106UV** (~80 zł) - magnetyczna do auta

#### Dla HF (trzeba Up-converter):
- **Długi drut** (jak dla ATS Mini)
- **MLA-30+** (~250 zł) - aktywna pętla

---

## 🎯 Projekty praktyczne z RTL-SDR

### Projekt 1: Stacja odbioru ADS-B (NAJPOPULARNIEJSZY!)

**Co to robi?**  
Pokazuje samoloty w promieniu 200-300 km na mapie w czasie rzeczywistym.

**Czego potrzebujesz:**
- RTL-SDR Blog V4 (~150 zł)
- Antena ADS-B (w zestawie lub DIY)
- Komputer (lub Raspberry Pi)
- Oprogramowanie: dump1090

**Instrukcja (uproszczona):**
1. Zainstaluj dump1090 (Windows/Linux)
2. Podłącz RTL-SDR
3. Antena ADS-B na okno/balkon (pionowo)
4. Uruchom dump1090
5. Otwórz przeglądarkę: `localhost:8080`

**EFEKT:** Widzisz mapę z samolotami! 🛩️

**Bonus:** Możesz udostępniać dane do FlightRadar24/FlightAware i dostać **konto premium gratis**!

**Szczegóły:** Patrz `06-adsb-sledzenie-samolotow.md`

---

### Projekt 2: Odbiór satelitów NOAA (zdjęcia z kosmosu!)

**Co to robi?**  
Odbierasz sygnał z satelitów pogodowych NOAA i dekoduje na zdjęcie Ziemi!

**Czego potrzebujesz:**
- RTL-SDR
- Antena V-dipol
- WXtoImg (software)

**Jak to działa:**
1. Sprawdź przelot NOAA (strona: n2yo.com)
2. Ustaw antenę (kierunek przelotu)
3. Nagrywaj sygnał podczas przelotu (~15 min)
4. Dekoduj w WXtoImg

**EFEKT:** Masz zdjęcie Europy z kosmosu! 🛰️

**To wymaga praktyki, ale efekt WOW!**

---

### Projekt 3: Monitoring służb ratunkowych

**Co słuchasz:**
- Straż Pożarna
- Pogotowie Ratunkowe
- Policja (jeśli niezszyfrowana)

**Częstotliwości (przykładowe - sprawdź lokalne):**
- 154-156 MHz - Służby miejskie
- 160-162 MHz - Służby medyczne
- 169 MHz - Ratownictwo

**UWAGA PRAWNA:**  
W Polsce **odbiór jest legalny**, ale:
- ❌ Nie możesz używać informacji do celów przestępczych
- ❌ Nie możesz nagrywać i publikować
- ✅ Możesz słuchać dla hobby/edukacji

---

### Projekt 4: DAB+ Radio cyfrowe

**Co to:** Cyfrowe radio (lepsza jakość niż FM)

**Jak słuchać:**
1. SDR# + plugin DAB
2. Częstotliwość: 174-230 MHz (pasmo DAB+ w Polsce)
3. Dekoduj sygnał

**Efekt:** Radio w jakości CD!

---

## 🐛 Typowe problemy i rozwiązania

### Problem 1: "No device found" w SDR#
**Rozwiązanie:**
- Sprawdź czy RTL-SDR podłączony
- Zainstaluj sterowniki Zadig ponownie
- Spróbuj inny port USB

### Problem 2: Dużo szumów/zakłóceń
**Rozwiązanie:**
- Odsuń SDR od komputera (użyj przedłużacza USB)
- Wyłącz ładowarki, lampy LED
- Zmniejsz Gain (wzmocnienie)

### Problem 3: Słaby odbiór
**Rozwiązanie:**
- Lepsza antena!
- Antena wyżej, na okno/balkon
- Zwiększ Gain

### Problem 4: Overload / ADC Overload
**Rozwiązanie:**
- Zmniejsz Gain
- Włącz filtry w SDR#
- Odsuń antenę od silnych nadajników

---

## 💡 Wskazówki dla początkujących

### 1. Zacznij od FM
To najprostsze - zawsze działa, silne sygnały.

### 2. Eksperymentuj z Gain
- Za wysokie = szumy, przeciążenie
- Za niskie = słaby odbiór
- Złoty środek: 20-40 dB (zależy od anteny)

### 3. Używaj waterfall
To Twój najlepszy przyjaciel - widzisz gdzie coś jest zanim usłyszysz.

### 4. Notuj odkrycia
Ciekawy sygnał? Zapisz częstotliwość, godzinę, co to było.

### 5. Dołącz do społeczności
- r/RTLSDR (Reddit)
- Grupy FB o SDR
- radioreference.com (baza częstotliwości)

---

## 📚 Materiały do nauki

### YouTube:
- **"RTL-SDR Tutorial"** by KF6UJG
- **"Getting started with RTL-SDR"** by Tech Minds

### Strony:
- **rtl-sdr.com** - oficjalny blog, tutorials
- **sigidwiki.com** - rozpoznawanie sygnałów
- **radioreference.com** - baza częstotliwości

### Książki (dla zaawansowanych):
- "The Hobbyist's Guide to RTL-SDR" (darmowe PDF)

---

## 🎯 Kolejne kroki

### Po 1 miesiącu z SDR:
- [ ] Opanowałeś FM, AM, SSB
- [ ] Widzisz samoloty na ADS-B
- [ ] Złapałeś pierwszy satelita NOAA

### Po 3 miesiącach:
- [ ] Masz kilka anten zoptymalizowanych
- [ ] Dekodowanie sygnałów cyfrowych (DMR, P25)
- [ ] Udostępniasz dane ADS-B online

### Po 6 miesiącach:
- [ ] Rozważasz drugi SDR (HackRF, Airspy)
- [ ] Up-converter dla pasm HF
- [ ] Może nawet... licencja radioamatorska? 📻

---

## 🔗 Co dalej?

1. ✅ Przeczytałeś: `04-sdr-wprowadzenie.md`
2. ➡️ **NASTĘPNIE:**
   - `06-adsb-sledzenie-samolotow.md` - szczegółowy projekt ADS-B
   - `05-skanery-radiowe.md` - alternatywa dla SDR

---

**RTL-SDR otwiera drzwi do niewidzialnego świata fal radiowych.** 🌍📡

**Czy jesteś gotowy na przygodę?**

*Uwaga: SDR to zajęcie na lata, nie na dni. Ciesz się procesem!*