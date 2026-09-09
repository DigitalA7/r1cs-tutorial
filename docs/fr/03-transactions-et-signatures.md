# Transactions et signatures

Une transaction décrit l'émetteur, le destinataire, le montant et les données nécessaires à l'anti-rejeu.
Le message signé doit couvrir tous les champs qui influencent la transition d'état.
Le tutoriel utilise une signature de type Schnorr et fournit sa version native ainsi que ses contraintes.
La vérification dans le circuit prouve que le détenteur de la clé privée a autorisé l'opération.
L'oracle aléatoire dérive un défi à partir du message et des éléments de la signature.
Un encodage différent entre la création du message et le gadget R1CS invaliderait le lien cryptographique.
La signature seule ne suffit pas : le circuit vérifie aussi l'existence du compte et la disponibilité du solde.

[Chapitre suivant : R1CS](04-r1cs-et-gadgets.md)
