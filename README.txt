KARTOVNÍK 2.0 – VĚRNOSTNÍ KARTY
=================================

CO JE NOVÉ
- 31 předpřipravených obchodů s grafickými štítky v designu značky
  (Tesco, Lidl, Kaufland, Albert, Billa, Penny, dm, Rossmann a další).
- Výběr obchodu naplní jméno, kategorii a obrázek.
- Vlastní fotografie / obrázek ke každé kartě (zmenší se před uložením).
- Načítání čárového nebo QR kódu fotoaparátem.
- Náhradní načtení kódu z fotografie.
- Nově i kódy Code 39 a UPC-A; nadále Code 128, EAN-13, EAN-8, QR.
- Export/import záloh zahrnuje i obrázky.
- Staré karty z Kartovníku 1.0 zůstanou v prohlížeči zachovány.

JAK NAHRÁT NA GITHUB
1. Rozbal ZIP a nahraj všech 5 souborů do kořenové složky repozitáře:
   index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png.
2. V GitHubu nastav Settings > Pages > Deploy from branch > main > /(root).
3. Otevři adresu GitHub Pages na iPhonu přes Safari.
4. Sdílet > Přidat na plochu. Ikona se zobrazí mezi aplikacemi.

JAK NAČÍST KARTU KAMEROU
1. Přidat > vybrat obchod > Skenovat fotoaparátem.
2. Povol přístup ke kameře; namiř kód do výřezu.
3. Pokud kamera nepůjde, použij Načíst kód z fotky nebo zadej číslo ručně.
4. Po rozpoznání zkontroluj typ a číslo kódu, potom ulož.

DŮLEŽITÉ
- Kamera funguje pouze přes HTTPS (např. GitHub Pages) nebo localhost,
  nikoli při otevření souboru index.html z disku.
- Pro skenování se při prvním spuštění načte knihovna html5-qrcode 2.3.8
  ze sítě CDN. Bez připojení proto může být skenování nedostupné;
  uložené karty a jejich čárové/QR kódy fungují offline.
- Skenování na skutečném iPhonu nelze automatickým testem ověřit.
  Webová knihovna uvádí podporu Safari pro iOS 15.1+.
- Podporované snímané typy: QR, Code 128, EAN-13, EAN-8, UPC-A, Code 39.
- Grafické štítky jsou místní stylizované reprezentace značek,
  nejde o oficiální loga, aplikace ani partnerství s obchodníky.
- Vlastní fotografie mohou rychle zaplnit úložiště Safari; pravidelně
  si stáhni zálohu JSON. Data jsou pouze na konkrétním zařízení.
- Při přenosu na nový telefon použij Nastavení > Záloha a obnovení.
- Není potřeba žádný účet, server ani databáze.

KNIHOVNA SKENOVÁNÍ
html5-qrcode 2.3.8, Apache-2.0, https://github.com/mebjas/html5-qrcode
Načítá se při prvním použití z jsDelivr CDN.
