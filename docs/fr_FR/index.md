# Plugin gestionmsg

gestionmsg est un plugin **Jeedom** qui permet de gérer les destinataires et messages associés.

# Configuration du plugin
Après avoir installé le plugin, il vous suffit de l’activer. Ce plugin n’a aucune configuration particulière :

![Image Configuration_Plugin](/images/ConfPlugin.PNG)

# Configuration des équipements
La configuration des équipements gestionmsg est accessible à partir du menu plugin :

![Image Chemin Equipement](/images/ConfEqChemin.PNG)


# Page d'Accueil

![Image Accueil Equipement](/images/ConfEqAccueil.PNG)

* **Ajouter** : permet d'ajouter un équipement
* **Configuration** : permet d'accéder à la configuration du PLUGIN
* **Gestion Destinataire** : permet de gérer les destinataires (nom, e-mail, tel...)

## Gestion des destinataires

![Image modal Gestion Destinataires](/images/mdGestionDestinataires.PNG)

Depuis cette fenêtre, on peut gérer les destinataires:
* **Ajouter** : ajout d'un destinataire
* **Ajouter Users Jeedom** : ajout des utilisateurs Jeedom configurés dans la section *Réglages->Système->Utilisateurs*
 - leur numero de téléphone et e-mail sont renseignés **uniquement** si les plugins *mail et sms* sont installés et qu'une commande portant le nom du User est configurée sinon il faut le renseigner manuellement.
 - si un destinataire porte le nom d'un User Jeedom alors les champs tel et mail sont remplacés si vide.
* **SynchroJeedom** : permet de synchroniser les destinataires du plugin gestionmsg avec les users Jeedom et les plugins de type communication (*mail et sms*).
 - Si le destinataire n'existe pas dans les Users alors un User du nom du destinataire sera créé (il sera non actif, et sans droits).
 - Si une commande porte le nom du destinataire dans les plugins de type communication alors les numeros de telephone et e-mail seront mis à jour.
* **Supprimer**: permet de supprimer en meme temps les destinataires selectionnés 

**LE PLUGIN AJOUTE OU MET A JOUR JEEDOM OU LES AUTRES PLUGINS MAIS NE SUPPRIME PAS DES COMMANDES.**


![Image modal Entete](/images/mdGestionDestinatairesEntete.PNG)

* **LOGIN** : renseigner le nom du destinataire.
* **E-mail** : renseigner l'e-mail du destinataire.
* **Tel.** : renseigner le numero de telephone du destinataire au format +33xxxxxxxxx.
* **Utilisateur Jeedom** : indique si le destinataire est un User Jeedom.
* **Synchronisé** : indique si il y a eu une SynchroJeedom (la date et heure s'affichent).
* **Actions** : Sauvegarder ou Supprimer destinataire.
* **Selection** : si cochée alors tous les destinataires sont selectionnés. (pour par exemple supprimer plusieurs destinataires en meme temps).
                

## Ajouter un équipement gestionmsg

![Image Accueil Equipement](/images/EqAccueil.PNG)




