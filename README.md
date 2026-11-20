# lassiazyouen.page

Ce dépôt ne porte qu'un renvoi : le site de Youen Lassiaz a déménagé à l'adresse [lassiazyouen.fr.eu.org](https://lassiazyouen.fr.eu.org/). Chaque page de l'ancienne adresse, `lassiazyouen.page`, mène à la même page de la nouvelle, jusqu'à l'expiration de ce nom le 29 décembre 2026 ; le dépôt sera supprimé ensuite.

Le site et son code : [mon-portfolio.v2](https://github.com/Jasonette1/mon-portfolio.v2).

## Fonctionnement

*   GitHub Pages publie le seul dossier `docs/`, sous le domaine `lassiazyouen.page` (`docs/CNAME`) : ce README et la licence ne sont pas servis, donc aucune adresse n'échappe au renvoi.
*   `docs/index.html` (l'accueil) et `docs/404.html` (toute autre adresse : GitHub Pages le sert pour chaque page qu'il ne trouve pas) sont identiques, doublon voulu. Un script envoie le visiteur à la même adresse sur `lassiazyouen.fr.eu.org`, chemin, paramètres et ancre compris ; l'origine y est écrite en dur, rien de ce que tape un visiteur ne peut mener ailleurs. Sans script, la page mène à l'accueil du site et montre un lien.
*   `docs/.nojekyll` : les fichiers sont servis tels quels.

## Licence

Code sous licence MIT : voir [`LICENSE`](LICENSE).
