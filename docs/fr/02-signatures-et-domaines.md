# 02 — Signatures et domaines

Les actions sont encodees puis signees selon leur domaine : action L1, agent, transfert ou operation EVM ne sont pas interchangeables.
Le domaine EIP-712, la chaine cible et la structure exacte de la charge utile protegent l intention de l utilisateur.
Une normalisation differente des nombres, adresses ou champs produit une signature portant sur un autre message.
Les helpers du SDK doivent rester la source d encodage plutot qu une reimplementation partielle dans l application.
Avant signature, l interface doit afficher actif, cote, prix, taille, type d ordre et destinataire lorsque pertinent.
La signature prouve une autorisation ; elle ne garantit ni execution ni prix obtenu.
Source : [`hyperliquid/utils/signing.py`](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/hyperliquid/utils/signing.py).

[Suite : nonces](03-nonces-et-reprises.md)
