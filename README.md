# Formation React 2025

## Exercice 8 - Exercice 8 - react-query : Récupération des users via API
- Lancer la commande `npm install @tanstack/react-query@5.81.5`
- Lancer la commande `npm axios@1.10.0`
- Télécharger le projet [api_backend](https://github.com/Formation-React-2025/api_backend) `git clone https://github.com/Formation-React-2025/api_backend.git`
- Lancer l'API : dans le répertoire `api_backend` lancer les commandes `npm install` puis `npm start`

### 1 - Récupération des users depuis une API
- Dans le package `./src/commons/utils`, télécharger le fichier [Api.utils.js](https://github.com/Formation-React-2025/datas/blob/main/Api.utils.js)
- Dans le package `./src/commons/services/user`, télécharger le fichier [User.service.js](https://github.com/Formation-React-2025/datas/blob/main/User.service.js)

- En utilisant la fonction `getUsers` définie dans `User.service.js`, reprendre l'exercice précédent et utiliser react-query pour charger les users depuis l'API

### 2 - Affichage conditionnel en fonction de l'état d'envoi de la requête
- En fonction de l'état de la requête effectuer les actions suivantes :
  - Si la requête est en cours d'envoi, afficher une message "récupération des utilisateurs ..."
  - Si l'envoi de la requête est terminé, afficher :
    - En cas d'erreur, un message en rouge :
      - soit le message de l'erreur si présent, soit un message par défaut si non présent
    - En cas de succès, afficher le tableau des utilisateurs avec les données chargées.