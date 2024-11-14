Oto prosty przykład programu napisanego w CLLE (Command Language for ILE) na platformę IBM i (dawniej AS/400). Program ten jest zapisem CLLE, który wyświetla komunikat na ekranie użytkownika.


### Opis działania:
1. **PGM** - Deklaracja początku programu.
2. **DCL VAR(&MSG) TYPE(*CHAR) LEN(50)** - Definicja zmiennej `&MSG` o długości 50 znaków, która przechowa komunikat do wyświetlenia.
3. **CHGVAR VAR(&MSG) VALUE('Witaj w świecie IBM i!')** - Ustawienie wartości zmiennej `&MSG` na tekst, który chcemy wyświetlić.
4. **SNDPGMMSG MSG(&MSG) MSGTYPE(*INFO)** - Polecenie wyświetlenia zawartości zmiennej `&MSG` jako wiadomości informacyjnej.
5. **ENDPGM** - Zakończenie programu.

### Uruchomienie programu:
1. Zapisać kod do pliku źródłowego (np. `MSGTESTCL` w bibliotece źródłowej).
2. Skompilować kod jako program CLLE (polecenie `CRTBNDCL PGM(MYLIB/MSGTESTCL) SRCFILE(MYLIB/QCLSRC) SRCMBR(MSGTESTCL)`).
3. Uruchomić program poleceniem `CALL PGM(MYLIB/MSGTESTCL)`.

To prosty przykład, który można rozszerzyć o bardziej zaawansowane funkcjonalności IBM i oraz programowania w CLLE.