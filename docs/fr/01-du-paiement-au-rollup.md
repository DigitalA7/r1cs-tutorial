# Du paiement au rollup SNARK

Le tutoriel arkworks construit progressivement un système de paiement puis l'encapsule dans un circuit de rollup.
Le code sépare les comptes, les transactions, le registre et les contraintes R1CS qui reproduisent leur logique.
Une preuve SNARK atteste qu'un lot de transactions transforme correctement un ancien état en un nouvel état.
Le vérificateur n'a pas besoin de rejouer chaque transfert ni de connaître tous les témoins privés.
Les racines de Merkle représentent compactement les états avant et après le lot.
Le circuit vérifie signatures, soldes, nonces et chemins d'appartenance avant de calculer la nouvelle racine.
Ce parcours suit cette transition d'état et souligne les invariants qui doivent être contraints.

[Chapitre suivant : comptes et clés](02-comptes-cles-soldes.md)
