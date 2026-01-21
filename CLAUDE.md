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
    "platnost_od": "",
    "platnost_do": "7.2.2026"
}
```

### 2. Příspěvek (novinka, oznámení)

```json
{
    "typ": "prispevek",
    "datum": "21. 1. 2026",
    "text": "Text příspěvku...",
    "obrazek": "images/novinky/fotka.jpg",
    "platnost_od": "",
    "platnost_do": ""
}
```

Příspěvek bez obrázku - zobrazí se logo Chrpy:
```json
{
    "typ": "prispevek",
    "datum": "21. 1. 2026",
    "text": "Text příspěvku bez obrázku...",
    "obrazek": "",
    "platnost_od": "",
    "platnost_do": ""
}
```

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
