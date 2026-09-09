# Arbre de Merkle et appartenance

Le registre compresse l'ensemble des comptes dans une racine de Merkle utilisée comme engagement d'état.
Pour modifier un compte, le prouveur fournit sa feuille et le chemin de frères jusqu'à la racine.
Le circuit reconstruit chaque niveau en plaçant le nœud à gauche ou à droite selon l'index.
La racine calculée doit être égale à l'ancienne racine publique avant toute transition.
Après mise à jour du solde ou du nonce, le même chemin permet de dériver une nouvelle racine.
La fonction de hachage et l'encodage de feuille doivent être identiques dans `ledger.rs` et dans les contraintes.
Un index non contraint ou un chemin réutilisé au mauvais endroit pourrait rompre l'appartenance prouvée.

[Chapitre suivant : transition d'état](06-transition-et-lot.md)
