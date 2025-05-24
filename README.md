# Uniswap WalletConnect PoC

## 💥 Vulnerability
This proof-of-concept demonstrates abuse of `walletconnect://` URI handling inside Uniswap's iframe-loaded interface using `callback=` param.

## 🧪 Simulation
- Loads iframe with `callback=walletconnect://attacker.site`
- Sends `postMessage` to request `eth_requestAccounts`
- Logs any response using `log.php`

## 🛠 Setup
1. Deploy to Vercel or any PHP host (if `log.php` is needed)
2. Visit the site, open DevTools Console
3. Observe postMessage logs or `log.txt`

## ⚠️ Warning
**This is for educational and authorized security research only.**
