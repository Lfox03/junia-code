---
title: Les bases en HTML | JuniaCode
description: Page d'accueil de la partie cours de HTML
---

# Cours HTML

Le **HTML** (HyperText Markup Language) est le langage de balisage standard pour créer des pages Web. Il décrit la structure d'une page Web de manière sémantique.

!!! info "Le rôle du HTML"
    Imaginez le HTML comme le **squelette** d'une page web. 
    * **HTML** structure le contenu (titres, paragraphes, images).
    * **CSS** gère l'apparence (couleurs, polices, mise en page).
    * **JavaScript** gère l'interactivité.

## Structure de base

Chaque page HTML suit une structure précise. Voici le modèle minimal requis pour qu'un navigateur comprenne votre page.

=== "Code Source"

    ```html linenums="1" title="index.html"
    <!DOCTYPE html>
    <html lang="fr">
      <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Mon premier site</title>
      </head>
      <body>
        <h1>Bonjour le monde !</h1>
        <p>Ceci est un paragraphe.</p>
      </body>
    </html>
    ```

=== "Détails de la structure"

    * **`<!DOCTYPE html>`** : Indique au navigateur qu'il s'agit d'un document HTML5.
    * **`<html>`** : La racine de la page. L'attribut `lang="fr"` est crucial pour l'accessibilité et le référencement.
    * **`<head>`** : Contient les métadonnées (titre, encodage) qui ne sont pas affichées directement sur la page.
    * **`<body>`** : Contient tout ce qui est visible par l'utilisateur (textes, images, liens).

## Les balises courantes

Le HTML utilise des "tags" (balises) pour définir les éléments. La plupart des balises ont une ouverture `<tag>` et une fermeture `</tag>`.

### 1. Le Texte

Pour structurer votre texte, utilisez les titres et les paragraphes.

| Balise | Description | Exemple d'utilisation |
| :--- | :--- | :--- |
| `<h1>` à `<h6>` | Titres (du plus important au moins important) | Le titre principal de la page |
| `<p>` | Paragraphe | Un bloc de texte standard |
| `<strong>` | Mise en exergue forte (souvent gras) | **Texte important** |
| `<em>` | Emphase (souvent italique) | *Texte accentué* |

### 2. Les Liens et Images

C'est ici que le web prend tout son sens ("HyperText").

!!! tip "Astuce : Accessibilité"
    N'oubliez jamais l'attribut `alt` pour les images. Il décrit l'image pour les personnes malvoyantes utilisant des lecteurs d'écran.

```html title="Exemples de médias"
<a href="[https://www.google.com](https://www.google.com)" target="_blank">Aller sur Google</a>

<img src="chat.jpg" alt="Un chaton mignon qui dort sur un canapé" width="300">
```