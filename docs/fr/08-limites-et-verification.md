# Limites et points de vérification

Ce dépôt est un tutoriel : il illustre les contraintes d'un rollup, pas une implémentation prête pour la production.
Le parcours ne couvre pas disponibilité des données, séquenceur, dépôts et retraits L1, récursion ni gouvernance des clés.
Les bornes numériques, collisions d'encodage, indices Merkle et conditions d'échec méritent une revue dédiée.
Une vraie intégration doit aussi définir quelles données sont publiques et comment elles sont liées au contrat vérificateur.
Aucune installation, compilation ou exécution nouvelle n'a été réalisée pendant cette lecture documentaire.
Les tests présents dans les crates `simple-payments`, `merkle-tree-example` et `rollup` sont les références de validation.
Les garanties décrites ici proviennent du code observé et ne constituent pas un audit cryptographique.

[Retour au sommaire](README.md)
