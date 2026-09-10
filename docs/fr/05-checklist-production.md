# 05 — Checklist d integration defensive

1. Separer services de lecture, signataire et moteur de strategie.
2. Verrouiller le reseau, l URL API et le domaine de signature attendus.
3. Coordonner les nonces entre processus et persister les intentions avant envoi.
4. Valider precision, taille minimale, prix, slippage et indicateur reduce-only.
5. Interpreter les statuts par element et reconciler fills, ordres et positions apres timeout.
6. Limiter les clefs agents, masquer les secrets et journaliser sans charge signee sensible.
Ce parcours est documentaire, pas un audit ni un conseil de trading. Aucune installation ou execution de tests n a ete effectuee.
Source de verification future : [`tests`](https://github.com/hyperliquid-dex/hyperliquid-python-sdk/tree/master/tests).

[Retour au sommaire](README.md)
