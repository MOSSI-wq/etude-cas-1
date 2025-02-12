SIDIALI MOSLIM
HIBA BENJELLOUN
Classe:5IIR7

Ce microservice permet de réaliser des opérations CRUD sur une entité "COMMANDE" sans utiliser de lignes SQL. Il inclut les fonctionnalités suivantes :

La table "COMMANDE" (version 1) contient les colonnes suivantes : id, description, quantité, date, montant.
La configuration du microservice est gérée via Spring Cloud et GitHub.
Le microservice dispose d'une propriété personnalisée mes-config-ms.commandes-last pour afficher les commandes des derniers jours (par défaut, 10 jours).
La configuration peut être modifiée en utilisant le service Actuator pour charger dynamiquement un nouveau nombre de jours (par exemple, 20 jours).
Le microservice dispose d'une supervision de sa santé. Le statut "UP" est affiché lorsque des commandes existent dans la table "COMMANDE", sinon le statut "DOWN" est affiché.
