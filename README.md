Site des Régataïdes
===================

- http://regataiades.fr (wwww => redirige vers regataiades.fr)
- http://regataiades.com (wwww => redirige vers regataiades.com)

# Modifications du site en PROD

1. Effectuer les modifications html/css/...
2. Commiter et pusher sur github : `git add . ; git commit -m "..."; git push`
3. Cloudflare déploie les page sur son infra : https://dash.cloudflare.com/62948f54c40e381d1b9e3e8a31319711/pages/view/regataiades

# Hébergement sur Cloudflare

## DNS
La gestion DNS est stocké en automatiquepar Cloudflare
    - regataiades.fr : https://dash.cloudflare.com/62948f54c40e381d1b9e3e8a31319711/regataiades.com/dns/records
    - regataiades.com : https://dash.cloudflare.com/62948f54c40e381d1b9e3e8a31319711/regataiades.com/dns/records

## Pages
Hébergement des pages https://dash.cloudflare.com/62948f54c40e381d1b9e3e8a31319711/pages/view/regataiades

Hébergé sur regataiades-website-2019.pages.dev avec *.regataiades.fr et *.regataiades.com comme alias

## Déploiement
Cloudflare détecte les modifications sur la branche master du dépôt git https://github.com/una-club/regataiades-website-2019 et les déploie sur regataiades-website-2019.pages.dev.

### Configuration
- https://dash.cloudflare.com/62948f54c40e381d1b9e3e8a31319711/pages/view/regataiades/settings/production
- https://github.com/organizations/una-club/settings/installations/59213256


# TODO
- Ajouter de la doc sur comment monter un environement de développement local (sans doute basé sur la même image docker)
- Créer une instance de test (sous-domaine ou sous-répertoire)
