# Production et vérification de la preuve

Une fois le circuit synthétisé, le système SNARK produit des paramètres, une clé de preuve et une clé de vérification.
Le prouveur combine le circuit, les témoins privés et les entrées publiques pour créer une preuve succincte.
Le vérificateur reçoit la preuve avec l'ancien et le nouvel engagement d'état.
Il vérifie la relation sans apprendre les clés privées ni reconstruire toutes les branches Merkle.
Selon le schéma choisi, la génération des paramètres peut exiger une cérémonie de confiance spécifique au circuit.
Toute modification de forme du circuit peut rendre les anciennes clés incompatibles.
L'application qui accepte la preuve doit également valider le format et la sémantique des entrées publiques.

[Chapitre suivant : limites](08-limites-et-verification.md)
