# Pincab OS — Releases

Ce dépôt héberge les exécutables publiés de **Pincab OS**, utilisés par le
système de mise à jour intégré à l'application (onglet *Système & Écrans*
du Setup).

Il ne contient pas le code source complet du projet — uniquement les
binaires compilés (`.exe`) attachés à chaque release, ainsi que leurs
notes de version.

## Composants

| Composant | Préfixe de tag | Fichier attendu |
|---|---|---|
| Setup | `setup-vX.Y.Z` | `Pincab Setup.exe` |
| Frontend | `frontend-vX.Y.Z` | `Pincab OS.exe` |

Les deux composants sont versionnés **indépendamment** : une mise à jour
du Frontend n'implique pas forcément une mise à jour du Setup, et
inversement.

## Comment ça marche

L'application Pincab OS interroge automatiquement l'API GitHub de ce
dépôt (`/releases`) lorsque l'utilisateur clique sur "Mettre à jour" dans
le Setup. Si une release plus récente est trouvée pour le composant
concerné, l'utilisateur voit les notes de version ci-dessous et peut
choisir d'installer la mise à jour en un clic.

Voici le pack de base à avoir en premier: https://mega.nz/folder/SZdizYLA#hA2Q0Rxpr4SA9vd9VKglTw
