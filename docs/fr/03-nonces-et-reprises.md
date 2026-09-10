# 03 — Nonces, agents et reprises

Le nonce participe a l unicite temporelle des actions signees et ne doit pas etre produit independamment par plusieurs workers sans coordination.
Un redemarrage peut rejouer une intention dont le resultat reseau est encore inconnu.
Il faut persister un identifiant applicatif, le nonce, le hash de requete et le resultat observe avant toute nouvelle tentative.
Une cle agent reduit l exposition de la cle principale, mais ses permissions et son cycle de vie doivent etre suivis.
Les horloges locales, files de retry et executions concurrentes sont donc des composants de securite.
En cas de timeout, interroger l etat avant de resoumettre une action financiere.
Source : [`hyperliquid/exchange.py`](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/hyperliquid/exchange.py).

[Suite : cycle des ordres](04-ordres-et-erreurs.md)
