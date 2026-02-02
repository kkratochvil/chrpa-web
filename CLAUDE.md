# Chrpa Chrudim - Web

## Struktura projektu

- `index.html` - hlavní stránka webu
- `style.css` - styly
- `akce.json` - novinky a akce (editovatelné)
- `images/letaky/` - složka pro letáky akcí

## Editace novinek

Novinky se načítají ze souboru `akce.json`. Podporované jsou dva typy:

### 1. Akce (koncert, festival)

```json
{
    "typ": "akce",
    "nazev": "Název akce",
    "datum": "7. 2. 2026",
    "cas": "18:00",
    "misto": "Místo konání",
    "popis": "Popis akce...",
    "vstupne": "350 Kč",
    "letak": "images/letaky/nazev_letaku.jpg",
    "tlacitko_text": "Zobrazit leták",
    "tlacitko_link": "",
    "platnost_od": "",
    "platnost_do": "7.2.2026"
}
```

#### Tlačítko u akce

| Pole | Popis |
|------|-------|
| `tlacitko_text` | Text tlačítka (např. "Koupit lístky", "Web akce"). Pokud prázdné, tlačítko se nezobrazí. |
| `tlacitko_link` | Odkaz tlačítka. Pokud prázdné, použije se cesta z `letak`. |

Příklady:
- **Bez tlačítka:** `"tlacitko_text": ""`
- **Odkaz na leták:** `"tlacitko_text": "Zobrazit leták"`, `"tlacitko_link": ""`
- **Koupit lístky:** `"tlacitko_text": "Koupit lístky"`, `"tlacitko_link": "https://goout.cz/..."`
- **Web autora:** `"tlacitko_text": "Web kapely"`, `"tlacitko_link": "https://example.com"`

### 2. Příspěvek (novinka, oznámení)

```json
{
    "typ": "prispevek",
    "datum": "21. 1. 2026",
    "nadpis": "Název příspěvku",
    "text": "Text příspěvku...",
    "obrazek": "images/novinky/fotka.jpg",
    "tlacitko_text": "Fotky na Facebooku",
    "tlacitko_link": "https://facebook.com/album/...",
    "platnost_od": "",
    "platnost_do": ""
}
```

Příspěvek bez obrázku - zobrazí se kompaktně:
```json
{
    "typ": "prispevek",
    "datum": "1. 2. 2026",
    "nadpis": "Hraní v pivnici Svatý Mikuláš",
    "text": "V sobotu jsme na pozvání kamaráda zajeli zahrát...",
    "obrazek": "",
    "tlacitko_text": "Fotky na Facebooku",
    "tlacitko_link": "https://facebook.com/album/...",
    "platnost_od": "",
    "platnost_do": "6.2.2026"
}
```

| Pole | Popis |
|------|-------|
| `nadpis` | Název/titulek příspěvku (volitelný) |
| `text` | Delší popis, co se dělo |
| `obrazek` | Cesta k obrázku (prázdné = kompaktní zobrazení) |
| `tlacitko_text` | Text tlačítka (prázdné = bez tlačítka) |
| `tlacitko_link` | Odkaz např. na FB album |

## Platnost příspěvků

| Nastavení | Chování |
|-----------|---------|
| Nic nenastaveno | Zobrazuje se vždy |
| Jen `platnost_od` | Zobrazí se od daného data |
| Jen `platnost_do` | Zobrazí se do daného data |
| Obojí | Zobrazí se v daném rozmezí |

Formát data: `D.M.YYYY` (např. `1.1.2026` nebo `15.12.2026`)

## Jak přidat novou položku

1. Otevři `akce.json` v textovém editoru
2. Přidej nový objekt do pole (nezapomeň čárku za předchozím):

```json
[
    {
        "typ": "prispevek",
        "datum": "25. 1. 2026",
        "text": "Nový příspěvek...",
        "obrazek": "",
        "platnost_od": "",
        "platnost_do": ""
    },
    {
        "typ": "akce",
        "nazev": "Existující akce",
        ...
    }
]
```

3. Ulož soubor

## Deploy na web (Git)

```bash
cd D:\Chrpa\Chrpa\Web
git add akce.json
git commit -m "nova akce"
git push
```

Netlify automaticky deployne změny na **chrpachrudim.cz**.

## Pravidla JSON

- Mezi položkami musí být **čárka** (kromě poslední)
- Texty v **uvozovkách** `"text"`
- Prázdné hodnoty: `""`
- Obrázky/letáky nahrát do příslušné složky v `images/`

## Hosting

- **Netlify** - automatický deploy z GitHubu
- **GitHub repozitář**: https://github.com/kkratochvil/chrpa-web

## Tvorba obrázků a plakátů

### Obrázky (pozadí, ilustrace)

Vytvořeno pomocí **ChatGPT** (DALL-E) - stačí popsat, co chceš vygenerovat.

### Plakáty

Vytvořeno pomocí **Canva** (canva.com, zdarma):

1. Jdi na [canva.com](https://canva.com)
2. „Vytvořit návrh" → Plakát
3. Nahraj obrázek (např. z ChatGPT)
4. Přidej text (nadpis, datum, místo...)
5. Export → PNG nebo PDF (pro tisk)

Tipy:
- Text lze umístit nahoře do prázdného prostoru nebo dole na „pergamen"
- Canva má krásné fonty a snadné zarovnání
- Ideální pro koncertní plakáty

### Optimalizace obrázků

Velké obrázky (PNG) převést na JPG pomocí ffmpeg:
```bash
ffmpeg -i plakat.png -q:v 2 plakat.jpg
```
Výrazně zmenší velikost souboru (typicky 70-80% úspora).
