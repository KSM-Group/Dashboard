# REDLOGIS KPI Dashboard

Dashboard analityczny dla magazynu Redlogis (SYCÓW).

## 🚀 Deployment

Hosted on **GitHub Pages**: `https://redlogis.github.io/warehouse-dashboard/`

## 📁 Struktura

```
/
├── index.html          # Główny dashboard (single-file app)
└── README.md
```

## 🔐 Dostęp

Dashboard chroniony hasłem logowania. Hasło zarządzane przez administratora.

Zakładki chronione dodatkowo:
- 🎯 **KPI** — hasło: `KPI`
- 👥 **Pracownicy** — hasło: `Pracownicy`

## 📊 Pliki źródłowe (wczytywane ręcznie)

| Plik | Źródło |
|---|---|
| `Dokumenty_export.xlsx` | PinQuark WMS → Wydanie-widżet |
| `Rejestr_operacji.xlsx` | PinQuark WMS → Operacje |
| `Dokumenty_z_etykietami.xlsx` | PinQuark WMS → Etykiety kurierskie |

Dane są zapamiętywane w `localStorage` przeglądarki i wczytują się automatycznie przy kolejnym otwarciu.

## 🔧 Stack techniczny

- **SheetJS** 0.18.5 — parsowanie XLSX
- **Chart.js** 4.4.0 — wykresy
- Brak backendu, brak serwera, brak instalacji

## 🗺️ Roadmap

- [ ] Live API z Azure Function (`pinquark-proxy-redlogis`)
- [ ] Auto-refresh co minutę po podłączeniu API
- [ ] Widok tygodniowy/miesięczny w Terminowości
- [ ] Integracja z listą obecności (Microsoft Graph API)

## 📞 Kontakt

Repo: `Redlogis/warehouse-dashboard` (prywatne)
