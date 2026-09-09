# R1CS et gadgets

R1CS exprime le calcul comme des contraintes multiplicatives entre combinaisons linéaires.
Arkworks alloue les valeurs publiques comme entrées et les données privées comme témoins.
Les gadgets traduisent hachage, comparaison, sélection conditionnelle et signature dans ce langage.
Chaque branche logique doit devenir une contrainte ; une condition évaluée seulement en Rust n'est pas prouvée.
Les variables booléennes doivent aussi être contraintes à zéro ou un avant de servir de sélecteurs.
La satisfaction d'un système R1CS signifie uniquement que les équations déclarées sont vraies.
La sécurité dépend donc de l'exhaustivité des contraintes autant que de la primitive SNARK choisie.

[Chapitre suivant : arbre de Merkle](05-merkle-et-appartenance.md)
