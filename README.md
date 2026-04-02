# Cod reducere Otter — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Otter** de pe [shopilo.ro](https://shopilo.ro/magazin/otter.ro). Returneaza **cupoane Otter** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-otter](https://shopilo-ro.github.io/cod-reducere-otter/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-otter
cd cod-reducere-otter
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Otter",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la toate produsele cu pret intreg",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/otter.ro"
  }
]
```

## Cupoane Otter disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la toate produsele cu pret intreg | [shopilo.ro](https://shopilo.ro/magazin/otter.ro) |

Codurile active: **[shopilo.ro/magazin/otter.ro](https://shopilo.ro/magazin/otter.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Otter?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/otter.ro), adauga produsele in cos pe Otter, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Otter?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Otter?
Pagina [shopilo.ro/magazin/otter.ro](https://shopilo.ro/magazin/otter.ro) este actualizata zilnic cu cele mai noi cod reducere Otter, voucher Otter si cupon promotional Otter.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Otter

Otter este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/otter.ro) cele mai bune cod reducere Otter, cupoane Otter verificate si voucher Otter active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-otter
```

```javascript
const { fetchCoupons } = require('cod-reducere-otter');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
