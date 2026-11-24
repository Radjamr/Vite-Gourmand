%%mocodo
:::
utilisateur: utilisateur id, nom, email, password, prenom, telephone, ville, pays, adresse postale, #role id > role > role id
:::
commande: numero commande, date commande, date prestation, heure livraison, prix menu, nombre personne, prix livraison, pret materiel, restitution matériel, #utilisateur id > utilisateur > utilisateur id, #menu id > menu > menu id
:::


:
role: role id, libelle
:::
regime: regime id, libelle
:::
suivi: suivi id, statut, date heure, #numero commande > commande > numero commande
:


:
horaire: horaire id, jour, heure ouverture, heure fermeture
:
avis: avis id, note, description, statut, #utilisateur id > utilisateur > utilisateur id
:::
menu: menu id, titre, nombre personne minimum, prix par personne, description, quantite restante, #regime id > regime > regime id, #theme id > theme > theme id
:::


:
allergene: allergene id, libelle
:
contient: #plat id > plat > plat id, _#allergene id > allergene > allergene id
:
plat: plat id, titre plat, photo
:
repas: #menu id > menu > menu id, _#plat id > plat > plat id
:
theme: theme id, libelle
: