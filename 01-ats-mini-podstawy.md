# ATS Mini SI4732 - Kompletny Przewodnik

## 📻 Co to jest ATS Mini?

ATS Mini to **kieszonkowy odbiornik radiowy wielopasm**, który zmieści Ci się w kieszeni, ale potrafi słuchać stacji z całego świata.

### Analogia
To jak **szwajcarski scyzoryk** w świecie radia - mały, lekki, ale ma wszystko co potrzeba:
- Radio FM (lokalne stacje)
- Fale średnie AM/MW (radio regionalne)
- Fale krótkie SW (świat!)
- Tryby specjalne LSB/USB (radioamatorzy)

---

## 🔧 Specyfikacja techniczna (uproszczona)

| Parametr | Wartość | Co to znaczy? |
|----------|---------|---------------|
| **Zakres częstotliwości** | 0.5 - 108 MHz | Od LW do FM - prawie wszystko! |
| **Chip DSP** | SI4732 | Mózg radia - przetwarza sygnały cyfrowo |
| **Ekran** | 1.9" IPS kolorowy | Wyświetlacz jak w smartfonie (320x170 px) |
| **Bateria** | 800 mAh | ~10 godzin słuchania |
| **Ładowanie** | USB Type-C | Jak telefon |
| **Gniazdo słuchawkowe** | 3.5mm (jack) | Standardowe słuchawki |
| **Gniazdo anteny** | 3.5mm (jack) | WAŻNE - to samo co słuchawki! |
| **Waga** | ~50-70g | Jak średnia czekolada |
| **Wymiary** | 73x32x12 mm | Mniejsze niż telefon |

---

## 📡 Czego ATS Mini NIE ma (ważne!)

### ❌ BNC/SMA - standardowe złącza antenowe
Zamiast tego ma **3.5mm jack** (jak słuchawki). Dlatego potrzebujesz **przejściówek** do lepszych anten.

### ❌ Pasm bardzo wysokich (powyżej 108 MHz)
Nie odbierze:
- PMR (446 MHz)
- ADS-B samoloty (1090 MHz)
- Telefony komórkowe

**Rozwiązanie:** Dokup później RTL-SDR (~150 zł) dla tych pasm.

### ❌ Głośnika wbudowanego
Musisz używać **słuchawek** (albo dokupić głośniczek USB-C).

### ❌ Funkcji nadawania
To **tylko odbiornik** - nie nadajesz (ale to legalne i bezpieczne!).

---

## 🎯 W czym ATS Mini jest ŚWIETNY?

### ✅ Fale krótkie (HF/SW) - 3-30 MHz
**To jest jego supermoc!**

Możesz słuchać:
- BBC World Service (różne częstotliwości)
- Radio Havana Cuba (6000 kHz)
- China Radio International
- Voice of America
- Radioamatorzy ze świata

**Dlaczego to fajne?**  
W nocy, siedząc w domu w Mysłowicach, możesz słuchać stacji z **Australii, Japonii, Ameryki Południowej** - bez Internetu!

### ✅ AM/MW - 300 kHz - 3 MHz
Lokalne stacje AM, które w kryzysie nadają komunikaty.

### ✅ LW - 30-300 kHz
**Polskie Radio 225 kHz** - działa nawet jak cała reszta padnie. To Twoja najbardziej niezawodna stacja awaryjna!

### ✅ FM - 87.5-108 MHz
Normalne radio FM, jak w każdym radiu.

---

## 🚀 Pierwsze kroki z ATS Mini

### Krok 1: Rozpakowanie i ładowanie
1. Wyjmij radio z pudełka
2. Podłącz kabel USB-C
3. Ładuj 2-3 godziny (pierwsza ładowak)
4. Załącz antenę teleskopową (wkręć w gniazdo 3.5mm - to małe gniazdo oznaczone symbolem anteny)

**UWAGA:** Jest **DWIE dziurki 3.5mm**:
- Jedna to **słuchawki** (🎧)
- Druga to **antena** (📡)
Nie pomyl!

### Krok 2: Włączanie
1. Przytrzymaj przycisk Power (zwykle 2-3 sekundy)
2. Ekran się zapali
3. Domyślnie włączy się na FM

### Krok 3: Pierwsze słuchanie FM
1. Rozłóż antenę teleskopową **pionowo**
2. Włóż słuchawki (kabel słuchawkowy działa też jak antena!)
3. Przyciskami góra/dół szukaj stacji
4. **Mysłowice:** Spróbuj 88.6 FM (Polskie Radio Katowice)

**Udało się?** ✅ Gratulacje, słuchasz radia!

### Krok 4: Testowanie innych pasm

#### LW - Polskie Radio 225 kHz
1. Przycisk MENU lub MODE → wybierz **LW**
2. Ręcznie wpisz: **225** (lub użyj strojenia)
3. Słuchawki w uszach
4. Antena poziomo (fale długie lubią poziom)

**Co usłyszysz?**  
Słaby sygnał, trochę szumów, ale **powinno coś być**. To normalne dla LW.

#### MW - AM lokalnie
1. Przejdź do trybu **MW** lub **AM**
2. Spróbuj 1602 kHz (Radio Maryja - łatwe do znalezienia)
3. Wieczorem zasięg będzie lepszy!

#### SW - Świat!
1. Przejdź do trybu **SW** lub **HF**
2. Spróbuj takich częstotliwości:
   - **6000 kHz** - Radio Havana (wieczorem)
   - **7200-7300 kHz** - pasmo amatorskie 40m
   - **9400-9900 kHz** - stacje międzynarodowe
   - **15000-15800 kHz** - fale krótkie (dzień)

**Najlepszy czas:** Wieczór i noc (20:00-02:00)

---

## 🎛️ Podstawowe funkcje (przybliżone - może się różnić w zależności od firmware)

### Strojenie częstotliwości
- **Krok po kroku:** Przyciski ▲/▼
- **Szybkie:** Przytrzymaj ▲/▼
- **Ręczne wpisywanie:** Przycisk cyfrowy / FREQ

### Tryby pracy
- **FM** - radio FM (87.5-108 MHz)
- **AM** - fale średnie
- **LW** - fale długie
- **SW** - fale krótkie
- **LSB/USB** - Single Side Band (dla zaawansowanych)

### Szerokość pasma (BW - Bandwidth)
Określa jak "szeroki" kawałek częstotliwości radio słucha.

**Analogia:** To jak regulacja ostrości w aparacie:
- **Szerokie (6 kHz)** - lepszy dźwięk, ale więcej szumów
- **Wąskie (1 kHz)** - gorszy dźwięk, ale mniej szumów

**Kiedy używać?**
- **FM:** Zawsze szerokie
- **AM silny sygnał:** Szerokie (4-6 kHz)
- **AM słaby:** Wąskie (2-3 kHz)
- **SW zagraniczne:** Wąskie (1-2 kHz)

### Siła sygnału (S-meter)
Wskaźnik na ekranie pokazujący **jak mocny jest sygnał**.
- S1-S3 = słaby (szumi, trzeszczy)
- S5-S7 = dobry (słychać wyraźnie)
- S9+ = bardzo mocny (krystalicznie)

---

## 📝 Ćwiczenie praktyczne: Pierwszy dziennik nasłuchowy

**Cel:** Nauczyć się, co i kiedy można słuchać.

### Zadanie 1: Test lokalnych stacji FM (15 min)
1. Włącz FM
2. Przeskanuj 87.5 - 108 MHz
3. Zapisz w notesie:

```
Data: ___________
Godzina: _________
Pasmo: FM

| Częstotliwość | Nazwa stacji | Siła sygnału | Uwagi |
|---------------|--------------|--------------|-------|
| 88.6 MHz      | PR Katowice  | S9           | Bardzo mocna |
| 90.8 MHz      | Radio Zet    | S8           | Wyraźna |
| ...           | ...          | ...          | ...   |
```

### Zadanie 2: Test LW 225 kHz (10 min)
1. Przełącz na LW
2. Ustaw 225 kHz
3. Różne pozycje anteny:
   - Pionowo
   - Poziomo
   - Pod kątem 45°

**Który układ daje najlepszy odbiór?** _________________

### Zadanie 3: Polowanie na SW wieczorem (30 min)
Najlepiej: 20:00-22:00

Przeskanuj te zakresy:
- 6000-6200 kHz (49m band)
- 7100-7300 kHz (41m band)
- 9400-9900 kHz (31m band)

**Ile stacji znalazłeś?** _______

**Czy usłyszałeś coś w obcym języku?** _______

---

## 🔋 Zarządzanie baterią

### Jak wydłużyć czas pracy?
1. **Zmniejsz jasność ekranu** - Menu → Display → Brightness
2. **Wyłącz podświetlenie** - Auto-off 10 sekund
3. **Głośność 50-70%** - nie na full
4. **Wyłączaj gdy nie używasz** - nie zostawiaj w standby

### Ładowanie
- **Pierwsze ładowanie:** 3 godziny
- **Normalne:** 2 godziny
- **Używaj podczas ładowania:** Tak, można!

### Awaryjne zasilanie
Jeśli padnie bateria w terenie:
- **Powerbank** → kabel USB-C → ATS Mini
- Działa jak zwykłe ładowanie, możesz słuchać dalej

---

## 🎓 Zadania domowe dla początkujących

### Tydzień 1: Poznanie urządzenia
- [ ] Włącz i przeskanuj FM (znajdź 5 lokalnych stacji)
- [ ] Znajdź 225 kHz na LW (Polskie Radio)
- [ ] Wieczorem: Znajdź jedną stację na SW

### Tydzień 2: Eksperymenty
- [ ] Testuj różne pozycje anteny (pionowo, poziomo, na oknie)
- [ ] Porównaj odbiór dzień vs noc (ta sama częstotliwość SW)
- [ ] Zapisuj obserwacje: która godzina daje najlepszy odbiór?

### Tydzień 3: Zaawansowane
- [ ] Spróbuj LSB/USB na 7200 kHz (radioamatorzy)
- [ ] Znajdź 3 stacje zagraniczne na SW
- [ ] Eksperymentuj z szerokością pasma (BW)

---

## ⚙️ Ustawienia rekomendowane dla Mysłowic

### FM - stacje lokalne
- **Tryb:** FM
- **BW:** Auto lub 100 kHz
- **Antena:** Pionowo, pełna długość

### LW 225 kHz (awaria!)
- **Tryb:** LW
- **BW:** 2-3 kHz
- **Antena:** Poziomo lub pod kątem

### SW - nocne słuchanie
- **Tryb:** SW lub AM
- **BW:** 2-3 kHz (wąskie = mniej szumów)
- **Antena:** Najdłuższa możliwa, eksperymentuj z kierunkiem
- **Godzina:** 20:00-02:00 (najlepszy odbiór)

---

## 🐛 Najczęstsze problemy i rozwiązania

### Problem: Słaby sygnał na wszystkich pasmach
**Rozwiązanie:**
- Sprawdź czy antena jest podłączona do właściwej dziurki (📡 nie 🎧)
- Wypróbuj inne miejsce (od okna, balkon)
- Dla SW: Czekaj do wieczora

### Problem: Szumy, trzaski
**Rozwiązanie:**
- Odsuń się od komputera, ładowarek, lamp LED
- Zmniejsz BW (szerokość pasma)
- Dla FM: Zmień orientację anteny

### Problem: Nic nie słychać na SW
**Rozwiązanie:**
- **To normalne w dzień!** Fale krótkie najlepiej działają wieczorem i nocą
- Spróbuj wyższych częstotliwości (15-18 MHz) w dzień
- Niższe częstotliwości (6-9 MHz) w nocy

### Problem: Bateria szybko się rozładowuje
**Rozwiązanie:**
- Zmniejsz jasność ekranu
- Wyłącz auto-scan
- Może być zużyta bateria (po ~1-2 latach użytkowania)

---

## 📚 Co dalej?

1. ✅ Przeczytałeś: `01-ats-mini-podstawy.md`
2. ➡️ **NASTĘPNIE:** `02-anteny-przewodnik.md` - popraw odbiór!
3. `03-plan-nauki-krok-po-kroku.md` - systematyczna nauka

---

## 💡 Protip: Zapisuj wszystko!

**Stwórz dziennik nasłuchowy:**
```
=== Dziennik ATS Mini ===

Data: 15.10.2025
Godzina: 21:30
Lokalizacja: Mysłowice, balkon

Pasmo: SW
Częstotliwość: 7200 kHz
Tryb: USB
BW: 2.8 kHz
Sygnał: S7

Co słyszałem: Radioamatorzy, rozmowa po angielsku,
              operator z USA z Niemcami
Antena: Teleskopowa pionowo
Pogoda: Bezchmurnie

Uwagi: Lepszy odbiór niż wczoraj, chyba
       wpływ pogody?
```

**Dlaczego to ważne?**  
Za miesiąc zauważysz wzorce - które pasma, o której godzinie, w jakiej pogodzie działają najlepiej!

---

*Miłego słuchania! 📻*

*Następny krok: Lepsze anteny = lepszy odbiór!*