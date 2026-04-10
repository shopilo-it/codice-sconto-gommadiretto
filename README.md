# Codice sconto Gommadiretto, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Gommadiretto** da [shopilo.it](https://shopilo.it/negozi/gommadiretto.it). Restituisce **coupon Gommadiretto** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-gommadiretto](https://shopilo-it.github.io/codice-sconto-gommadiretto/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-gommadiretto
cd codice-sconto-gommadiretto
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Gommadiretto",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su pneumatici online",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/gommadiretto.it"
  }
]
```

## Coupon Gommadiretto disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su pneumatici online | [shopilo.it](https://shopilo.it/negozi/gommadiretto.it) |

Codici attivi: **[shopilo.it/negozi/gommadiretto.it](https://shopilo.it/negozi/gommadiretto.it)**

## Domande frequenti

### Come utilizzo un codice sconto Gommadiretto?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/gommadiretto.it), aggiungi i prodotti al carrello su Gommadiretto e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Gommadiretto?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Gommadiretto piu recenti?
La pagina [shopilo.it/negozi/gommadiretto.it](https://shopilo.it/negozi/gommadiretto.it) viene aggiornata quotidianamente con i codici sconto Gommadiretto, voucher Gommadiretto e coupon promozionali Gommadiretto piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Gommadiretto

Gommadiretto e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/gommadiretto.it) trovi i migliori codici sconto Gommadiretto, coupon Gommadiretto verificati e voucher Gommadiretto attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-gommadiretto
```

```javascript
const { fetchCoupons } = require('codice-sconto-gommadiretto');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
