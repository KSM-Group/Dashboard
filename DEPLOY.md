# 🚀 Instrukcja wdrożenia na GitHub Pages

## Krok 1 — Przygotuj repo

```bash
# Sklonuj istniejące repo (lub utwórz nowe)
git clone https://github.com/Redlogis/warehouse-dashboard.git
cd warehouse-dashboard

# Skopiuj pliki z tego archiwum do folderu repo
# - index.html
# - README.md
# - .github/workflows/deploy.yml
```

## Krok 2 — Wgraj pliki i zrób push

```bash
git add .
git commit -m "feat: deploy KPI dashboard v20"
git push origin main
```

## Krok 3 — Włącz GitHub Pages w ustawieniach repo

1. Wejdź na: `https://github.com/Redlogis/warehouse-dashboard/settings/pages`
2. **Source** → `GitHub Actions`
3. Kliknij **Save**

## Krok 4 — Poczekaj ~2 minuty

GitHub Actions automatycznie zbuduje i wdroży. Status widoczny w zakładce **Actions**.

## Wynik

Dashboard dostępny pod adresem:
```
https://redlogis.github.io/warehouse-dashboard/
```

---

## 🔐 Zmiana hasła logowania

W pliku `index.html` znajdź linię:
```javascript
const LOGIN_PWD = 'Redlogis2026';
```
Zmień na wybrane hasło i zrób `git push`.

---

## 🔄 Aktualizacja dashboardu

Każdy `git push` do brancha `main` automatycznie wdraża nową wersję (GitHub Actions).

---

## ⚠️ Uwagi

- Repo **prywatne** + GitHub Pages **wymaga planu GitHub Pro/Team** (~$4/mies per user)
- Alternatywa: ustaw repo jako **publiczne** (Pages działa bezpłatnie) — dashboard i tak chroniony hasłem
- `localStorage` działa per domena — dane zapisane na `github.io` będą dostępne dla każdego użytkownika na tej maszynie
