# Manifeste atria-tools

- GitHub (`github.com/atria-tools`) est le seul serveur : un seul remote `origin`, aucun `mirror`.
- `<remote fetch="../../">` reste relatif : l'URL des projets dérive de celle du manifeste,
  ce qui permet un `island init` en SSH comme en HTTPS.
- Branches : `master` pour la release, `dev` pour le développement et par défaut.
  Un projet sans `dev` (`death`, `qworktree`) est cloné sur sa branche par défaut.
- Le respect de `default-branch` au clonage demande une version d'island plus récente
  que la 1.3.1 publiée : celle-ci clone la branche par défaut du serveur.
