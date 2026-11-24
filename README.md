# lassiazyouen.page

Ce dépôt ne porte qu'un renvoi : le site de Youen Lassiaz a déménagé à l'adresse [lassiazyouen.fr.eu.org](https://lassiazyouen.fr.eu.org/). Chaque page de l'ancienne adresse, `lassiazyouen.page`, mène à la même page de la nouvelle, jusqu'à l'expiration de ce nom le 29 décembre 2026 ; le dépôt sera supprimé ensuite.

Le site et son code : [mon-portfolio.v2](https://github.com/Jasonette1/mon-portfolio.v2).

## Fonctionnement

*   GitHub Pages publie le seul dossier `docs/`, sous le domaine `lassiazyouen.page` (`docs/CNAME`) : ni ce README, ni la licence, ni `docs/CNAME` ne sont servis, donc aucune adresse n'échappe au renvoi.
*   `docs/index.html` (l'accueil) et `docs/404.html` (toute autre adresse : GitHub Pages le sert pour chaque page qu'il ne trouve pas) sont identiques, doublon voulu. Un script envoie le visiteur à la même adresse sur `lassiazyouen.fr.eu.org`, chemin, paramètres et ancre compris ; l'origine y est écrite en dur, rien de ce que tape un visiteur ne peut mener ailleurs. Sans script, la page mène à l'accueil du site et montre un lien.
*   Pas de `docs/.nojekyll` : GitHub Pages construit le dossier avec Jekyll, qui recopie les deux pages telles quelles et ne publie pas `CNAME` ; avec `.nojekyll`, `/CNAME` était servi comme un fichier à télécharger.

## Licence

Code sous licence MIT : voir [`LICENSE`](LICENSE).
