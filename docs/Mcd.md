# MCD - Vite & Gourmand

![MCD](mcd.png)

## Code Mocodo

```
possede, 11 utilisateur, 0N role
utilisateur : utilisateur id, nom, email, password, prenom, telephone, ville, pays, adresse postale
commander, 0N utilisateur, 11 commande
commande : numero commande, date commande, date prestation, heure livraison, prix menu, nombre personne, prix livraison, pret materiel, restitution matériel
suivre, 1N commande, 11 suivi

role : role id, libelle
publie, 0N utilisateur, 11 avis
regime : regime id, libelle
choisir, 0N menu, 11 commande
suivi : suivi id, statut, date heure

horaire : horaire id , jour, heure ouverture, heure fermeture
avis : avis id, note, description, statut
adapte, 11 menu, 0N regime
menu : menu id, titre, nombre personne minimum, prix par personne, description, quantite restante
propose, 11 menu, 0N theme

allergene : allergene id, libelle
contient, 0N plat, 0N allergene
plat : plat id, titre plat, photo
repas, 1N menu, 0N plat
theme: theme id, libelle
```
