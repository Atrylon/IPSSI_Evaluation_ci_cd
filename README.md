Projet : Via un zip
Version de node : 12

Objectif : Mettre en place une CI Travis

A lancer tout le temps via la CI :
    - JsHint => Analyse Statique
    - Retire => Securité
    - Twly => Analyse Statique (Sur la branche master uniquement)

Emplacement des executables : ./node_modules/.bin/

JsHint => Il faut préciser en paramètre l'emplacement du fichier / dossier à analyser
Retire => Aucun paramètre
Twly   => Aucun paramètre

Si vous rencontrez une erreur => Il faut la corriger

Il faut deploy le code présent sur la branche dev sur une application Heroku
Contenu du fichier Procfile :

    `web: node src/server.js`

Ajouter un fichier explication.txt à la racine et m'expliquer comment faire pour bloquer
une pull request vers master sni la CI echoue