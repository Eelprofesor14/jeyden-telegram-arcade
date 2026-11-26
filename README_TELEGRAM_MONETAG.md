# Telegram Mini Apps + Monetag / AdsGram Bundle ($5 PayPal / USDT Payout)

## 1. Deploy Gratis en 30 Segundos (HTTPS Obligatorio para Telegram)
- **Opción A (Cloudflare Pages Drop):** Entrá a `https://dash.cloudflare.com/` > `Workers & Pages` > `Create` > `Pages` > `Upload assets` y arrastrá esta carpeta `telegram-miniapps-monetag`.
- **Opción B (GitHub Pages):** Subí esta carpeta a un repo público en `Eelprofesor14` y activá `Settings > Pages`.

## 2. Conectar en Telegram (`@BotFather`)
1. Abrí `@BotFather` en Telegram y enviá `/newbot` (ej. `Jeyden Neon Arcade`, `@JeydenArcadeBot`).
2. Enviá `/newapp`, elegí el bot, subí el ícono `512x512` de `orbit-breaker-six-stores/covers/` y pegá la URL HTTPS de tu deploy.

## 3. Activar Monetización ($0 mínimo de tráfico)
1. En **Monetag** (`https://monetag.com` -> *Telegram Mini Apps*), creá una zona *Rewarded Interstitial* y copiá el `<script src='//libtl.com/sdk.js' data-zone='XXXX' data-sdk='show_XXXX'></script>`.
2. Pegá ese `<script>` en el `<head>` de `orbit-breaker/index.html` y definí `window.ORBIT_MONETAG_FN = 'show_XXXX';` — `StoreBridge` ya llama automáticamente a `window[ORBIT_MONETAG_FN]()` en cada transición de sector y botón de *Revive*!
