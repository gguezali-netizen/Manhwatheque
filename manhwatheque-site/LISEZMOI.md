# Manhwathèque : ton site à toi, synchronisé, gratuit

Un site tout simple où tu saisis tes séries à la main. Il est hébergé sur GitHub Pages
et tes séries sont sauvegardées dans un fichier secret (« gist ») de ton compte GitHub.
Plus rien ne dépend de Claude.

## 1. Mettre le site en ligne (5 minutes, une seule fois)

1. Crée un compte sur github.com (gratuit).
2. « New repository » : nom `manhwatheque`, visibilité **Public**
   (GitHub Pages gratuit l'exige), puis « Create repository ».
3. Clique sur « uploading an existing file » et glisse tous les fichiers de ce dossier
   (`index.html`, `manifest.webmanifest`, `icon.svg` et les 3 images `.png`).
   Valide avec « Commit changes ».
4. « Settings » → « Pages » → Source : « Deploy from a branch », branche `main`,
   dossier `/ (root)` → « Save ».
5. Après 1 à 2 minutes, ton site est à `https://TON-PSEUDO.github.io/manhwatheque/`.

Le dépôt public ne contient que le code du site, aucune de tes séries.

## 2. Activer la synchro (une fois par appareil)

1. Sur le site, onglet « Synchro ».
2. Ouvre le lien de création du jeton : l'autorisation « gist » est déjà cochée.
   Choisis « No expiration », puis « Generate token » en bas de page.
3. Copie le jeton (il commence par `ghp_`), colle-le dans le site et clique sur
   « Se connecter ». Un gist secret « Manhwathèque (données) » est créé.
4. Sur ton autre appareil : onglet « Synchro », colle le même jeton. Ou, plus rapide :
   sur le premier appareil, « Copier le lien de connexion », puis ouvre ce lien sur
   l'autre appareil (envoie-le seulement à toi-même).

Ensuite tout est automatique : chaque modification part vers GitHub au bout de
quelques secondes, et chaque appareil récupère les changements à l'ouverture.

## 3. Sur ton téléphone

- iPhone (Safari) : Partager → « Sur l'écran d'accueil ».
- Android (Chrome) : menu ⋮ → « Ajouter à l'écran d'accueil ».

## Récupérer tes séries de la version Claude

Sur la version Claude : « Exporter en JSON » (en bas de page). Sur le nouveau site :
« Importer » et choisis ce fichier. Avec la synchro active, elles arrivent sur tous
tes appareils.

## Ce qu'il faut savoir

- **Le jeton** ne donne accès qu'à tes gists GitHub, pas à tes dépôts. Il reste dans
  le navigateur de chaque appareil. Si tu le perds, crée-en un autre : tes données
  restent dans le gist.
- **Secret ne veut pas dire chiffré.** Un gist secret n'est pas listé, mais toute
  personne qui connaîtrait son adresse pourrait le lire. N'y écris rien de sensible.
- **Deux appareils modifient la même série en même temps :** la modification la plus
  récente gagne. Les séries différentes, elles, sont toutes conservées.
- **Hors ligne :** tes changements sont gardés sur l'appareil et envoyés au retour du
  réseau.
- Pense à « Exporter une sauvegarde » de temps en temps.
