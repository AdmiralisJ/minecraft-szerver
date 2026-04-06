# VRCBűnvadászok – Docs

MkDocs Material alapú dokumentációs oldal.

## Telepítés

### 1. Python és pip
Szükséges a Python 3.8+. Ellenőrzés:
```bash
python --version
```

### 2. MkDocs Material telepítése
```bash
pip install mkdocs-material
```

### 3. Helyi előnézet
```bash
cd vrcbunvadaszok
mkdocs serve
```
Ezután nyisd meg: http://127.0.0.1:8000

### 4. Build (statikus fájlok generálása)
```bash
mkdocs build
```
A `site/` mappában lesznek a kész HTML fájlok – ezt töltsd fel a szerveredre.

---

## Saját domainre feltöltés

A `mkdocs build` után a `site/` mappa tartalmát töltsd fel a webszerveredre
(pl. FTP, vagy a tárhelyed file managere segítségével).

A `mkdocs.yml`-ben állítsd be a saját domain-t:
```yaml
site_url: https://docs.vasarnaplened.hu
```

---

## Tartalom szerkesztése

Minden oldal a `docs/` mappában van, sima Markdown fájlok:

| Fájl | Oldal |
|------|-------|
| `docs/index.md` | Kezdőlap |
| `docs/csatlakozas.md` | Csatlakozás |
| `docs/szabalyok.md` | Szabályok |
| `docs/tagok.md` | Tagok |

Új oldalt hozzáadni:
1. Hozz létre egy új `.md` fájlt a `docs/` mappában
2. Add hozzá a `mkdocs.yml` `nav:` részéhez

---

## Dokumentáció

- [MkDocs Material docs](https://squidfunk.github.io/mkdocs-material/)
- [Admonitions (callout dobozok)](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)
- [Ikonok](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/)
