# 01 — Separer Info et Exchange

Le SDK distingue les lectures de marche et de compte (`Info`) des actions signees (`Exchange`).
Cette frontiere limite les clefs privees aux chemins qui en ont reellement besoin.
Les lectures publiques peuvent utiliser une adresse de compte sans disposer du signataire.
Les actions d ordre, de transfert ou de retrait passent par une charge utile canonique et une signature.
Une application doit conserver cette separation jusque dans ses services et journaux.
Ne jamais placer la cle privee dans un composant seulement charge d afficher le carnet ou les positions.
Sources : [`hyperliquid/info.py`](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/hyperliquid/info.py) et [`exchange.py`](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/blob/master/hyperliquid/exchange.py).

[Suite : signatures et domaines](02-signatures-et-domaines.md)
