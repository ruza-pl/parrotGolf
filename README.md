# parrotGolf v.0.1
Sterowanie systemem głośnomówiącym Parrot Ck3000 Evolution za pomocą kierowicy multifunkcyjnej w VW Golf MK6

Sterowanie polega na odebraniu wiadomości CAN z informacją nt. użytego przycisku i przesłaniu tego do CK3000. 

Kody Can do wykorzystania: 

0x5C1 to ID ktorego szukamy, obslugujace klawisze na kierownicy
Wiadomosc zbudowana jest w taki sposob: 
<code>
5C1  XX 00 00 60  <br>
     00  Puszczone klawisze <br>
    Lewa strona <br>
     02  Następny     > <br>
     03  Poprzedni    < <br>
     06  Głośność +   + <br>
     07  Głośność -   - <br>
     1A  Telefon      ✆ <br>
     0A  Menu <br>
     22  Do góry <br>
     23  Do dołu <br>
     28  OK <br>
     2B  Wycisz (wybieranie glosowe) <br>
     09  MFD Poprzedni ekran <br>
     0A  MFD Nastepny ekran <br>
     29  Wstecz <br>
</code>
