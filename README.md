# Codice sconto Spartoo, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Spartoo** da [shopilo.it](https://shopilo.it/negozi/spartoo.it). Restituisce **coupon Spartoo** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-spartoo](https://shopilo-it.github.io/codice-sconto-spartoo/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-spartoo
cd codice-sconto-spartoo
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Spartoo",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su scarpe e borse",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/spartoo.it"
  }
]
```

## Coupon Spartoo disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su scarpe e borse | [shopilo.it](https://shopilo.it/negozi/spartoo.it) |

Codici attivi: **[shopilo.it/negozi/spartoo.it](https://shopilo.it/negozi/spartoo.it)**

## Domande frequenti

### Come utilizzo un codice sconto Spartoo?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/spartoo.it), aggiungi i prodotti al carrello su Spartoo e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Spartoo?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Spartoo piu recenti?
La pagina [shopilo.it/negozi/spartoo.it](https://shopilo.it/negozi/spartoo.it) viene aggiornata quotidianamente con i codici sconto Spartoo, voucher Spartoo e coupon promozionali Spartoo piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Spartoo

Spartoo e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/spartoo.it) trovi i migliori codici sconto Spartoo, coupon Spartoo verificati e voucher Spartoo attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-spartoo
```

```javascript
const { fetchCoupons } = require('codice-sconto-spartoo');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
