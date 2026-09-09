# Comptes, clés, soldes et nonces

Le module `account.rs` regroupe les données nécessaires pour identifier et faire évoluer un compte.
Une clé publique relie le compte à l'autorité capable d'autoriser une transaction.
Le solde borne la valeur transférable et le nonce impose un ordre aux opérations d'un même émetteur.
Dans le code natif, ces champs sont des valeurs Rust ; dans le circuit, ils deviennent des variables contraintes.
La représentation en bits ou en éléments de corps doit être identique lors du hachage et de la vérification.
Le nonce empêche qu'une transaction valide soit rejouée contre le même état.
Le circuit doit relier chaque nouvelle valeur à l'ancienne au lieu d'accepter un témoin libre fourni par le prouveur.

[Chapitre suivant : transactions](03-transactions-et-signatures.md)
