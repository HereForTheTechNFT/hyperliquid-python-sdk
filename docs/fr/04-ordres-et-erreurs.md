# 04 — Ordres, annulations et erreurs partielles

Une reponse HTTP reussie ne signifie pas que chaque ordre du lot a ete accepte.
Le client doit examiner le statut de chaque element et conserver la correspondance avec l intention d origine.
Les ordres limites, market abstraits en limites, triggers et reductions de position n ont pas les memes risques.
Une annulation peut croiser une execution deja survenue ; le portefeuille doit reconciler fills, ordres ouverts et position.
Les tailles et prix doivent respecter les precisions de l actif avant signature, sans arrondi silencieux defavorable.
La boucle sure est : soumettre, interpreter chaque statut, relire l etat, puis seulement decider d un retry.
Sources : [`hyperliquid/exchange.py`](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/hyperliquid/exchange.py) et [`examples`](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/tree/master/examples).

[Suite : checklist](05-checklist-production.md)
