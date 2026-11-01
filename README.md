# Pincab OS — Releases

Ce dépôt héberge les versions publiées de **Pincab OS**, utilisées par le système de mise à jour automatique intégré à l'application.

Il ne contient pas le code source complet du projet — uniquement les archives `.zip` attachées à chaque release, ainsi que leurs notes de version détaillées.

---

## 📥 Installation initiale (le Pack complet)

Si vous installez Pincab OS pour la toute première fois, voici la marche à suivre :

👉 **[Télécharger le Pack complet Pincab OS v1.4.0 (lien Mega)](https://mega.nz/file/jY10hJwC#9oUteHOEjhAPu8jhIyYin0OMwV8nVuGxejwsshTAaQ0)**

1. Extrayez l'archive **directement sur `C:\`** : vous obtenez le dossier `C:\pincab_os`.
2. Lancez **`Pincab Setup.exe`** et réglez vos écrans, vos chemins Visual Pinball et vos contrôles, puis cliquez sur **ENREGISTRER**.
3. Lancez **`Pincab OS.exe`** : c'est parti !

Le fichier `LISEZ_MOI_PREMIERE_INSTALLATION.txt` (dans le pack) reprend ces étapes en détail, et l'icône **ⓘ** de chaque onglet du Setup ouvre le mode d'emploi complet (10 langues).

✅ Ce pack regroupe tout en une seule fois : les fichiers de base **et** toutes les mises à jour déjà intégrées. Inutile de repasser par les anciennes releases publiées sur GitHub : un seul téléchargement suffit.

➡️ Une fois ce pack installé, votre système est directement en **v1.4.0** et toutes les futures mises à jour se feront de manière 100 % automatique depuis le Setup.

### Contenu du pack

| Élément | Rôle |
|---|---|
| `Pincab OS.exe` | Le Frontend (le menu du cabinet) |
| `Pincab Setup.exe` | Le Setup (tous les réglages) |
| `pincab_web.exe` | La page de configuration web (téléphone, tablette, autre PC) |
| `pincab_pup_com.exe` | Le serveur PuP PincabOS (PuP packs sans PinUP Player) |
| `pincab_updater.exe` | Le programme de mise à jour |
| `pincab_lang.json` | Les traductions (10 langues) |
| `assets\`, `sounds\` | Icônes, images et sons de l'interface |
| `Wheel de navigation\`, `Medias Pinball FX defaut\` | Médias par défaut des wheels et de Pinball FX |
| `jukebox\` | Musiques du Jukebox (Attract Mode) |
| `vlc64\` | Lecteur vidéo intégré |
| `outils\` | PINemHi (scores) et la tirette Pinball FX |
| `plugins_b2s\`, `plugins_dmd\` | Plugin B2S et DLL DMD du moteur PuP PincabOS |

Votre configuration (`config_systeme.json`) est créée au premier enregistrement dans le Setup, avec une sauvegarde automatique chaque jour dans `C:\pincab_os\sauvegardes`.

---

## 🕰️ Vous avez déjà Pincab OS ?

- **Version 1.0.1 ou plus récente** : rien à télécharger ici. Ouvrez le Setup → onglet **Système & Écrans** → **Mettre à jour le Setup**, puis **Mettre à jour le Frontend**. Vos réglages sont conservés.
- **Toute première version (avant le système de mise à jour automatique)** : le plus simple est d'installer le Pack complet ci-dessus. Pour garder vos réglages, recopiez ensuite votre ancien `config_systeme.json` et votre `pincab_database.json` dans le nouveau dossier `C:\pincab_os`.

---

## ⚙️ Composants et versions

Les deux composants principaux sont versionnés indépendamment : une mise à jour du Frontend n'implique pas forcément une mise à jour du Setup, et inversement.

| Composant | Préfixe de tag | Fichier attendu dans la release |
|---|---|---|
| Setup | `setup-vX.Y.Z` | Archive `.zip` (`Maj.setup.pincab_os.X.Y.Z.zip`) |
| Frontend | `frontend-vX.Y.Z` | Archive `.zip` (`Maj.frontend.pincab_os.X.Y.Z.zip`) |

La mise à jour du Setup installe aussi la page web (`pincab_web.exe`), le serveur PuP (`pincab_pup_com.exe`) et les plugins PuP.

---

## 🔄 Comment ça marche ?

Lorsque vous cliquez sur **« Mettre à jour »** dans l'onglet **Système & Écrans** du Setup, Pincab OS interroge ce dépôt.

Si une version plus récente est détectée :

1. Vous êtes notifié et pouvez lire les nouveautés.
2. Si vous validez, le téléchargement démarre (jauge de progression dans le bouton).
3. L'archive est décompressée et les nouveaux fichiers (programmes, images, sons, traductions) remplacent les anciens dans `C:\pincab_os`, de manière totalement autonome.
4. Les programmes annexes en cours d'exécution (page web, serveur PuP) sont fermés puis relancés automatiquement ; les plugins PuP déjà installés sont mis à jour tout seuls.

🔒 Une mise à jour ne touche **jamais** à vos réglages : configuration, base de tables, scores, sauvegardes, identifiants de la page web et réglages du DMD virtuel restent intacts.

---

## 🔗 Liens

- 🎬 [Chaîne YouTube Arcadepassion](https://www.youtube.com/@Arcadepassion) : présentations et tutoriels
- 📋 [Toutes les releases](https://github.com/Arcadepassion/pincab-os-releases/releases)
