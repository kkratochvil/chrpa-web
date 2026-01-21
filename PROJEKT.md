# Web pro Chrpu Chrudim - Poznámky k projektu

## O projektu
Statický web pro trampskou skupinu **Chrpa Chrudim**, která funguje od roku 1974.

## Barvy (z loga/vlajky)
- Žlutá: `#FBB63A`
- Modrá: `#1E607A`

## Struktura webu
1. **Úvodní stránka (Hero)** - fotka kapely, nápis "Chrpa Chrudim" (písmo Great Vibes), logo dole
2. **O nás** - historie skupiny + 2 fotky (1977 a chrpa_odchod) + video box "Country rádio"
3. **Novinky** - stylizovaný odkaz na Facebook stránku (plugin nefungoval spolehlivě)
4. **Koncerty** - tabulka s nadcházejícími koncerty + sloupec "Zvadlo" pro letáky
5. **Písničky** - audio přehrávače (12 nahrávek) + vzpomínka na zvukaře Áška
6. **Diskografie** - akordeon s 5 CD (Vzpomínky, 20 let, 30 let, 35 let, 40 let) s obaly CD a přehrávači
7. **Členové** - 5 karet s fotkami + poznámka o konferenciérovi Romanu Dostálovi
8. **Galerie** - akordeon s fotkami z akcí (s popisky)
9. **Kroniky** - 4 díly historických kronik s prohlížečem
10. **Kontakt** - kontaktní údaje + materiály pro pořadatele

## Koncerty 2026
| Datum | Název | Místo | Zvadlo |
|-------|-------|-------|--------|
| 7. 2. 2026 | Písně dávnejch cest | Česká Třebová | ✓ |
| 21. 3. 2026 | Trampské jaro | Chrudim | |
| 30. 5. 2026 | FTP Horní Jelení | Horní Jelení | |
| 17. 10. 2026 | Trampský podzim | Chrudim | |

## Navigace
- Položky: O nás, Novinky, Koncerty, Písničky, Diskografie, Členové, Galerie, Kroniky, Kontakt
- Ikony YouTube a Facebook

## Struktura složek
```
Web/
├── index.html
├── style.css
├── PROJEKT.md
├── images/
│   ├── CHRPA_vlajka.png (logo s průhledným pozadím)
│   ├── CHRPA_vlajka.pdf (originál z tiskárny)
│   ├── chrpa1977.JPG
│   ├── DSC00535 kopie.jpg
│   ├── DSC00540 kopie.jpg (úvodní fotka)
│   ├── DSC00555 kopie.jpg (Tomáš Klásek)
│   ├── DSC00566 kopie.jpg (Jiří Kratochvíl)
│   ├── DSC00571 kopie.jpg (Kamil Kratochvíl)
│   ├── DSC00579 kopie.jpg (Ota Červinka)
│   ├── DSC00587 kopie.jpg (Ája Fandelová)
│   ├── IMG00022 kopie.jpg
│   └── letaky/
│       └── pisne_davnejch_cest.jpg
├── nahravky/
│   ├── 01 Hoj trempové piráti.wav
│   ├── 02 Čajová růže.wav
│   ├── 03 To se mi jen zdá.wav
│   ├── 04 Do ticha hraj mi dál.wav
│   ├── 05 Song abonenta.wav
│   ├── 06 Anita.wav
│   ├── 07 Vodácká.wav
│   ├── 08 Vdovy z Cordoby.wav
│   ├── 09 Černá kára.wav
│   ├── 10 Bye bye podzimu.wav
│   ├── 11 Podzimní zpráva.wav
│   └── 12 Až pojedou časně ráno tramvaje.wav
├── kroniky/
│   ├── CHRPA 1/ (322 stran, soubory 001.jpg - 322.jpg)
│   ├── CHRPA 2/ (293 stran)
│   ├── CHRPA 3/ (323 stran)
│   └── CHRPA 4/ (195 stran)
├── diskografie/
│   ├── CD Vzpominky/ (22 historických nahrávek MP3 + obal_front.jpg, obal_back.jpg)
│   ├── CD Chrpa 20 let/ (14 písní MP3 + obal)
│   ├── CD Chrpa 30 let/ (17 písní MP3 + obal)
│   ├── CD Chrpa 35 let/ (21 písní MP3 + obal)
│   └── CD Chrpa 40 let/ (19 písní MP3 + obal)
├── galerie/
│   ├── 25doli/ (Doli Klub 2025 - 3 fotky)
│   ├── 25chrudim_podzim/ (Trampský podzim Chrudim 2025 - 9 fotek)
│   ├── 25jeleni/ (FTP Horní Jelení 2025 - 5 fotek)
│   ├── 25olesnice/ (Olešnice 2025 - 1 fotka)
│   ├── 16svojsice/ (Svojšice 2016 - 2 fotky)
│   ├── 15gong/ (Náměšťský Gong 2015 - 5 fotek)
│   └── historie/ (Historické fotky)
└── kontakty/
    ├── Stage_plan_Chrpa.png
    ├── logo.png
    ├── foto.jpg
    └── chrpa-text.txt
```

## Členové kapely (současná sestava)
1. **Tomáš Klásek** - harmoniky, zpěv
2. **Jiří Kratochvíl** - baskytara
3. **Kamil Kratochvíl** - doprovodná kytara, zpěv
4. **Ota Červinka** - sólová kytara, zpěv
5. **Ája Fandelová** - zpěv

**Konferenciér:** Roman Dostál (doprovází kapelu na pódiích téměř od vzniku)

## Kontaktní údaje
- **Telefon:** 776 823 528 (Kamil Kratochvíl)
- **Email:** chrpa.chrudim@gmail.com

## Propojené služby
- **YouTube video** - Country rádio k 50. výročí: https://www.youtube.com/watch?v=iwOXblzigy0
- **Facebook stránka** - https://www.facebook.com/profile.php?id=61577306934961

## Text "O nás"
> Trampská skupina Chrpa Chrudim již více než 50 let hraje trampskou muziku, kterou baví své posluchače po celé republice. Stavíme především na vícehlasém zpěvu, který je naším poznávacím znamením a dodává písním osobitý, plný zvuk.
>
> V repertoáru máme písně vlastní i převzaté – od krásných starých trampských klasik až po moderní trampskou píseň. Každý si u nás najde to své.
>
> Kapela vznikla 3. října 1974 a za tu dobu získala řadu ocenění – od Porty přes Náměšťskou placku až po FTP Horní Jelení. Jsme vděční za každé uznání, ale nejvíc nás těší, když vidíme spokojené tváře v publiku.
>
> Na podzim 2024 odešel zakladatel Josef „Bob" Kratochvíl do zaslouženého hudebního důchodu a kapela pokračuje v současné pětičlenné sestavě s nezměněným elánem.

## Co zbývá doplnit
- [x] Kontaktní údaje (telefon, email) ✓
- [x] Odkazy na YouTube a Facebook v navigaci (správné URL) ✓
- [x] Koupit doménu a nahrát web na hosting ✓

---

## HOSTING - Aktuální stav

### Doména
- **Doména:** `chrpachrudim.cz`
- **Registrátor:** [subreg.cz](https://subreg.cz)
- **Administrace:** přihlásit se na subreg.cz

### Hosting
- **Platforma:** [Netlify](https://www.netlify.com) (zdarma)
- **Přihlášení:** Google účet `chrpa.chrudim@gmail.com`
- **URL:** https://chrpachrudim.cz

### DNS nastavení (v subreg.cz)
Pro propojení domény s Netlify byly nastaveny tyto DNS záznamy:

| Typ | Název | Hodnota |
|-----|-------|---------|
| A | @ | 75.2.60.5 |
| CNAME | www | chrpachrudim.netlify.app |

### Jak změnit DNS záznamy
1. Přihlásit se na [subreg.cz](https://subreg.cz)
2. Kliknout na doménu `chrpachrudim.cz`
3. Vybrat **"DNS záznamy"** nebo **"DNS správa"**
4. Upravit/přidat záznamy podle potřeby

### Aktualizace webu
1. Přihlásit se na [app.netlify.com](https://app.netlify.com) (přes Google účet chrpa.chrudim@gmail.com)
2. Kliknout na stránku (site)
3. Přejít na záložku **"Deploys"**
4. Přetáhnout aktualizovanou složku `Web` do sekce "Deploy manually"
5. Nová verze bude online za pár sekund

### Poznámky
- HTTPS certifikát je automaticky poskytnut Netlify (zdarma)
- Facebook Page Plugin nefunguje spolehlivě - nahrazen stylizovaným odkazem na FB stránku
- Soubor `_redirects` zajišťuje přesměrování na index.html (SPA routing)
- Soubor `.htaccess` je záloha pro Apache hostingy

---

## Jak přidat písničku
1. Nahrát WAV/MP3 do složky `nahravky/`
2. V `index.html` v sekci Písničky přidat:
```html
<div class="sample-item">
    <h3>Název písničky</h3>
    <audio controls>
        <source src="nahravky/nazev-souboru.wav" type="audio/wav">
    </audio>
</div>
```

## Jak přidat koncert
V `index.html` v sekci Koncerty přidat řádek do tabulky:
```html
<tr>
    <td data-label="Datum">15. 3. 2026</td>
    <td data-label="Název">Název akce</td>
    <td data-label="Místo">Místo konání</td>
    <td data-label="Zvadlo"></td>
</tr>
```

## Jak přidat zvadlo ke koncertu
1. Nahrát obrázek letáku do `images/letaky/`
2. V tabulce koncertů do buňky Zvadlo přidat odkaz:
```html
<td data-label="Zvadlo"><a href="images/letaky/nazev-souboru.jpg" target="_blank">📄</a></td>
```

## Jak přidat fotku do galerie
```html
<div class="gallery-item">
    <img src="images/nazev-fotky.jpg" alt="Popis">
    <span class="caption">Volitelný popisek fotky</span>
</div>
```
Popisek (`<span class="caption">`) je volitelný - pokud ho nepřidáš, fotka se zobrazí bez něj.

## Technické poznámky
- Web je statický HTML/CSS, bez backendu
- Responzivní design (mobil + PC)
- Písmo: Great Vibes (nadpis), Playfair Display (sekce), Open Sans (text)
- Fonty načítány z Google Fonts
- Nahrávky jsou ve formátu WAV (větší soubory, ale kvalitní)

## Historie kapely (z kroniky)
- **3. října 1974** - založení kapely
- Zakladatel: **Josef „Bob" Kratochvíl**
- První zkouška: u Boba v bytě v Pardubicích
- Zakládající členové: Bob, Hrub, Kolja a Jíra
- **Podzim 2024** - Bob odchází do hudebního důchodu

## Ocenění
- Porta
- Náměšťská placka (festival v Náměšti nad Oslavou)
- FTP Horní Jelení
- Cena diváků na Podlužanské kytaře

## Vzpomínka na Áška
V sekci Písničky je věnování zvukaři Áškovi:
> Písně jsou nahrány z živého koncertu Trampský podzim 2025 a připravil je pro nás náš dlouholetý kamarád a zvukař Ášek, který bohužel několik dní nato podlehl těžké nemoci. Tato sekce slouží i jako vzpomínka na něho.
> *S díky Chrpa*

---

## Diskografie
Sekce s akordeónem pro přehrávání CD (kliknutím na obal se rozbalí seznam písní):
| CD | Počet písní | Formát | Obaly |
|---------|-------------|--------|-------|
| Vzpomínky | 22 | MP3 | obal_front.jpg, obal_back.jpg |
| 20 let | 14 | MP3 | obal.jpg |
| 30 let | 17 | MP3 | obal.jpg |
| 35 let | 21 | MP3 | obal.jpg |
| 40 let | 19 | MP3 | obal.jpg |

**Lightbox:** Kliknutím na malý obrázek obalu se zobrazí ve velkém.

## Galerie - sekce s popisky
| Akce | Počet fotek | Popisky |
|------|-------------|---------|
| Doli Klub 2025 | 3 | Doli klub Pardubice, Chrpa, Country Colaps |
| Trampský podzim Chrudim 2025 | 9 | Plný sál, Chrpa, Ajeto, Béďa Šedivka, 90. narozeniny, jam session aj. |
| FTP Horní Jelení 2025 | 5 | 49. ročník FTP, Porota, Vítězství, Béďa Šedifka, Vyhlášení |
| Olešnice 2025 | 1 | Pozvání od Zmijáků na 40. ročník Olešnické kytky |
| Svojšice 2016 | 2 | - |
| Náměšťský Gong 2015 | 5 | - |
| Historické fotky | 2 | Bob, Chrpa v době největší slávy |

---

## Provedené úpravy (chronologicky)
1. Vytvořena základní struktura webu
2. Barvy upraveny podle loga (#FBB63A, #1E607A)
3. Logo zbaveno bílého pozadí (ručně)
4. Úvodní fotka - text "Chrpa Chrudim" dole uprostřed, logo pod ním
5. Navigace - vycentrovaná, s ikonami soc. sítí
6. O nás - 2 fotky vedle textu + video box Country rádio
7. Novinky - Facebook Page Plugin (přesunuto pod O nás)
8. Koncerty - tabulka
9. Písničky - 12 audio přehrávačů
10. Členové - 5 karet se jmény a nástroji
11. Galerie - mřížka fotek
12. Kroniky - 4 karty s náhledy kronik
13. Kontakt - jednoduchý layout
14. Přesunuty obrázky do `images/`, nahrávky do `nahravky/`
15. Aktualizován text O nás podle požadavků
16. Koncerty - doplněny skutečné termíny na rok 2026
17. Tabulka koncertů - přidán sloupec "Zvadlo" pro letáky
18. Přidán leták k akci Písně dávnejch cest (images/letaky/)
19. Písničky - přidána vzpomínka na zvukaře Áška
20. Členové - odstraněny přezdívky, upraven pořadí nástrojů (nástroj před zpěvem)
21. Galerie - přestavěna na akordeon (kliknutí rozbalí fotky z akce)
22. Galerie - přidán lightbox pro zvětšení fotek
23. Galerie - přidána možnost popisků k fotkám
24. Kroniky - soubory přejmenovány na 001.jpg, 002.jpg atd.
25. Kroniky - přidán prohlížeč s navigací (šipky, klávesy, číslo stránky)
26. Kroniky - aktualizován úvodní text (Roman Dostál - digitalizace)
27. Kontakt - doplněny skutečné údaje (tel, email)
28. Kontakt - přidána sekce "Pro pořadatele" s materiály ke stažení
29. Kontakt - přidána informace o zřizovateli (Beseda Chrudim)
30. Navigace - opraveny odkazy na YouTube a Facebook
31. Vytvořena složka kontakty/ s materiály pro pořadatele
32. Diskografie - nová sekce s 5 záložkami (Archiv, 20-40 let)
33. Diskografie - WMA soubory převedeny na MP3 pomocí ffmpeg
34. Diskografie - všechny soubory přejmenovány bez diakritiky
35. Galerie - přidány nové sekce: Doli Klub 2025, Trampský podzim Chrudim 2025, FTP Horní Jelení 2025, Olešnice 2025
36. Galerie - přidány popisky ke všem fotkám
37. Galerie - Doli Klub 2025 přesunut na první místo (poslední hraní)
38. O nás - změněna fotka na chrpa_odchod.jpg
39. Favicon - přidána vlajka Chrpy do hlavičky webu
40. Vytvořen soubor `_redirects` pro Netlify (přesměrování na index.html)
41. Vytvořen soubor `.htaccess` pro Apache (zakázání výpisu složek)
42. Optimalizace obrázků pomocí ffmpeg (viz sekce níže)
43. Diskografie - změněna z tabů na akordeon (stejný styl jako galerie)
44. Diskografie - "Archiv" přejmenován na "Vzpomínky" s obalem CD
45. Facebook Page Plugin nahrazen stylizovaným odkazem (plugin nefungoval spolehlivě)
46. Opravy responzivního designu pro mobil (iPhone 15 Safari - overflow-x, width)
47. Kontakt - odstraněn text o zřizovateli
48. Členové - přidána poznámka o konferenciérovi Romanu Dostálovi
49. Diskografie - přidán lightbox pro zvětšení obalů CD
50. Diskografie - změněn úvodní obrázek Vzpomínek na obal_front.jpg
51. Optimalizovány obal_front.jpg (4.9 MB → 475 KB) a obal_back.jpg (2.5 MB → 682 KB)
52. Oprava mobilního zobrazení tabulky koncertů (zarovnání textu)

---

## Optimalizace obrázků

Pro rychlejší načítání webu byly všechny velké fotky optimalizovány pomocí ffmpeg.

### Příkaz pro optimalizaci
```bash
ffmpeg -i vstup.jpg -vf "scale=1920:-1" -q:v 3 vystup.jpg
```
- `scale=1920:-1` = šířka max 1920px, výška proporcionálně
- `-q:v 3` = kvalita (1-31, nižší = lepší)

### Výsledky optimalizace

| Složka | Před | Po | Úspora |
|--------|------|-----|--------|
| images/ | 87 MB | 3.9 MB | 95% |
| galerie/ | 53 MB | 7.2 MB | 86% |
| kroniky/ | 1.2 GB | 292 MB | 76% |
| **Celkem** | **1.35 GB** | **~300 MB** | **~78%** |

### Optimalizované soubory v images/
- chrpa_uvodni.jpg (15 MB → 452 KB)
- aja.jpg (13 MB → 402 KB)
- chrpa_odchod.jpg (11 MB → 455 KB)
- chrpa_ruce.jpg (14 MB → 182 KB)
- jirka.jpg (14 MB → 517 KB)
- klokan.jpg (13 MB → 449 KB)
- ota.jpg (12 MB → 488 KB)
- tomas.jpg (12 MB → 553 KB)

### Poznámky
- MP3/MP4 soubory nebyly optimalizovány (nelze bez ztráty kvality)
- Kroniky zmenšeny na max. 1200px šířky (stále čitelné)
- Galerie a hlavní fotky na max. 1920px šířky
