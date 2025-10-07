# ADS-B - Śledzenie Samolotów w Czasie Rzeczywistym

## ✈️ Co to jest ADS-B?

### Prosta definicja
**ADS-B** (Automatic Dependent Surveillance-Broadcast) to system, w którym **samoloty nadają swoją pozycję** przez radio.

### Jak to działa?
Każdy samolot co 1 sekundę wysyła:
- Swoją pozycję GPS (szerokość, długość, wysokość)
- Prędkość
- Kurs (kierunek lotu)
- Numer lotu (np. LOT123)
- Typ samolotu

**Częstotliwość:** 1090 MHz (UHF)  
**Zasięg:** ~300-400 km (zależy od wysokości samolotu i Twojej anteny)

### Analogia
To jak GPS w samochodzie, ale samolot **transmituje swoją pozycję do wszystkich**, nie tylko do siebie.

**Wyobraź sobie:** Każda taksówka w mieście co sekundę mówi przez radio "Jestem taksówka 123, jadę ulicą Główną, prędkość 50 km/h". Ty możesz słuchać i widzieć wszystkie taksówki na mapie!

---

## 🎯 Po co to komu?

### 1. Fascynacja lotnictwem
- Widzisz **każdy samolot** w promieniu 200-300 km
- Śledź loty rodziny/znajomych
- Zobacz szlaki międzynarodowe nad Polską

### 2. Edukacja
- Naucz się rozpoznawać typy samolotów (Boeing 737, Airbus A320)
- Zobacz jak wyglądają procedury ILS (lądowanie)
- Zrozum gęstość ruchu lotniczego

### 3. Praktyczność
- Sprawdź czy lot będzie na czas (widzisz samolot w powietrzu!)
- Monitoruj opóźnienia
- Ciekawostka na imprezie ("zobacz, LOT leci nad nami!")

### 4. Społeczność
Możesz **udostępniać** swoje dane do:
- **FlightRadar24** → dostaniesz konto Business (wartość ~600€/rok) GRATIS!
- **FlightAware** → konto Enterprise GRATIS
- **ADSBexchange** → wsparcie wolnej społeczności

---

## 🛠️ Czego potrzebujesz?

### Minimalna wersja (~150-200 zł):
1. **RTL-SDR Blog V3/V4** - ~150 zł
2. **Antena** - w zestawie (mała 1090 MHz)
3. **Komputer** - masz już (laptop/PC)
4. **Oprogramowanie** - darmowe (dump1090)

### Profesjonalna wersja (~400-600 zł):
1. **RTL-SDR + FlightAware Prostick Plus** - ~250 zł (wzmacniacz + filtr)
2. **Antena zewnętrzna** - DIY (~20 zł) lub gotowa (~100 zł)
3. **Raspberry Pi 4** - ~200 zł (stacja 24/7)
4. **Zasilacz, karta SD** - ~50 zł

---

## 📡 Która antena dla ADS-B?

### Opcja 1: Fabryczna (w zestawie RTL-SDR)
**Wygląd:** Mała antena ~10 cm

**Zalety:**
✅ Darmowa (w zestawie)  
✅ Działa od razu

**Wady:**
❌ Krótka → zasięg ~50-100 km  
❌ Nieoptymalna

**Efekt:** Zobaczysz samoloty nad miastem, ale nie daleko.

---

### Opcja 2: DIY Colinear (~20 zł) - POLECANA!
**Co to:** Antena z kawałka kabla koncentrycznego

**Czego potrzebujesz:**
- Kabel RG-6 lub RG-58 (75Ω / 50Ω) - 50 cm
- Złącze SMA męskie - ~5 zł
- Nóż, taśma izolacyjna

**Instrukcja budowy:**
Szukaj na YouTube: **"DIY 1090 MHz collinear antenna"**

**Popularna konstrukcja (długości dla RG-6):**
```
Złącze SMA
    |
    |--- 7.3 cm (ekran + rdzeń)
    |
    |--- Usunięta izolacja (4.8 cm)
    |
    |--- 7.3 cm (ekran + rdzeń)
    |
    |--- Usunięta izolacja (4.8 cm)
    |
    |--- 7.3 cm (koniec)
```

**Efekt:** Zasięg 150-250 km! (3-5x lepszy niż fabryczna)

**Koszt:** ~20 zł  
**Czas budowy:** 30-60 min

---

### Opcja 3: Gotowa antena zewnętrzna (~100-150 zł)
**Przykłady:**
- FlightAware ADS-B Antenna (~100 zł)
- DPD Productions 1090 MHz (~120 zł)

**Zalety:**
✅ Profesjonalna  
✅ Optimized dla 1090 MHz  
✅ Nie musisz lutować

**Wady:**
❌ Droższe  
❌ Trzeba czekać na wysyłkę

---

### Opcja 4: Antena bazowa + wzmacniacz (~250 zł)
**FlightAware Pro Stick Plus**  
= RTL-SDR + wzmacniacz + filtr w jednym

**Zalety:**
✅ Najlepszy odbiór  
✅ Filtr 1090 MHz (eliminuje zakłócenia)  
✅ Wzmacniacz LNA (słabe sygnały stają się mocne)

**Wady:**
❌ Najdroższe

**Dla kogo:** Chcesz stacji profesjonalnej / udostępniasz dane 24/7

---

## 🖥️ Oprogramowanie - krok po kroku

### Metoda 1: Windows - dump1090 (najprostsza)

#### KROK 1: Zainstaluj sterowniki RTL-SDR
Patrz: `04-sdr-wprowadzenie.md` → sekcja "Instalacja sterowników"

**Skrót:**
1. Pobierz Zadig (zadig.akeo.ie)
2. Podłącz RTL-SDR
3. Zainstaluj driver WinUSB

#### KROK 2: Pobierz dump1090
**Gdzie:** github.com/antirez/dump1090  
lub wersja Windows: github.com/MalcolmRobb/dump1090

**Jak uruchomić:**
1. Rozpakuj do folderu (np. `C:\dump1090`)
2. Otwórz CMD (wiersz poleceń)
3. Przejdź do folderu: `cd C:\dump1090`
4. Uruchom: `dump1090.exe --interactive --net`

**Co się stanie:**
- Zobaczy tekst z danymi samolotów (ICAO, lot, pozycja)
- W przeglądarce: `http://localhost:8080` → MAPA!

---

### Metoda 2: Raspberry Pi - PiAware (stacja 24/7)

**Co to:** Gotowy obraz systemu dla Raspberry Pi od FlightAware

#### KROK 1: Przygotowanie (koszt ~250 zł)
- **Raspberry Pi 4** (2GB RAM wystarczy) - ~200 zł
- **Karta microSD** 16GB - ~20 zł
- **Zasilacz USB-C** 3A - ~30 zł
- **RTL-SDR** - masz już
- **Antena** - DIY lub gotowa

#### KROK 2: Instalacja PiAware
1. Pobierz obraz: **flightaware.com/adsb/piaware/install**
2. Nagraj na kartę SD (użyj Etcher: balena.io/etcher)
3. Włóż kartę do Raspberry Pi
4. Podłącz RTL-SDR do USB
5. Podłącz zasilanie
6. Czekaj 5 minut (pierwsze uruchomienie)

#### KROK 3: Konfiguracja
1. W przeglądarce: `http://piaware.local` (lub IP Raspberry)
2. Zarejestruj konto FlightAware
3. Połącz stację z kontem
4. Gotowe!

**Efekt:** Twoja stacja pracuje 24/7, udostępnia dane do FlightAware, dostajesz konto Business GRATIS!

---

### Metoda 3: ADSBexchange (dla zaawansowanych)

**Dlaczego ADSBexchange?**
- FlightRadar24 **filtruje** niektóre samoloty (wojskowe, prywatne VIP)
- ADSBexchange pokazuje **WSZYSTKO** (uncensored)

**Instalacja:** Podobna do PiAware, ale używasz obrazu ADSBexchange

**Szczegóły:** adsbexchange.com/how-to-feed

---

## 📊 Interpretacja danych

### Co widzisz na mapie?

#### Ikony samolotów:
- **Samolot z niebieską strzałką** = komercyjny (LOT, Lufthansa)
- **Samolot żółty** = prywatny / cargo
- **Samolot czerwony** = sygnał słaby / stare dane
- **Helikopter** = oczywiście helikopter 🚁

#### Informacje po kliknięciu:
```
Flight: LOT123
Aircraft: Boeing 737-800
Altitude: 10000 m (33000 ft)
Speed: 850 km/h (460 knots)
Heading: 270° (West)
Squawk: 2000
```

### Co oznaczają poszczególne dane?

#### Altitude (wysokość):
- **0-3000 ft** = Start/lądowanie
- **30000-40000 ft** = przelot (typowo)
- **40000+ ft** = wysokopułapowy (biznes jet)

#### Speed (prędkość):
- **Ground speed** = prędkość względem ziemi
- **Typowo:** 800-900 km/h dla odrzutowców

#### Squawk (kod transpondera):
- **7700** = EMERGENCY! (awaria!)
- **7600** = Utrata łączności radiowej
- **7500** = Porwanie!
- **1200** = VFR (loty rekreacyjne, bez planu lotu)

**Jeśli widzisz 7700 - to prawdziwa awaria! Możesz śledzić jak ląduje.**

---

## 🎯 Optymalizacja zasięgu - jak widzieć dalej?

### 1. Antena wyżej = dalszy zasięg
**Matematyka:**
- Antena na ziemi → zasięg ~50 km (widoczność po horyzont)
- Antena 10m → zasięg ~150 km
- Antena 20m → zasięg ~200 km
- Antena 50m → zasięg ~300 km

**Dlaczego?** 1090 MHz to UHF - leci w linii prostej. Zakrzywienie Ziemi ogranicza zasięg!

**Rozwiązanie:**
- **Balkon/dach** - najwyżej jak można
- **Maszt** - jeśli masz ogród
- **Okno wysokiego piętra** - lepsze niż parter

---

### 2. Dobra antena
Patrz wyżej - DIY Colinear daje 3-5x lepszy zasięg niż fabryczna!

---

### 3. Filtr + wzmacniacz
**FlightAware Pro Stick Plus** zawiera:
- **Filtr 1090 MHz** - eliminuje zakłócenia z innych częstotliwości
- **LNA (Low Noise Amplifier)** - wzmacnia słabe sygnały

**Efekt:** +50-100 km zasięgu!

---

### 4. Kabel - im krótszy, tym lepiej
**Problem:** Kabel koncentryczny ma **straty** na UHF.

**Zasada:** Każde 10m kabla RG-58 = -3 dB (połowa mocy)

**Rozwiązanie:**
- RTL-SDR + Raspberry Pi **przy antenie** (na zewnątrz/strychu)
- Zasilanie przez PoE lub długi kabel USB
- Dane przez WiFi/Ethernet

---

### 5. Unikaj zakłóceń
**Źródła zakłóceń na 1090 MHz:**
- Routery WiFi (2.4 GHz harmonics)
- Telewizja cyfrowa (harmonics)
- Telefony komórkowe

**Rozwiązanie:**
- Antena **daleko od elektroniki**
- Użyj **filtra 1090 MHz**

---

## 📈 Statystyki i analiza

### Co możesz śledzić?

#### 1. Liczba samolotów dziennie
Typowo nad Mysłowicami/Górnym Śląskiem: **200-500 samolotów/dzień**

#### 2. Najwyżej latający
Rekord świata: ~15000m (50000 ft) - loty biznesowe

#### 3. Najszybszy
- Komercyjne: ~900-950 km/h (Boeing 777, 787)
- Wojskowe: ~2000+ km/h (myśliwce, jeśli wykryjesz)

#### 4. Najpopularniejsze trasy nad Polską
- Frankfurt → Warszawa
- Londyn → Kraków
- Amsterdam → Katowice

---

## 🌍 Udostępnianie danych - jak dostać darmowe konto?

### FlightRadar24 - Business Account (wartość ~600€/rok)

**Co dostajesz:**
- Brak reklam
- Pełna historia lotów (365 dni)
- Filmy z lotu (Cockpit view)
- Alerty dla wybranych samolotów
- Priorytetowy support

**Jak dostać:**
1. Zainstaluj FR24 feeder (instrukcja: flightradar24.com/share-your-data)
2. Udostępniaj dane 24/7
3. Po weryfikacji (kilka dni) → aktywują konto Business

**Wymóg:** Stacja 24/7 (Raspberry Pi)

---

### FlightAware - Enterprise Account

**Co dostajesz:**
- Rozszerzone alerty
- API access
- Premium maps

**Jak dostać:**
1. Zainstaluj PiAware (patrz wyżej)
2. Udostępniaj dane
3. Automatycznie dostajesz upgrade

---

### ADSBexchange - wsparcie społeczności

**Nie dają konta premium** (bo wszystko jest darmowe!), ale:
- Widzisz **wszystkie** samoloty (uncensored)
- Wspiersz wolną społeczność
- Dostęp do danych wojskowych, VIP (nie są filtrowane)

---

## 🐛 Problemy i rozwiązania

### Problem 1: Widzę 0 samolotów
**Sprawdź:**
- Czy antena podłączona?
- Czy RTL-SDR działa? (test w SDR#)
- Czy częstotliwość = 1090 MHz?
- Czy dump1090 działa?

**Rozwiązanie:**
- Test w SDR# na 1090 MHz - powinno być widać krótkie impulsy (piki)
- Jeśli nic nie ma → problem z anteną / lokalizacją

---

### Problem 2: Widzę tylko 1-2 samoloty
**Przyczyna:** Słaba antena lub złe miejsce

**Rozwiązanie:**
- Antena **wyżej** (balkon, dach)
- Lepsza antena (DIY colinear)
- Sprawdź kierunek (może budynek zasłania?)

---

### Problem 3: Samoloty "znikają" i "pojawiają się"
**Przyczyna:** Słaby sygnał lub zakłócenia

**Rozwiązanie:**
- Zwiększ gain w RTL-SDR (ale nie za dużo!)
- Filtr 1090 MHz
- Sprawdź kabel (może zły kontakt?)

---

### Problem 4: Overload / ADC Overflow
**Przyczyna:** Za duże wzmocnienie lub silny sygnał w pobliżu

**Rozwiązanie:**
- Zmniejsz gain
- Dodaj filtr (FlightAware Pro Stick ma wbudowany)

---

## 🎓 Projekt: 30 dni ze śledzeniem samolotów

### Tydzień 1: Setup podstawowy
- [ ] Dzień 1-2: Kup/zamów RTL-SDR
- [ ] Dzień 3-4: Zainstaluj oprogramowanie (dump1090)
- [ ] Dzień 5: Pierwsze samoloty na mapie!
- [ ] Dzień 6-7: Testuj różne pozycje anteny

### Tydzień 2: Optymalizacja
- [ ] Zbuduj DIY Colinear antenna
- [ ] Porównaj zasięg (fabryczna vs DIY)
- [ ] Znajdź najlepsze miejsce dla anteny

### Tydzień 3: Analiza
- [ ] Notuj statystyki codziennie (ile samolotów?)
- [ ] Jakie trasy najpopularniejsze?
- [ ] O której godzinie najwięcej ruchu?

### Tydzień 4: Społeczność
- [ ] Zainstaluj PiAware (jeśli masz Raspberry Pi)
- [ ] Zarejestruj feeder FlightRadar24/FlightAware
- [ ] Dostań darmowe konto premium! 🎉

**Efekt:** Po miesiącu śledzisz 200+ samolotów dziennie i masz profesjonalną stację!

---

## 📱 Aplikacje mobilne

### FlightRadar24 (iOS/Android)
**Funkcje:**
- Mapa w czasie rzeczywistym
- Informacje o lotach
- AR (Augmented Reality) - skieruj telefon w niebo, zobaczysz który samolot leci

**Cena:** Darmowa (z ograniczeniami) / Premium jeśli feedujesz dane

---

### FlightAware (iOS/Android)
Podobnie do FR24, inna baza danych.

---

### Plane Finder (iOS/Android)
Alternatywa, mniejsza społeczność.

---

## 🎯 Zaawansowane: Dekodowanie Mode S

**Co to:** Mode S to rozszerzone dane ADS-B:
- Identyfikacja samolotu (N-number, rejestracja)
- Dane o manewrach
- Intent (planowane zmiany kursu/wysokości)

**Jak dekodować:**
- **dump1090** już to robi!
- **ModeSdeco2** - zaawansowana analiza

**Dla geek'ów:** Możesz napisać własny parser w Pythonie!

---

## 📚 Co dalej?

1. ✅ Przeczytałeś: `06-adsb-sledzenie-samolotow.md`
2. ➡️ **NASTĘPNIE:**
   - `07-czestotliwosci-co-sluchac.md` - pełna lista częstotliwości
   - `08-slownik-pojec.md` - wszystkie terminy wyjaśnione

---

**ADS-B to najlepsza zabawa z radiem - widzisz efekty od razu!** ✈️📡

**Miłego śledzenia!**

*Pro tip: Jak pierwszy raz zobaczysz 50 samolotów na mapie jednocześnie, będziesz w szoku jak gęsty jest ruch nad Polską!*