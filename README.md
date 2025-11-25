## 🎄 BabboNataleSegretoFe

Frontend minimale e intuitivo per il tuo Secret Santa:
- Lista di nomi per l’input
- Output chiaro e semplice

## 🚀 Installazione e Avvio
# Installa dipendenze

```bash
npm install
```

# Avvia frontend in dev mode
npm run dev

## Configurazione backend

Nel file main.ts modifica la prima riga per mettere il link che connette il backend:

const apiUrl = "https://tuo-backend-link.cloudflared.com"; // esempio

## Esporre la porta per il frontend
Opzione 1 – Cloudflare Tunnel (consigliata)
# Installa cloudflared

```bash
brew install cloudflare/cloudflare/cloudflared
```
# Avvia il tunnel sulla porta 5173
```bash
cloudflared tunnel --url http://localhost:5173
```


Ti verrà fornito un URL pubblico tipo https://random-string.trycloudflare.com.

Opzione 2 – Ngrok
# Avvia tunnel ngrok sulla porta 5173
```bash
http ngrok 5173
```

Ti darà un link pubblico temporaneo per usare il frontend.

🔗 Uso del link

Per usare il frontend correttamente:

# Aggiungi il token come parametro "t" al link
https://12345ab6789c.ngrok-free.app/?t=MPNu64bFHwrlWt65pMW8Qw==:wmIyrOrw5AhApAb4f4avFA


Il token permette al frontend di identificarti e ricevere l’estrazione corretta.
