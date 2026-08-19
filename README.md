# Pincab OS — Releases

Ce dépôt héberge les versions publiées de **Pincab OS**, utilisées par le système de mise à jour automatisé intégré à l'application.

Il ne contient pas le code source complet du projet — uniquement les binaires compilés (`.exe`) ou les archives (`.zip`) attachés à chaque release, ainsi que leurs notes de version détaillées.

## 📥 Installation Initiale (Le Pack de Base)

Si vous installez Pincab OS pour la toute première fois, voici la marche à suivre :

1. 👉 **[Télécharger le Pack de Base complet (Lien Mega)](https://mega.nz/folder/SZdizYLA#hA2Q0Rxpr4SA9vd9VKglTw)**
2. Extrayez ce dossier sur votre machine (idéalement dans `C:\pincab_os`).

⚠️ **TRÈS IMPORTANT :** Ce pack Mega contient la toute première version de Pincab OS. Elle **n'intègre pas encore le système de mise à jour automatique en ligne**.

Pour bénéficier des mises à jour en un clic par la suite, vous devez effectuer **votre première mise à jour manuellement**. Téléchargez les archives des mises à jour initiales ci-dessous :
* 🔗 **[Mise à jour Setup v1.0.1](https://github.com/Arcadepassion/pincab-os-releases/releases/tag/setup-v1.0.1)**
* 🔗 **[Mise à jour Frontend v1.0.1](https://github.com/Arcadepassion/pincab-os-releases/releases/tag/frontend-v1.0.1)**

*(Note : Vous pouvez également télécharger la toute dernière version disponible depuis l'onglet **Releases**).*

**Ensuite :**
1. Extrayez les archives téléchargées.
2. Remplacez manuellement les anciens fichiers par les nouveaux dans votre dossier `C:\pincab_os`.

Une fois cette opération effectuée, votre système sera à niveau et **toutes les futures mises à jour se feront de manière 100% automatique** directement depuis le Setup !

## ⚙️ Composants et Versioning

Les deux composants principaux sont versionnés **indépendamment** : une mise à jour du Frontend n'implique pas forcément une mise à jour du Setup, et inversement.

| Composant | Préfixe de tag | Fichier(s) attendu(s) dans la Release |
|---|---|---|
| **Setup** | `setup-vX.Y.Z` | Archive `.zip` (recommandé) ou `Pincab Setup.exe` |
| **Frontend** | `frontend-vX.Y.Z` | `Pincab OS.exe` (ou archive `.zip`) |

## 🔄 Comment ça marche (Une fois votre système à jour) ?

L'application Pincab OS interrogera automatiquement l'API GitHub de ce dépôt (`/releases`) lorsque vous cliquerez sur "Mettre à jour" depuis l'onglet **Système & Écrans** du Setup. 

Si une version plus récente est détectée :
1. Vous êtes notifié et pouvez lire les nouveautés.
2. Si vous validez, le téléchargement démarre.
3. Le système télécharge l'archive, extrait les nouveaux fichiers (exécutables, images, traductions) et remplace les anciens de manière totalement autonome et invisible en arrière-plan.
