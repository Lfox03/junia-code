#  Flash Cards : Développement Web

Utilisez ces cartes pour tester vos connaissances. Cliquez sur une carte pour révéler la réponse !

---

##  HTML (Structure)

??? note "Carte 1 : Quel est le rôle de l'attribut `alt` dans une balise `<img>` ?"
    **Réponse :**
    Il fournit une **description textuelle** de l'image. 
    - Il est lu par les lecteurs d'écran pour l'accessibilité.
    - Il s'affiche si l'image ne parvient pas à charger.
    - Il aide au référencement (SEO).

??? note "Carte 2 : Quelle est la différence entre `<ul>` et `<ol>` ?"
    **Réponse :**
    - `<ul>` (Unordered List) : Crée une liste à **puces** (sans ordre précis).
    - `<ol>` (Ordered List) : Crée une liste **numérotée** (étapes chronologiques).

??? note "Carte 3 : Où place-t-on la balise `<title>` d'une page ?"
    **Réponse :**
    À l'intérieur de la section **`<head>`**. Elle définit le nom de l'onglet dans le navigateur.

---

##  CSS (Style)

??? tip "Carte 4 : Quelle est la différence entre `padding` et `margin` ?"
    **Réponse :**
    - **`padding`** : L'espace à l'**intérieur** de l'élément (entre le contenu et la bordure).
    - **`margin`** : L'espace à l'**extérieur** de l'élément (entre la bordure et les autres éléments voisins).

??? tip "Carte 5 : Que signifie la "Cascade" dans CSS ?"
    **Réponse :**
    Elle définit l'ordre de priorité appliqué aux styles. Si deux règles s'opposent, le navigateur choisit en fonction de :
    1. L'origine (style navigateur vs auteur).
    2. La **spécificité** du sélecteur (ex: un ID bat une classe).
    3. L'ordre d'apparition (le dernier écrit gagne).

??? tip "Carte 6 : Comment centrer un élément horizontalement avec Flexbox ?"
    **Réponse :**
    Il faut appliquer `display: flex;` au parent, puis :
    ```css
    justify-content: center;
    ```

---

##  Concepts Avancés

??? abstract "Carte 7 : Qu'est-ce qu'une balise sémantique ?"
    **Réponse :**
    C'est une balise qui donne du **sens** au contenu plutôt que de simplement définir son apparence.
    *Exemples :* `<article>`, `<aside>`, `<nav>`, `<footer>`.
    *Contraire :* `<div>` ou `<span>` qui sont génériques.

---

!!! info "Conseil de révision"
    Révisez 
    
    ![jad](https://avatars.githubusercontent.com/u/9075017?v=4){ width="150" } 