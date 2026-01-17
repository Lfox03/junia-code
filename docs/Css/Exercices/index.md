# Exercices Pratiques : HTML & CSS

Mettez vos connaissances à l'épreuve avec ces défis progressifs.

---

## Exercice 1 : La Carte de Profil (HTML Sémantique)

**Objectif :** Créer la structure d'une carte de présentation personnelle en utilisant les balises sémantiques appropriées.

!!! question "Énoncé"
    Réalisez une structure HTML qui contient :
    * Un conteneur principal (`<article>`).
    * Une image de profil.
    * Un titre de niveau 2 pour le nom.
    * Un court paragraphe de biographie.
    * Une liste de liens vers des réseaux sociaux.



??? tip "Indice"
    Pensez à utiliser la balise `<ul>` pour la liste des réseaux sociaux et n'oubliez pas l'attribut `alt` pour l'image !

=== "Code à compléter"

    ```html
    <article class="profile-card">
      <img src="..." alt="...">
      </article>
    ```

=== "Solution"

    ```html linenums="1" title="Solution Exercice 1"
    <article class="profile-card">
      <img src="avatar.jpg" alt="Photo de Jean Dupont">
      <h2>Jean Dupont</h2>
      <p>Développeur Web passionné par le CSS moderne.</p>
      <nav>
        <ul>
          <li><a href="#">LinkedIn</a></li>
          <li><a href="#">GitHub</a></li>
        </ul>
      </nav>
    </article>
    ```

---

## Exercice 2 : Le Modèle de Boîte (CSS)

**Objectif :** Styliser un bouton en utilisant les marges, les bordures et le rembourrage.

!!! question "Défi Style"
    Appliquez les propriétés suivantes à un bouton pour qu'il ressemble à un bouton d'action moderne :
    * Couleur de fond bleue.
    * Texte blanc.
    * Padding de `12px` en haut/bas et `24px` à gauche/droite.
    * Bordure arrondie de `8px`.
    * Supprimer la bordure par défaut.

=== "HTML de base"

    ```html
    <button class="btn-primary">Cliquez ici</button>
    ```

=== "Solution CSS"

    ```css linenums="1" title="style.css"
    .btn-primary {
      background-color: #1976d2;
      color: white;
      padding: 12px 24px;
      border-radius: 8px;
      border: none;
      cursor: pointer;
      font-weight: bold;
      transition: background-color 0.3s;
    }

    .btn-primary:hover {
      background-color: #115293;
    }
    ```

---

## Exercice 3 : Mise en page Flexbox

**Objectif :** Aligner trois boîtes horizontalement et les centrer dans la page.

!!! question "Consignes"
    À partir du code HTML fourni, écrivez le CSS nécessaire pour que les trois boîtes soient :
    1. Alignées sur une seule ligne.
    2. Espacées uniformément.
    3. Centrées verticalement dans leur conteneur.



=== "Structure HTML"

    ```html
    <div class="layout-container">
      <div class="box">A</div>
      <div class="box">B</div>
      <div class="box">C</div>
    </div>
    ```

=== "Solution CSS"

    ```css linenums="1"
    .layout-container {
      display: flex;             /* Active Flexbox */
      justify-content: space-around; /* Espacement uniforme */
      align-items: center;      /* Centrage vertical */
      min-height: 200px;        /* Hauteur pour voir le centrage */
      background-color: #f5f5f5;
    }

    .box {
      background: #ff5252;
      color: white;
      padding: 20px;
      width: 50px;
      text-align: center;
    }
    ```

---

## ✅ Auto-évaluation

Une fois terminé, vérifiez vos points :

* [ ] Mes balises HTML sont-elles bien fermées ?
* [ ] Mon CSS est-il bien lié au fichier HTML ?
* [ ] Est-ce que mon design est lisible sur mobile ?

!!! success "Félicitations"
    Si vous avez réussi ces trois exercices, vous avez les bases nécessaires pour construire des composants web simples et élégants !