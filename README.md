# Code promo Lebara, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Lebara** depuis [shopilo.fr](https://shopilo.fr/reductions/lebara.fr). Renvoie les **coupons Lebara** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-lebara](https://shopilo-fr.github.io/code-promo-lebara/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-lebara
cd code-promo-lebara
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Lebara",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les forfaits mobiles",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/lebara.fr"
  }
]
```

## Coupons Lebara disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les forfaits mobiles | [shopilo.fr](https://shopilo.fr/reductions/lebara.fr) |

Codes actifs : **[shopilo.fr/reductions/lebara.fr](https://shopilo.fr/reductions/lebara.fr)**

## Questions frequentes

### Comment utiliser un code promo Lebara ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/lebara.fr), ajoutez les produits a votre panier sur Lebara et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Lebara ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Lebara les plus recents ?
La page [shopilo.fr/reductions/lebara.fr](https://shopilo.fr/reductions/lebara.fr) est mise a jour quotidiennement avec les codes promo Lebara, bons de reduction Lebara et coupons promotionnels Lebara les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Lebara

Lebara est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/lebara.fr), retrouvez les meilleurs codes promo Lebara, coupons Lebara verifies et bons de reduction Lebara actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-lebara
```

```javascript
const { fetchCoupons } = require('code-promo-lebara');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
