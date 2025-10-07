# Skanery Radiowe - Kompletny Przewodnik

## 🤔 Co to jest skaner radiowy?

### Prosta definicja
Skaner to radio, które **automatycznie przeskakuje** między częstotliwościami i **zatrzymuje się**, gdy coś nadaje.

### Analogia
Wyobraź sobie, że masz 100 stacji radiowych:
- **Zwykłe radio:** Musisz ręcznie przełączać każdą z nich
- **Skaner:** Radio samo przeskakuje wszystkie 100 i zatrzymuje się gdy coś mówi

**To jak "patrol" po falach radiowych.**

---

## 📻 Skaner vs ATS Mini vs RTL-SDR

| Cecha | ATS Mini | RTL-SDR | Skaner |
|-------|----------|---------|--------|
| **Auto-skanowanie** | ❌ Musisz ręcznie | ⚠️ W software | ✅ Wbudowane |
| **Przenośność** | ✅✅ Kieszonkowy | ❌ Wymaga laptop | ✅ Przenośny |
| **Pasma HF/SW** | ✅✅ Doskonałe | ❌* | ❌ Rzadko |
| **Pasma VHF/UHF** | ✅ Tak | ✅✅ Doskonałe | ✅✅ Doskonałe |
| **Do auta** | ⚠️ Niewygodne | ❌ | ✅ Często 12V |
| **Bateria** | ✅ Wbudowana | ❌ USB | ✅ Baterie/akumulator |
| **Łatwość obsługi** | ✅ Prosta | ⚠️ Wymaga PC | ✅ Bardzo prosta |
| **Cena** | ~150 zł | ~150 zł | ~400-800 zł |
| **Złącze anteny** | 3.5mm jack | SMA | BNC/SMA |

*RTL-SDR bez konwertera Up-converter

### Kiedy wybrać skaner zamiast ATS Mini lub SDR?

#### ✅ Skaner jest dla Ciebie jeśli:
- Interesują Cię **VHF/UHF** (lotnictwo, służby, PMR)
- Chcesz **mobilności** (auto, góry, miasto)
- Nie potrzebujesz **fal krótkich HF**
- Chcesz **prostoty** - włącz i słuchaj
- Lubisz "polować" na aktywne rozmowy

#### ❌ Skaner NIE jest dla Ciebie jeśli:
- Interesują Cię **fale krótkie SW** (stacje zagraniczne)
- Masz mały budżet (ATS Mini + SDR = tyle co skaner)
- Chcesz **wizualizacji** (waterfall)
- Potrzebujesz dekodowania cyfrowego (lepszy SDR)

---

## 🎯 Rodzaje skanerów

### 1. Podstawowe skanery ręczne
**Opis:** Małe, jak krótkofalówka, do ręki lub paska

**Przykłady:**
- Uniden Bearcat BC125AT
- Whistler WS1040
- Albrecht AE 125H

**Zakres:** Zwykle 25-512 MHz + 806-960 MHz  
**Cena:** ~400-700 zł  
**Dla kogo:** Hobbyści, początkujący

---

### 2. Skanery bazowe/stacjonarne
**Opis:** Większe, do domu/auta, często więcej funkcji

**Przykłady:**
- Uniden HomePatrol-2
- Whistler TRX-1
- Uniden SDS100

**Zakres:** Szerszy, często 25-1300 MHz  
**Cena:** ~800-2500 zł  
**Dla kogo:** Zaawansowani, stacje nasłuchowe

---

### 3. "Skanery" mobilne (faktycznie to transceivery)
**Opis:** Radio dwukierunkowe z funkcją skanowania

**Przykłady:**
- Baofeng UV-5R (~100 zł)
- Yaesu VX-6R (~800 zł)
- Icom IC-V86 (~600 zł)

**Zakres:** Zwykle 136-174 MHz (VHF) + 400-520 MHz (UHF)  
**Cena:** ~100-1000 zł  
**Dla kogo:** Radioamatorzy, prepperzy

**⚠️ UWAGA:** To **nadajniki** - bez licencji możesz nadawać TYLKO na PMR (446 MHz, 0.5W)!

---

## 🏆 Rekomendowane modele dla początkujących

### 🥇 Najlepszy wybór: Uniden Bearcat BC125AT
**Cena:** ~500-700 zł (Allegro, eBay)

**Specyfikacja:**
- Zakres: 25-512 MHz + 806-960 MHz
- 500 kanałów w pamięci
- Prosty w obsłudze
- Zasilanie: 2x AA baterie
- Złącze: BNC

**Zalety:**
✅ Legendarna niezawodność  
✅ Prosty dla początkujących  
✅ Dobra czułość  
✅ Close Call (wykrywa silne sygnały w pobliżu)

**Wady:**
❌ Bez trunking (cyfrowe systemy)  
❌ Droższy niż Baofeng  
❌ Nie ma HF

**Dla kogo:** Ktoś kto serio myśli o nasłuchach VHF/UHF

---

### 🥈 Budżetowa opcja: Baofeng UV-5R
**Cena:** ~100-150 zł (AliExpress, Allegro)

**Specyfikacja:**
- Zakres: 136-174 MHz (VHF) + 400-520 MHz (UHF)
- 128 kanałów
- Funkcja skanowania
- Zasilanie: Akumulator Li-Ion (wbudowany)
- Złącze: SMA

**Zalety:**
✅ BARDZO TANI (~100 zł)  
✅ Kompaktowy  
✅ Może nadawać (PMR 446 MHz legalnie)  
✅ Dobry do nauki

**Wady:**
❌ Słaba jakość audio  
❌ Interfejs "z lat 90."  
❌ Funkcje nadawcze = pokusa nielegalnego użycia  
❌ Wąski zakres

**Dla kogo:** 
- Budżet do 150 zł
- Chcesz **również** nadawać na PMR
- Nie przeszkadza Ci kiepski interfejs

**⚠️ Legalne użycie:**
- ✅ Słuchanie: wszystko OK
- ✅ Nadawanie na PMR 446 MHz (max 0.5W)
- ❌ Nadawanie gdzie indziej = NIELEGALNE bez licencji!

---

### 🥉 Średnia półka: Whistler WS1040
**Cena:** ~600-800 zł

**Specyfikacja:**
- Zakres: 29-512 MHz + 764-1300 MHz
- 1800 kanałów
- Skywarn (alerty pogodowe - USA)
- Zasilanie: 2x AA
- Złącze: BNC

**Zalety:**
✅ Szeroki zakres  
✅ Dużo pamięci  
✅ Łatwa programowanie (software)

**Wady:**
❌ Droższy  
❌ Niektóre funkcje dla rynku USA

**Dla kogo:** Zaawansowani użytkownicy z budżetem

---

## 📋 Czego słuchać skanerem?

### 1. Lotnictwo (118-137 MHz) - AM
**Co słyszysz:** Rozmowy pilot-wieża kontrolna

**Przykładowe częstotliwości (Polska):**
- 118.100 MHz - Katowice Tower
- 119.100 MHz - Katowice Approach
- 120.900 MHz - Kraków Tower
- 121.500 MHz - **Częstotliwość awaryjna lotnicza**

**Jak słuchać:**
1. Tryb: **AM** (nie FM!)
2. Ustaw częstotliwość lotniska
3. Słuchaj rozmów

**Co usłyszysz:**
> "Katowice Tower, LOT 123, final runway 27"  
> "LOT 123, cleared to land runway 27, wind 270 at 10 knots"

**To fascynujące i 100% legalne!** ✈️

**Baza lotnisk:** airnav.com, skyvector.com

---

### 2. PMR (446 MHz) - FM
**Co to:** Personal Mobile Radio - krótkofalówki cywilne

**Częstotliwości:**
- 446.00625 MHz (Kanał 1)
- 446.01875 MHz (Kanał 2)
- ...
- 446.09375 MHz (Kanał 8) - **awaryjny**

**Co usłyszysz:**
- Rodziny na wycieczce
- Ochrona sklepów
- Budowy
- Imprezy masowe
- Czasem... ciekawe rozmowy 😄

**Tryb:** FM  
**Legalność:** ✅ Słuchanie OK

---

### 3. Służby ratunkowe (różne częstotliwości)
**UWAGA PRAWNA:** W Polsce słuchanie jest legalne, ale:
- ❌ Nie możesz używać informacji do przestępstw
- ❌ Nie możesz publikować nagrań
- ✅ Możesz słuchać dla hobby

**Przykładowe częstotliwości (zależne od regionu):**
- 154-156 MHz - Straż Miejska, niektóre służby
- 160-162 MHz - Pogotowie (częściowo)
- 169 MHz - Ratownictwo

**Problem:** Wiele służb przeszło na **cyfrę zaszyfrowaną** (TETRA) - nie posłuchasz.

**Sprawdź lokalne:** radioreference.com (baza światowa)

---

### 4. Radioamatorzy VHF/UHF
**Pasma amatorskie:**
- **144-146 MHz** (2m) - VHF
- **430-440 MHz** (70cm) - UHF

**Co usłyszysz:**
- Rozmowy między operatorami
- Testy sprzętu
- Contestów (konkursy)
- Czasem ciekawe rozmowy techniczne

**Tryb:** FM (lokalnie), SSB (daleki zasięg)

---

### 5. Marine (morze/statki) - opcjonalnie
**Jeśli mieszkasz blisko morza:**
- 156.800 MHz - **Kanał 16** (awaryjny)
- 156-158 MHz - łączność morska

**Tryb:** FM

---

## 🛠️ Jak używać skanera - krok po kroku

### FAZA 1: Przygotowanie (dzień 1)

#### 1. Rozpakownie i ładowanie
- Włóż baterie / naładuj akumulator
- Przeczytaj instrukcję (przynajmniej podstawy!)
- Załącz antenę

#### 2. Pierwsze włączenie
- Włącz (przycisk Power)
- Ustaw głośność (50-70%)
- Sprawdź poziom baterii

---

### FAZA 2: Programowanie (dzień 1-2)

Większość skanerów wymaga **zaprogramowania częstotliwości**.

#### Metoda 1: Ręcznie (dla 5-10 kanałów)
**Przykład dla Uniden BC125AT:**
1. Tryb PROGRAM
2. Wybierz numer kanału (np. 1)
3. Wpisz częstotliwość: 118.100 MHz
4. Zapisz (ENTER)
5. Powtórz dla kolejnych kanałów

#### Metoda 2: Software (dla 100+ kanałów)
**Dla większości skanerów istnieje PC software:**
- Uniden: Sentinel/BCTools
- Whistler: EZ-Scan
- Baofeng: CHIRP (darmowy!)

**Procedura:**
1. Podłącz skaner do PC (kabel USB/szeregowy)
2. Uruchom software
3. Zaimportuj listę częstotliwości (CSV lub baza)
4. Zapisz do skanera

**Bazy częstotliwości:**
- radioreference.com - globalna baza
- przemien.net - Polska baza (mniej aktualna)

---

### FAZA 3: Pierwsze skanowanie (dzień 2-3)

#### 1. Tryb skanowania
- Włącz skaner
- Przycisk: **SCAN** lub **SEARCH**
- Skaner przeskakuje kanały

**Zachowanie:**
- Gdy coś nadaje → **zatrzyma się**
- Po zakończeniu rozmowy (2-5 sek ciszy) → **skanuje dalej**

#### 2. Obserwuj co znajdujesz
Notuj:
```
=== Dziennik skanowania ===
Data: __________
Lokalizacja: __________

| Czas | Częstotliwość | Co słyszałem | Siła |
|------|---------------|--------------|------|
| 14:23 | 118.1 MHz | Katowice Tower | S8 |
| 14:45 | 446.0 MHz | Rodzina na spacerze | S5 |
| 15:10 | 154.2 MHz | ? (nieznane) | S3 |
```

#### 3. Zapisz ciekawe kanały
Jeśli coś interesującego:
- **HOLD** / **PAUSE** - zatrzymaj skanowanie
- **SAVE** / **STORE** - zapisz do banku kanałów

---

### FAZA 4: Zaawansowane funkcje (tydzień 1-2)

#### Close Call (Uniden)
**Co to:** Wykrywa **silne sygnały w pobliżu** automatycznie

**Jak użyć:**
1. Włącz Close Call
2. Gdy ktoś nadaje blisko (PMR, CB) → skaner się zatrzyma
3. Sprawdź częstotliwość, zapisz jeśli ciekawe

**Zastosowanie:**
- Szukanie lokalnej aktywności
- Znalezienie częstotliwości ochrony w centrum handlowym
- Polowanie na ukryte nadajniki

#### Lockout (blokada kanału)
**Co to:** Ignoruje nudne/głośne kanały

**Jak użyć:**
1. Podczas skanowania, gdy zatrzyma się na nudnym kanale
2. Przycisk: **LOCKOUT**
3. Skaner pominie ten kanał w przyszłości

#### Weather Alert (USA mainly)
Niektóre skanery (Whistler) mają alerty pogodowe dla USA.  
**W Polsce:** Nie działa (brak takiej usługi).

---

## 📱 Aplikacje mobilne jako "skaner"

### Nie masz budżetu na skaner? Użyj telefonu!

#### 1. SDR Touch (Android)
**Wymaga:** RTL-SDR + adapter USB OTG  
**Koszt:** App ~20 zł + RTL-SDR ~150 zł  
**Funkcje:** Pełny SDR w telefonie!

#### 2. Scanner Radio (Android/iOS)
**Nie wymaga sprzętu!**  
**Koszt:** Darmowe (z reklamami)  
**Funkcje:** Streamuje skanery z całego świata przez Internet

**Jak działa:**
- Ludzie udostępniają swoje skanery online (Broadcastify)
- Ty słuchasz przez aplikację
- Możesz słuchać: Nowy Jork, Londyn, Tokyo!

**Wady:**
- ❌ Nie jest "prawdziwe" radio (potrzeba Internetu)
- ❌ Opóźnienie 10-30 sekund
- ⚠️ Nie wszystkie miasta dostępne

**Zalety:**
✅ Darmowe / tanie  
✅ Ogromny wybór  
✅ Zero hardware'u

---

## 🚗 Skaner w samochodzie - setup

### Co potrzebujesz:
1. **Skaner** z gniazdem 12V (lub adapter)
2. **Antena magnetyczna** VHF/UHF
3. **Uchwyt** do deski rozdzielczej
4. **Kabel zasilania** 12V (zapalniczka)

### Instalacja:
1. **Antena na dachu** - magnes trzyma
2. **Przewód przez okno** lub dziurę (nie przytrzaskuj!)
3. **Skaner na uchwycie** przy desce
4. **Zasilanie z zapalniczki**

### Programowanie do auta:
**Zapisz częstotliwości tras, którymi jeździsz:**
- Katowice → Kraków: 118.1, 120.9 (lotniska po drodze)
- PMR kanały 1-8 (popularne na trasach)
- Lokalne służby

**Tryb:** Priority Scan (skanuje, ale priorytet dla ważnych kanałów)

### Bezpieczeństwo:
- ❌ Nie słuchaj zbyt głośno (musisz słyszeć sygnały drogowe!)
- ❌ Nie programuj podczas jazdy
- ✅ Ustaw wszystko przed wyjazdem

---

## 💡 Wskazówki profesjonalisty

### 1. Antena to 80% sukcesu
Fabryczna antena "gumowa" jest OK, ale:
- **Lepsza opcja:** Nagoya NA-771 (~50 zł)
- **Najlepsza:** Antena zewnętrzna (discone, magnet)

### 2. Lokalizacja ma znaczenie
- **W domu:** Przy oknie, najwyżej jak można
- **W aucie:** Antena na dachu (nie w bagażniku!)
- **W terenie:** Na wzniesieniu, antena pionowo

### 3. Notuj wszystko
Po tygodniu zapomnisz co było na 154.235 MHz.  
**Używaj apps:**
- **Scanner Master** (iOS)
- **RadioLog** (Android)

### 4. Dołącz do społeczności
- **Radioreference.com** - forum
- **Grupa FB:** "Skanery i nasłuchy radiowe PL"
- Lokalny klub radioamatorów

### 5. Legalność i etyka
**Legalne:**
✅ Słuchanie prawie wszystkiego  
✅ Notowanie częstotliwości  
✅ Hobby i edukacja

**Nielegalne/nieetyczne:**
❌ Używanie informacji do przestępstw  
❌ Publikowanie rozmów (prywatność!)  
❌ Ingerencja w służby (próba rozmowy)  
❌ Nagrywanie i sprzedaż

---

## 🎯 Projekt: 30 dni ze skanerem

### Tydzień 1: Podstawy
- [ ] Dzień 1-2: Zaprogramuj 20 kanałów lokalnych
- [ ] Dzień 3-4: Testuj różne tryby skanowania
- [ ] Dzień 5-7: Notuj co znajdujesz

### Tydzień 2: Lotnictwo
- [ ] Znajdź częstotliwości najbliższego lotniska
- [ ] Słuchaj codziennie 30 min
- [ ] Naucz się podstawowych zwrotów (clearance, roger, etc.)

### Tydzień 3: PMR i lokalne
- [ ] Skanuj PMR 446 MHz (8 kanałów)
- [ ] Eksperymentuj z Close Call
- [ ] Znajdź ciekawe lokalne częstotliwości

### Tydzień 4: Mobilność
- [ ] Zabierz skaner do auta/na spacer
- [ ] Testuj zasięg w różnych miejscach
- [ ] Optymalizuj listę kanałów

**Efekt:** Po miesiącu znasz swój teren "radiowy" jak własną kieszeń!

---

## 📊 Skaner vs inne opcje - ostateczna decyzja

### Wybierz SKANER jeśli:
- ✅ VHF/UHF (lotnictwo, PMR, służby) - to Twoje pasmo
- ✅ Chcesz przenośności bez laptopa
- ✅ Lubisz "polowanie" na aktywne sygnały
- ✅ Budżet 400-800 zł

### Wybierz ATS MINI jeśli:
- ✅ Interesują Cię fale krótkie (HF/SW)
- ✅ Chcesz kompaktowe radio (plecak ewakuacyjny)
- ✅ Budżet do 200 zł
- ✅ Nie potrzebujesz auto-skanowania

### Wybierz RTL-SDR jeśli:
- ✅ Chcesz WSZYSTKIEGO (dekodowanie, ADS-B, satelity)
- ✅ Nie przeszkadza Ci laptop
- ✅ Chcesz wizualizacji (waterfall)
- ✅ Jesteś geek'iem / programistą

### Idealny setup (800-1000 zł):
**ATS Mini** (150 zł) - HF/SW/FM  
**RTL-SDR** (150 zł) - VHF/UHF, ADS-B, dekodowanie  
**Skaner Baofeng UV-5R** (100 zł) - mobilny backup + PMR nadawanie

**= Pokrywasz 0.5-1766 MHz + mobilność!**

---

## 📚 Co dalej?

1. ✅ Przeczytałeś: `05-skanery-radiowe.md`
2. ➡️ **NASTĘPNIE:**
   - `06-adsb-sledzenie-samolotow.md` - jeśli interesuje Cię lotnictwo
   - `07-czestotliwosci-co-sluchac.md` - szczegółowa lista częstotliwości

---

**Skaner to Twoje "ucho" na miasto. Słuchaj, ucz się, ciesz się!** 📻🚁

*Pamiętaj: Skanowanie to maraton, nie sprint. Po miesiącu znasz każdy dźwięk w eterze.*