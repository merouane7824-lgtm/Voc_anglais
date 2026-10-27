<p align="center"><img src="icon.svg" width="120" alt="Icône Hello Bébé"></p>

# Hello Bébé

Une petite application web pour parler anglais à son tout-petit au quotidien. Les phrases et le vocabulaire sont classés par moment de la journée, avec la traduction en français et la prononciation audio.

## Contenu

16 thèmes, plus de 200 phrases et autant de mots :

| Moment | Thèmes |
| --- | --- |
| Le matin | Le réveil · Change & habillage |
| La journée | Jeux d'éveil · Mon corps · Les animaux · Couleurs & chiffres · En cuisine · Le ménage · La promenade · Voiture & courses |
| Le soir | Le bain · Sieste & coucher |
| À tout moment | Les repas · Soins & hygiène · Émotions & câlins · Consignes & sécurité |

## Fonctionnalités

- **Audio** : on touche une phrase pour l'entendre (accent américain ou britannique, vitesse normale ou lente). La voix est celle du téléphone.
- **3 phrases du jour**, qui changent chaque matin, et une suggestion de thème selon l'heure.
- **Cartes d'entraînement** : la phrase s'affiche en français, on la dit à voix haute, puis on vérifie en anglais.
- **Favoris** (★) et **phrases maîtrisées** (✓), avec une progression par thème.
- **Recherche** en anglais ou en français.
- **Une astuce par thème** pour savoir comment parler à un bébé (décrire ce qu'on fait, nommer en montrant…).
- Thème clair et sombre, utilisable hors connexion une fois installée.

Les favoris et la progression sont enregistrés dans le navigateur du téléphone, sans compte ni serveur.

## Utilisation

- **En local** : ouvrir `index.html` dans un navigateur.
- **En ligne** : activer GitHub Pages (Settings → Pages → Deploy from a branch → `main` / `root`). L'application sera alors disponible à l'adresse `https://merouane7824-lgtm.github.io/voc_anglais/`.
- **Sur l'écran d'accueil du téléphone** : ouvrir l'adresse en ligne, puis « Ajouter à l'écran d'accueil » (Safari : bouton Partager ; Chrome : menu ⋮). L'icône Hello Bébé apparaît comme une vraie application.

## Fichiers

| Fichier | Rôle |
| --- | --- |
| `index.html` | L'application complète (contenu, style et code dans un seul fichier) |
| `manifest.webmanifest` | Nom, couleurs et icônes pour l'installation sur téléphone |
| `sw.js` | Garde l'application disponible hors connexion |
| `icon.svg`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, `favicon-64.png` | Icônes |

## Ajouter des phrases

Tout le contenu est dans la constante `THEMES` au début du script de `index.html`. Chaque phrase s'écrit `"anglais|français"` :

```js
"Let's play!|On joue !",
```
