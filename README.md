# Pincab OS — Releases

Ce dépôt héberge les versions publiées de **Pincab OS**, utilisées par le système de mise à jour automatisé intégré à l'application.

Il ne contient pas le code source complet du projet — uniquement les binaires compilés (`.exe`) ou les archives (`.zip`) attachés à chaque release, ainsi que leurs notes de version détaillées.

## 📥 Installation Initiale (Le Pack de Base)

Si vous installez Pincab OS pour la toute première fois, ou si vous découvrez seulement le Frontend et ses configurations, voici la marche à suivre :

1. 👉 **[Télécharger le Pack complet Pincab OS v1.3.0 (Lien Mega)](https://mega.nz/folder/qMs0xAyS#lTSc_4M73SLN1N_Z52gsCw)**
2. Extrayez ce dossier sur votre machine (idéalement dans `C:\pincab_os`).

✅ **Ce pack regroupe tout en une seule fois** : les fichiers de base ET l'ensemble des fichiers de mises à jour successives, déjà intégrés. Il n'est **plus nécessaire de repasser par toutes les mises à jour antérieures publiées sur GitHub** pour arriver à cette version — un seul téléchargement suffit.

Il intègre également **le système de mise à jour automatique en ligne**, prêt à l'emploi dès l'extraction.

➡️ **Une fois ce pack installé, votre système est directement à jour en v1.3.0 et toutes les futures mises à jour se feront de manière 100% automatique** directement depuis le Setup, sans aucune manipulation supplémentaire.

### 🕰️ Vous possédez déjà une ancienne installation (antérieure à v1.0.1) ?

Si vous avez la toute première version de Pincab OS installée **avant la mise en place du système de mise à jour automatique**, et que vous préférez ne pas réinstaller depuis le pack complet ci-dessus, vous pouvez toujours effectuer la mise à jour manuelle initiale via GitHub :

* 🔗 **[Mise à jour Setup v1.0.1](https://github.com/Arcadepassion/pincab-os-releases/releases/tag/setup-v1.0.1)**
* 🔗 **[Mise à jour Frontend v1.0.1](https://github.com/Arcadepassion/pincab-os-releases/releases/tag/frontend-v1.0.1)**

*(Note : vous pouvez également télécharger la toute dernière version disponible depuis l'onglet **Releases**.)*

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
