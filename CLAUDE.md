Landing page pour presenter un project de swap on chain pour des banques.
Juste une landing page propre tres pro qui vise le comex de banques.
Tout le site doit etre ecrit en anglais
Design tres pro, sobre, a destination des institutions financières.
Garde un ton formel et rassurant, compatible avec le monde de la finance de marche., en mettant en avant la sécurité, la rapidité, la compliance et la flexibilité de la solution.

Apres chaque modif je veux que tu essatye d ouvrir le site voir si il marche encore.

## Blockchain
- Coder sur Canton (pas Ethereum). Retirer toute mention d'Ethereum comme plateforme.
- ETH comme token peut rester si pertinent, mais la blockchain est Canton.
- Avantages Canton : publique + privacy native dans les echanges.

## Fonctionnalites a integrer

### Limites de trading (section config)
- La banque fixe un plafond de notional par sous-jacent (actions, indices) pour le client.
- Le client peut modifier son notional a l interieur de ces plafonds.
- Si le client fait une demande de changement, la banque doit ACK (approuver).

### Kill switch (section config)
- Kill switch qui renvoie les fonds a leurs proprietaires en cas de bug.

### Periode d expiration (section config uniquement)
- Moment ou le swap expire : la banque peut alors mettre a jour les limites et le collateral.

## Avantages a mettre en avant
- Rapidite, securite, flexibilite, compliance
- Reduction des couts d intermediation
- Banque et client interagissent avec le meme SI
- Partage d actifs IT car codes sur la meme chaine
- Interoperabilite avec d autres acteurs


Les "Features" Techniques (Points saillants)
Utilise les points suivants pour rédiger la section "Comment ça marche" :

Block chain prive avec permission
Confidentialité Native (Daml) : Explique que contrairement aux blockchains classiques, les détails du swap (notionnel, maturité, taux) ne sont visibles que par les deux contreparties. "Ce que vous tradez ne regarde que vous."

Architecture "Zero-Infrastructure" pour le client : Précise que le client n'a pas besoin de gérer de nœud. Il accède au réseau via une interface sécurisée hébergée par la banque, tout en gardant une preuve cryptographique de ses transactions.
Ajoute que si besoin le client peut faire run son propre noeud.

Règlement Atomique

Interopérabilité : Mentionne que le swap peut être connecté à d'autres réseaux du Canton Network (Cash, Titres, Collatéral) pour une fluidité totale.
La gestion du colateral peut se faire ainsi. 
Connection via Zenith pour faire ETH -> Canton.

Constrained Collateral : le collat profite de l ecosysteme Canton pour etre investi dans des protocoles money-market et obligataires tokenises. Ajoute dans la section Technical Architecture.

Kill switch : supprime cette partie. Explique que grace a la blockchain canton les fonds ne peuvent pas etre bloque en cas de bug car si les deux partie sont ok le contrat peut etre update