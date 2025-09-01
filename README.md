# Snusslutt PWA

En enkel Progressive Web App du kan installere på mobil (Android/iOS) eller desktop. Fungerer offline.

## Filer
- `index.html` – Hovedappen (alt UI og logikk).
- `manifest.webmanifest` – App-manifest for installasjon.
- `service-worker.js` – Offline-cache av app-skjellettet.
- `icons/icon-192.png`, `icons/icon-512.png` – App-ikoner.

## Bruk
1. Åpne `index.html` fra en enkel webserver (for eksempel VS Code Live Server, `python3 -m http.server` eller last opp til Netlify/Vercel/GitHub Pages).
2. I appen: fyll inn slutt-dato, pris pr. boks, forbruk pr. uke, mål-dager og lagre.
3. Installer som app:
   - **iPhone (Safari):** Del-ikon → *Legg til på Hjem-skjermen*.
   - **Android (Chrome):** Meny ⋮ → *Installer app*.
4. Appen lagrer alt lokalt i `localStorage`.
5. Offline fungerer etter første besøk (service worker må få cachet filene).

## Notat
Helsepunktene er generelle motivasjons-milesteiner – ikke medisinske råd.
