# Landing page Cargou Consulting

Page unique, sans framework : `index.html` + `assets/`. Déployable telle quelle sur Vercel (projet statique, aucune commande de build).

## Configuration

Bloc `CONFIG` en bas de `index.html` :

| Clé | Rôle |
|---|---|
| `VIDEO_MP4` | URL directe du MP4 de la VSL (Bunny, Cloudflare Stream…). Prioritaire sur YouTube. |
| `YOUTUBE_ID` | Identifiant YouTube de la VSL, lecture via youtube-nocookie.com. |
| `WEB3FORMS_KEY` | Clé Web3Forms du formulaire. Vide = envoi simulé. |
| `CALENDLY_URL` | Si renseignée, remplace le formulaire par Calendly. |
| `VIDEO_GATE_SECONDS` | 0 = page complète. Ex. 180 = la suite s'affiche après 3 min de vidéo. |

Remplacer le domaine de `og:image` dans le `<head>` par le domaine final.

## Vidéo

Le dossier `video/` (ignoré par Git) contient l'original Frame.io et les encodages web 1080p / 720p. La vidéo doit être hébergée sur un service dédié, pas dans ce dépôt ni sur Vercel.

## Polices

SF Pro Display (police système Apple), Inter en repli via Google Fonts.
