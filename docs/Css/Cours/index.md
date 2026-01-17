# Apprendre le CSS

Le **CSS** (Cascading Style Sheets) est le langage utilisé pour styliser et mettre en page les documents HTML. Il permet de transformer un document brut en une interface utilisateur attrayante.

!!! abstract "Définition"
    Le CSS définit comment les éléments HTML doivent être affichés à l'écran, sur papier ou dans d'autres médias.

## Syntaxe et Sélecteurs

Une règle CSS se compose d'un **sélecteur** et d'un **bloc de déclaration**.



=== "Exemple de Syntaxe"

    ```css linenums="1" title="style.css"
    h1 {
      color: #2e7d32;
      font-size: 24px;
      text-align: center;
    }
    ```

=== "Explication"

    * **Sélecteur (`h1`)** : Cible l'élément HTML à styliser.
    * **Propriété (`color`)** : L'aspect que vous voulez changer.
    * **Valeur (`#2e7d32`)** : La nouvelle apparence appliquée.
    * **Déclaration** : La paire `propriété: valeur;`.

## Le Modèle de Boîte (Box Model)

C'est l'un des concepts les plus importants du CSS. Chaque élément HTML est considéré comme une boîte rectangulaire.



!!! info "Composants du Box Model"
    1.  **Content** : Le texte ou l'image de l'élément.
    2.  **Padding** : L'espace transparent autour du contenu (à l'intérieur de la bordure).
    3.  **Border** : La bordure qui entoure le padding et le contenu.
    4.  **Margin** : L'espace transparent à l'extérieur de la bordure (espace entre les éléments).

## Méthodes d'intégration

Il existe trois façons d'ajouter du CSS à votre HTML.

| Méthode | Description | Recommandation |
| :--- | :--- | :--- |
| **Externe** | Fichier `.css` séparé lié via `<link>` | ⭐ **Meilleure pratique** |
| **Interne** | Balise `<style>` dans le `<head>` | Pour des tests rapides |
| **En ligne** | Attribut `style="..."` sur une balise | À éviter (difficile à maintenir) |

## Mise en page moderne : Flexbox

Flexbox est un module de mise en page unidimensionnel qui permet de disposer les éléments en colonnes ou en rangées facilement.

=== "Le Code HTML"

    ```html
    <div class="container">
      <div class="item">1</div>
      <div class="item">2</div>
      <div class="item">3</div>
    </div>
    ```

=== "Le Code CSS (Flex)"

    ```css title="Flexbox centering"
    .container {
      display: flex;
      justify-content: center; /* Aligne horizontalement */
      align-items: center;     /* Aligne verticalement */
      gap: 10px;               /* Espace entre les items */
    }
    ```

## Bonnes Pratiques

!!! success "Utiliser des variables CSS"
    Les variables permettent de réutiliser des valeurs (comme les couleurs) sur tout votre site.
    ```css
    :root {
      --primary-color: #3f51b5;
    }
    
    button {
      background-color: var(--primary-color);
    }
    ```

!!! warning "Éviter `!important`"
    L'utilisation de `!important` casse la cascade naturelle du CSS et rend le débogage très difficile. Utilisez plutôt la **spécificité des sélecteurs**.

---

### Questions Fréquentes

??? question "Quelle est la différence entre une classe (`.`) et un ID (`#`) ?"
    * Une **classe** (`.ma-classe`) peut être utilisée sur plusieurs éléments de la même page.
    * Un **ID** (`#mon-id`) doit être unique et ne s'appliquer qu'à un seul élément.
    * *Conseil : Priorisez les classes pour le style.*

??? tip "Outils de développement"
    Faites un clic droit sur n'importe quel élément de votre navigateur et choisissez **Inspecter**. Cela vous permet de tester votre CSS en temps réel !