Site des Régataïdes
===================

- http://regataiades.fr
- http://regataiades.com

# Modifications du site en PROD

1. Effectuer les modifications html/css/...
2. Commiter et pusher : `git add . ; git commit -m "..."; git push`
3. Se connecter en ssh sur le serveur regataiades.fr
4. Se connecter dans le conteneur docker : `sudo docker exec -it regataiades bash`
5. Se rendre dans le répertoire root web : `cd /var/www/regataiades`
6. Mettre à jour le code : `git pull`

# Docker
Voir projet https://github.com/una-club/una-web-entrypoint

# TODO
- Ajouter de la doc sur comment monter un environement de développement local (sans doute basé sur la même image docker)
- Créer une instance de test (sous-domaine ou sous-répertoire)
