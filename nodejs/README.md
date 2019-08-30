Demonstration Digital Contest

Ce dossier contient une démonstration des agents Hyperledger Indy basique. Les agents fournissent une interface de navigateur Web pour montrer l'établissement des relations entre les agents, l'émission de justificatifs d'identité vérifiables et la preuve des demandes à partir de justificatifs d'identité vérifiables.

## Exécuter dans votre navigateur préféré

## Prérequis

Créer un compte sur [Docker Hub](https://hub.docker.com). Docker Hub est le "Play Store" pour l'éco système [Docker](https://docker.com).

## Instaler la démonstration

Rendez vous sur [Play with Docker](https://labs.play-with-docker.com/) et connectez vous si nécessaire.

Cliquez sur le boutton "Start" pour lancer un environement que vous pourrez utiliser pour lancer la démo. Une fois connecté cliquez sur `+Add an Instance` pour ajouter un terminal à votre navigateur. A l'intérieur du terminal lancez les commandes ci-dessous:

- `git clone https://github.com/KiefOx/DigitContest.git`

> **Astuce**: Pour coller du texte dans la fenêtre du terminal, cliquez avec le bouton droit de la souris sur la fenêtre et choisissez `paste` ou faite CTRL+SHIFT+V.

- Naviguez jusqu'à l'emplacement du code en exécutant la commande:
  - `cd DigitContest/education-master/LFS171x/indy-material/nodejs/`


## Commencer la démonstration

- Lancez la commande `chmod +x manage` pour pouvoir exécuter la commande 'manage'
- Lancez la commande `./manage build` pour "construire les composant du logiciel
- Lancez la commande `./manage up` pour lancer les composants

Il faut du temps pour que la démo démarre - beaucoup de choses se passent. Les journaux de tous les conteneurs s'affichent dans la fenêtre du terminal. Les journaux montrent l'édition des nœuds du "ledger" de la chaîne de blocs qui communiquent et des agents Indy qui démarrent et communiquent avec le "ledger".

* Vous devriez voir périodiquement des choses comme "Listening on port 3001", ce qui indique qu'un agent est opérationnel.



### Accéder aux agents:

Au démarrage de la démo, une série de numéros à 4 chiffres apparaîtra au-dessus du terminal. Ce sont les ports exposés des conteneurs en cours d'exécution et les numéros sont des liens pour démarrer un onglet du navigateur.

Cliquez sur les numéros suivants dans la liste pour accéder aux agents:

* **3000** pour Manuia
* **3002** pour Administration
* **3003** pour CCISM

Si vous cliquez sur les liens avant que l'Agent ne soit actif, vous pourriez obtenir un message d'erreur. Attendez plus longtemps, puis réessayez.

Vous pouvez également ouvrir dans un navigateur un Explorateur de Ledger Blockchain.:
* **9000**

> Le reste des numéros (ports - 9701-9708) sont les ports vers les nœuds du Ledger de la chaîne de blocage - deux par nœud.

Pour voir une démonstration, lancez la vidéo situé dans le dossier Démo.

## Arrêter la démo

Pour arrêter la démo, allez dans l'onglet du navigateur où vous avez lancé et fermer la fenêtre. Notez que si vous ne fermez pas l'onglet, la session terminal expirera 4 heures après son démarrage.

Ou utilisez Ctrl-c pour stopper la démo.

# Avertissement

* La "validation" de la "Government-ID" pour chacune des identités échoue souvent - un grand "X" rouge s'affiche.