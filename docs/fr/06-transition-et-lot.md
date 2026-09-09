# Transition d'état et traitement d'un lot

Le module `rollup.rs` applique une séquence de transactions à partir d'un état initial engagé.
Pour chaque transfert, le circuit vérifie l'émetteur, sa signature, son nonce et son solde disponible.
Il débite ensuite l'émetteur, crédite le destinataire et met à jour leurs feuilles.
La racine obtenue après une transaction devient l'entrée de la transaction suivante.
Cette chaîne interdit de prouver séparément des opérations incompatibles puis de combiner leurs résultats.
La racine initiale et la racine finale forment l'énoncé compact que le vérificateur peut publier ou contrôler.
Le nombre maximal de transactions et la profondeur de l'arbre déterminent directement la taille du circuit.

[Chapitre suivant : preuve SNARK](07-preuve-et-verification.md)
