# Słownik Pojęć Radiotechnicznych

## 📖 Jak korzystać ze słownika?

Pojęcia są posortowane **alfabetycznie** i oznaczone poziomem:
- 🟢 **Podstawowe** - musisz znać od razu
- 🟡 **Średniozaawansowane** - poznasz po miesiącu
- 🔴 **Zaawansowane** - dla geek'ów

---

## A

### 🟢 AM (Amplitude Modulation)
**Modulacja amplitudy** - sposób kodowania dźwięku w fali radiowej.

**Jak działa:** Zmienia się **wysokość** fali (amplituda)  
**Gdzie używane:** Fale średnie (MW), fale krótkie (SW), lotnictwo  
**Analogia:** Mówisz głośniej i ciszej - tak AM "pakuje" dźwiek

**Zalety:** Prosty system, daleki zasięg  
**Wady:** Podatny na zakłócenia (burze)

---

### 🟢 Antena
Urządzenie **łapiące** fale radiowe (odbiornik) lub **wysyłające** (nadajnik).

**Analogia:** Żagiel na łódce - łapie "wiatr radiowy"  
**Złota zasada:** Lepsza antena = 10x większy efekt niż droższe radio!

---

### 🟡 APRS (Automatic Packet Reporting System)
System przesyłania pozycji GPS przez radio (radioamatorzy).

**Częstotliwość:** 144.800 MHz (Europa)  
**Zastosowanie:** Śledzenie pozycji samochodów, osób w terenie

---

### 🔴 ATIS (Automatic Terminal Information Service)
Automatyczna transmisja informacji o pogodzie i warunkach na lotnisku.

**Przykład:** "Katowice ATIS information Delta, wind 270 at 10..."  
**Częstotliwości:** Różne dla każdego lotniska (np. 133.580 MHz Katowice)

---

### 🟢 Attenuator
Urządzenie **osłabiające** sygnał.

**Kiedy używać:** Gdy sygnał za mocny (przeciążenie odbiornika)  
**W praktyce:** Funkcja w SDR/radioach - zmniejsza Gain

---

## B

### 🟢 Bandwidth (BW) / Szerokość pasma
Określa **jak szeroki "kawałek"** częstotliwości radio słucha.

**Jednostka:** Hz, kHz  
**Analogia:** Szerokość rury - wąska = precyzyjna, szeroka = więcej przepływa

**Typowe wartości:**
- FM: 200 kHz (szerokie)
- AM: 6-10 kHz (średnie)
- SSB: 2-3 kHz (wąskie)
- CW (Morse): 0.5-1 kHz (bardzo wąskie)

**Kiedy wąskie:** Słaby sygnał, dużo szumów  
**Kiedy szerokie:** Mocny sygnał, lepsza jakość

---

### 🟡 BNC
Typ złącza antenowego (bajonetowe, szybkie).

**Wygląd:** Okrągłe, przekręcasz 1/4 obrotu  
**Gdzie używane:** Skanery, sprzęt profesjonalny  
**Twoje radio:** ATS Mini ma 3.5mm jack, potrzebujesz przejściówki!

---

### 🟡 Broadcast
Transmisja **dla ogółu** (np. radio FM, stacje SW).

**Przeciwieństwo:** Komunikacja punkt-punkt (radioamatorzy)

---

## C

### 🟡 CB (Citizen Band)
Pasmo radiowe dla obywateli (bez licencji).

**Częstotliwość:** 27 MHz (11m)  
**Moc:** Do 4W (Europa)  
**Kto używa:** Kierowcy TIR, starsi hobbyści  
**Tryb:** AM lub FM

---

### 🟡 CQ
Wywołanie ogólne w radiu.

**Znaczenie:** "Calling any station" (wołam dowolną stację)  
**Jak brzmi:** "CQ CQ CQ, this is SP5XYZ, calling CQ and standing by"

**Gdzie słuchać:** Pasma radioamatorskie (7, 14, 21 MHz)

---

### 🔴 CW (Continuous Wave)
**Kod Morse'a** - najstarsza forma łączności radiowej.

**Brzmienie:** Di-di-dit, daaaah  
**Gdzie:** Dolne części pasm radioamatorskich  
**Zaleta:** Działa przy ekstremalnie słabych sygnałach

---

## D

### 🟡 DCS (Digital Coded Squelch)
Cyfrowy kod wyciszania w PMR/CB.

**Jak działa:** Radio otwiera się tylko gdy słyszy właściwy kod  
**Zastosowanie:** Filtrowanie niechcianych rozmów  
**Uwaga:** Nie szyfruje, tylko filtruje!

---

### 🟡 Dipol
Typ anteny (dwa ramiona wychodzące z centrum).

**Wygląd:** Forma V lub linia prosta  
**Długość:** ~1/2 długości fali  
**Gdzie:** Zestawy RTL-SDR, anteny VHF/UHF

---

### 🟢 DSP (Digital Signal Processing)
Cyfrowe przetwarzanie sygnału.

**Co robi:** Przetwarza sygnał analogowy (fala radiowa) na cyfrowy (komputer)  
**Twoje radio:** ATS Mini ma chip DSP (SI4732)  
**Zaleta:** Lepsze filtry, mniej szumów niż analogowo

---

### 🟡 DX (Distance)
Daleki kontakt radiowy.

**Przykład:** Złapanie stacji z Australii z Polski = DX!  
**DX hunting:** Polowanie na dalekie stacje  
**DXpedition:** Wyjazd do rzadkiego kraju żeby nadawać

---

## E

### 🟡 EME (Earth-Moon-Earth)
Łączność przez **odbicie od Księżyca**!

**Jak działa:** Nadajesz w stronę Księżyca, fala odbija się i wraca  
**Kto używa:** Radioamatorzy z potężnymi antenami  
**Zaawansowanie:** 🔴🔴🔴 (dla hardcore geek'ów)

---

## F

### 🟢 FM (Frequency Modulation)
**Modulacja częstotliwości** - sposób kodowania dźwięku.

**Jak działa:** Zmienia się **częstotliwość** fali (nie amplituda jak w AM)  
**Gdzie:** Radio FM (87.5-108 MHz), PMR (446 MHz)  
**Zalety:** Odporny na zakłócenia, lepsza jakość  
**Wady:** Krótszy zasięg niż AM

---

### 🟡 FT8
Cyfrowy tryb łączności (bardzo wydajny przy słabych sygnałach).

**Brzmienie:** Jak modem dialup  
**Gdzie:** 7.074, 14.074, 21.074 MHz  
**Software:** WSJT-X  
**Popularne:** Bo działa gdy SSB już nie słychać!

---

## G

### 🟢 Gain (wzmocnienie)
Parametr określający **jak mocno** wzmacniamy sygnał.

**Jednostka:** dB (decybele)  
**Analogia:** Głośność na wzmacniaczu

**Typowe wartości:**
- 0-10 dB = niskie (dla silnych sygnałów)
- 20-30 dB = średnie (normalnie)
- 40-50 dB = wysokie (dla słabych sygnałów)

**Uwaga:** Za dużo gain = szumy i przeciążenie!

---

### 🟡 Ground plane
Płaszczyzna uziemiająca dla anteny.

**Przykład:** Dach samochodu dla anteny magnetycznej  
**Dlaczego ważne:** Antena + ground plane = lepszy odbiór  
**DIY:** Dla długich drutów - uziemienie zwiększa efektywność

---

## H

### 🟢 HF (High Frequency)
Fale krótkie, **3-30 MHz**.

**Inne nazwy:** SW (Short Wave)  
**Specjalność:** Globalny zasięg (odbicie od jonosfery)  
**Co słuchać:** Stacje międzynarodowe, radioamatorzy  
**Twoje radio:** ATS Mini - świetne na HF!

---

### 🟡 Ham Radio
Potoczna nazwa na **radio amatorskie**.

**Pochodzenie:** Niejasne (może od "ham-fisted" = niezdarny)  
**Wymaga:** Licencja (egzamin)  
**Pasma:** Wiele zakresów w HF, VHF, UHF

---

## I

### 🟡 ILS (Instrument Landing System)
System precyzyjnego lądowania na lotnisku.

**Częstotliwości:** 108-112 MHz  
**Jak działa:** Samolot "leci po promieniu" do pasa  
**Słyszalne:** Można słuchać rozmów pilotów ("established ILS")

---

### 🟡 Ionosphere (jonosfera)
Warstwa atmosfery, **odbija fale radiowe**.

**Wysokość:** 60-1000 km  
**Dlaczego ważna:** Dzięki niej HF ma globalny zasięg!  
**Zmienia się:** Dzień/noc, pora roku, cykl słoneczny

**Analogia:** Jak basen - fale HF odbijają się od "sufitu" (jonosfery) i wracają na Ziemię daleko

---

### 🟢 ISS (International Space Station)
Międzynarodowa Stacja Kosmiczna.

**Częstotliwości:**
- 145.800 MHz - FM voice (czasem astronauci gadają!)
- 437.550 MHz - SSTV (zdjęcia)

**Jak słuchać:** Sprawdź przelot (heavens-above.com), nastaw częstotliwość

---

## J

### 🟡 Jitter
Niestabilność sygnału (drgania częstotliwości).

**Objaw:** Sygnał "pływa", trzeba ciągle dostrajać  
**Przyczyna:** Słaby sygnał, zakłócenia, zła antena

---

## K

### 🟢 kHz (kiloherc)
Jednostka częstotliwości = 1000 Hz.

**Przykład:** 225 kHz = 225 000 Hz  
**Gdzie używane:** LW, MW, dolne HF

---

## L

### 🟡 LNA (Low Noise Amplifier)
Wzmacniacz małoszumny.

**Co robi:** Wzmacnia **bardzo słabe** sygnały bez dodawania szumów  
**Gdzie:** FlightAware Pro Stick Plus, profesjonalne anteny aktywne  
**Efekt:** +50-100 km zasięgu dla ADS-B!

---

### 🟢 LSB (Lower Side Band)
Dolna wstęga boczna (rodzaj SSB).

**Gdzie używane:** Pasma HF poniżej 10 MHz  
**Przykład:** 7.100-7.200 MHz (40m) - radioamatorzy w Europie  
**Tryb:** Na ATS Mini wybierasz "LSB"

---

### 🟢 LW (Long Wave)
Fale długie, **30-300 kHz**.

**Polskie Radio:** 225 kHz - **stacja awaryjna!**  
**Zasięg:** Tysiące km  
**Charakterystyka:** Słabe, szumią, ale działają zawsze

---

## M

### 🟢 MHz (megaherc)
Jednostka częstotliwości = 1 000 000 Hz.

**Przykład:** 88.6 MHz = 88 600 000 Hz  
**Gdzie:** FM (87.5-108 MHz), VHF, UHF

---

### 🟢 MW (Medium Wave)
Fale średnie, **300 kHz - 3 MHz**.

**Inne nazwy:** AM band  
**Przykład:** Radio Maryja 1602 kHz  
**Zasięg:** Nocą lepszy (odbicie od jonosfery)

---

### 🟡 Mode S
Zaawansowany tryb transpondera samolotów (ADS-B używa Mode S).

**Co przesyła:** ICAO kod, pozycja, prędkość, wysokość  
**Częstotliwość:** 1090 MHz

---

## N

### 🟡 NFM (Narrow FM)
Wąskie FM.

**Szerokość:** ~12.5 kHz  
**Gdzie:** PMR (446 MHz), niektóre służby  
**Różnica vs WFM:** Gorsze audio, ale mniejsze pasmo (więcej kanałów)

---

### 🟡 NOAA
Satelity pogodowe USA.

**Częstotliwości:**
- 137.100 MHz (NOAA 15)
- 137.620 MHz (NOAA 18)
- 137.912 MHz (NOAA 19)

**Co odbierasz:** Zdjęcie Ziemi z kosmosu (dekodowane w WXtoImg)

---

## O

### 🟡 Offset
Przesunięcie częstotliwości.

**Gdzie:** Repeatery (przemienniki)  
**Przykład:** Nadajesz 145.000 MHz, przemiennik retransmituje 145.600 MHz (+600 kHz offset)

---

### 🟡 Overload
Przeciążenie odbiornika (sygnał za mocny).

**Objaw:** Szumy, zniekształcenia, "wszystko słychać"  
**Rozwiązanie:** Zmniejsz Gain, dodaj attenuator

---

## P

### 🟢 PMR (Personal Mobile Radio)
Pasmo wolne (bez licencji) na 446 MHz.

**Kanały:** 8 (446.00625 - 446.09375 MHz)  
**Moc:** Max 0.5W  
**Kto używa:** Rodziny, ochrona, budowy, hobby

---

### 🟡 Propagacja
Rozprzestrzenianie się fal radiowych.

**Rodzaje:**
- **Ground wave** - wzdłuż ziemi (LW, MW)
- **Sky wave** - odbicie od jonosfery (HF)
- **Line of sight** - w linii prostej (VHF, UHF)

**Warunki:** Pogoda, pora dnia, cykl słoneczny wpływają na propagację

---

### 🟡 PTT (Push To Talk)
Przycisk "nadawaj".

**Jak działa:** Przytrzymujesz = mówisz, puszczasz = słuchasz  
**Gdzie:** Krótkofalówki PMR, radioamatorzy

---

## Q

### 🟡 QRM
Zakłócenia od innych stacji.

**Przykład:** "Mam dużo QRM na 14200 kHz" = jest dużo innych nadajników, trudno słuchać

---

### 🟡 QSL Card
Pocztówka potwierdzająca odbiór stacji.

**Jak działa:** Słuchasz stację → wysyłasz raport → dostaniesz pocztówkę  
**Kolekcjonerstwo:** Zbieranie QSL z różnych krajów

---

### 🟡 QSO
Kontakt radiowy (rozmowa).

**Przykład:** "Miałem QSO z USA" = rozmawiałem z operatorem z USA

---

## R

### 🟡 Repeater (Przemiennik)
Stacja automatycznie retransmitująca sygnał.

**Jak działa:** Odbiera na jednej częstotliwości, nadaje na innej  
**Cel:** Zwiększenie zasięgu  
**Gdzie:** Pasma amatorskie VHF/UHF, PMR (nie w Polsce standardowo)

---

### 🟢 RKO (Resuscytacja Krążeniowo-Oddechowa)
**Uwaga:** To nie jest termin radiowy! Ale jest w Twoich dokumentach pierwszej pomocy.

30 uciśnięć klatki + 2 oddechy, wezwij 112!

---

### 🟢 RTL-SDR
Typ odbiornika SDR (najtańszy i najpopularniejszy).

**Chip:** RTL2832U + R820T2  
**Zakres:** 24-1766 MHz  
**Cena:** ~100-150 zł  
**Wymaga:** Komputer + oprogramowanie

---

## S

### 🟢 S-meter
Wskaźnik siły sygnału.

**Skala:** S1 - S9 (+ dodatkowe dB)  
**Interpretacja:**
- S1-S3 = słaby (szumi)
- S5-S7 = dobry
- S9 = bardzo mocny
- S9+20dB = ekstremalnie mocny

---

### 🟡 SDR (Software Defined Radio)
Radio programowalne (magia dzieje się w software).

**Różnica vs tradycyjne:** Elektronika minimalna, wszystko w komputerze  
**Zalety:** Elastyczność, wizualizacja (waterfall), tanie

---

### 🟡 Simplex
Komunikacja bezpośrednia (obie stacje na tej samej częstotliwości).

**Przeciwieństwo:** Duplex (repeater - różne częstotliwości)

---

### 🟡 SINPO
Kod jakości sygnału (używany w raportach).

**Oznaczenia:**
- **S**ignal strength (siła sygnału) - 1-5
- **I**nterference (zakłócenia) - 1-5
- **N**oise (szum) - 1-5
- **P**ropagation (propagacja/fading) - 1-5
- **O**verall (ogólna ocena) - 1-5

**Przykład:** SINPO 55555 = perfekcyjny odbiór

---

### 🟡 SMA
Typ złącza antenowego (małe, gwintowane).

**Wygląd:** Małe, nakręcasz  
**Gdzie:** RTL-SDR, anteny aktywne, nowoczesny sprzęt

---

### 🟢 Squelch
Wyciszanie szumów (radio milczy gdy brak sygnału).

**Jak działa:** Ustaw poziom → radio otwiera się tylko gdy sygnał mocniejszy  
**Ustawienia:** 0 = wyłączone (słychać wszystko), 9 = bardzo wysoki próg

**Kiedy zmniejszyć:** Gdy nie słychać słabych stacji  
**Kiedy zwiększyć:** Gdy męczy Cię ciągły szum

---

### 🟢 SSB (Single Side Band)
Zaawansowany tryb AM (tylko jedna wstęga boczna).

**Typy:** USB (górna), LSB (dolna)  
**Gdzie:** Radioamatorzy HF  
**Zalety:** Lepsza jakość, mniejsze pasmo, dalszy zasięg  
**Wady:** Trzeba precyzyjnie dostroić (brzmi jak "kaczor Donald" gdy źle)

---

### 🟢 SW (Short Wave)
Fale krótkie = HF (3-30 MHz).

**Specjalność:** Globalny zasięg!  
**Twoje radio:** ATS Mini - mocna strona

---

## T

### 🟡 TETRA
Cyfrowy system łączności (służby w Polsce).

**Szyfrowanie:** Tak, nie posłuchasz  
**Kto używa:** Policja, straż, pogotowie (w dużych miastach)

---

### 🟡 Transceiver
Radio 2-kierunkowe (odbiera I nadaje).

**Przykład:** Baofeng UV-5R, radioamatorskie  
**Przeciwieństwo:** Receiver (tylko odbiera, jak ATS Mini)

---

### 🟡 Troposcatter
Odbicie fal od troposfery.

**Zasięg:** Ponad horyzont (VHF/UHF)  
**Kiedy:** Specjalne warunki atmosferyczne  
**Efekt:** Nagle słychać stacje 300-500 km dalej!

---

## U

### 🟢 UHF (Ultra High Frequency)
Fale ultra krótkie, **300 MHz - 3 GHz**.

**Przykłady:**
- PMR: 446 MHz
- ADS-B: 1090 MHz
- WiFi: 2.4 GHz

**Charakterystyka:** Krótki zasięg (linia wzroku), dużo informacji

---

### 🟡 USB (Upper Side Band)
Górna wstęga boczna (rodzaj SSB).

**Gdzie:** Pasma HF powyżej 10 MHz  
**Przykład:** 14.150-14.300 MHz (20m) - radioamatorzy

---

### 🟡 UTC (Universal Time Coordinated)
Czas uniwersalny (Greenwich).

**Dlaczego używamy:** Radioamatorzy z całego świata - wspólny czas  
**Polska:** UTC +1 (zimą), UTC +2 (latem)  
**Przykład:** 20:00 w Polsce = 19:00 UTC (zimą)

---

## V

### 🟢 VHF (Very High Frequency)
Fale bardzo krótkie, **30-300 MHz**.

**Przykłady:**
- FM radio: 87.5-108 MHz
- Lotnictwo: 118-137 MHz
- Radioamatorzy 2m: 144-146 MHz

**Charakterystyka:** Zasięg 50-100 km (linia wzroku)

---

### 🟡 VOX (Voice Operated Transmit)
Automatyczne nadawanie po wykryciu głosu.

**Jak działa:** Zaczniesz mówić → radio automatycznie nadaje  
**Gdzie:** Krótkofalówki PMR  
**Wady:** Czasem włącza się od szumów

---

## W

### 🟡 Waterfall
Wizualizacja widma częstotliwości (w SDR).

**Wygląd:** Kolorowa "kaskada"  
**Osie:**
- X = częstotliwość
- Y = czas (przeszłość na górze)
- Kolor = siła sygnału

**Dlaczego przydatne:** Widzisz gdzie są sygnały zanim usłyszysz!

---

### 🟡 WFM (Wideband FM)
Szerokie FM.

**Szerokość:** ~200 kHz  
**Gdzie:** Radio FM (87.5-108 MHz)  
**Różnica vs NFM:** Lepsza jakość audio, więcej pasma

---

## X

### 🟡 XIT (Transmit Incremental Tuning)
Przesunięcie częstotliwości nadawania.

**Dla kogo:** Zaawansowani radioamatorzy  
**Nie dotyczy:** Odbiornik (jak ATS Mini)

---

## Z

### 🟡 Zulu Time
Potoczna nazwa na UTC (czas uniwersalny).

**Pochodzenie:** Alfabet fonetyczny (Z = Zulu = UTC)  
**Użycie:** Lotnictwo, wojsko, radioamatorzy

---

## 🎯 Szybkie odniesienia

### Jednostki:
- **Hz** = herc (1 cykl/sekundę)
- **kHz** = kiloherc (1000 Hz)
- **MHz** = megaherc (1 000 000 Hz)
- **GHz** = gigaherc (1 000 000 000 Hz)

### Pasma (uproszczone):
- **LW** = 30-300 kHz
- **MW** = 300 kHz - 3 MHz
- **HF/SW** = 3-30 MHz
- **VHF** = 30-300 MHz
- **UHF** = 300 MHz - 3 GHz

### Tryby:
- **AM** = Amplitude Modulation
- **FM** = Frequency Modulation
- **SSB** = Single Side Band (USB/LSB)
- **CW** = Morse code

---

## 📚 To już koniec poradników!

Gratulacje - przeczytałeś wszystkie 8 plików! 🎉

**Masz teraz:**
1. ✅ Podstawy radiotechniki
2. ✅ Znajomość ATS Mini
3. ✅ Wiedzę o antenach
4. ✅ Plan nauki 12 tygodni
5. ✅ Informacje o SDR
6. ✅ Przewodnik po skanerach
7. ✅ Projekt ADS-B
8. ✅ Listę częstotliwości
9. ✅ Słownik pojęć

**Co teraz?**
- Wróć do `03-plan-nauki-krok-po-kroku.md` i zacznij tydzień 1!
- Drukuj to co potrzebne
- Rób notatki w dzienniku nasłuchowym
- Eksperymentuj!

---

**Powodzenia w przygodzie z radiem! 📻✨**

*"Każdy ekspert był kiedyś początkującym. Różnica? Ekspert nie przestał eksperymentować."*