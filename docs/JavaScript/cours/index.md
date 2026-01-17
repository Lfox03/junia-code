---
title: Les bases en JavaScript | JuniaCode
description: Page d'accueil de la partie cours de CSS
---

# JavaScript : Le Langage du Web

Le JavaScript (JS) est un langage de programmation de scripts principalement utilisé pour rendre les pages web interactives. Contrairement au HTML (structure) et au CSS (présentation), le JS gère le **comportement**.

---

## 1. Variables et Constantes

Depuis l'ES6, nous utilisons principalement `let` et `const`.



| Mot-clé | Portée (Scope) | Réassignable | Recommandation |
| :--- | :--- | :--- | :--- |
| `const` | Bloc | Non |  À utiliser par défaut |
| `let` | Bloc | Oui | Si la valeur doit changer |
| `var` | Fonction | Oui |  À éviter (obsolète) |

---

## 2. Les Fonctions

Il existe plusieurs façons de déclarer une fonction en JavaScript.

=== "Fonction Classique"
    ```javascript title="Fonction nommée"
    function saluer(nom) {
        return "Bonjour " + nom;
    }
    ```

=== "Fonction Fléchée (Arrow)"
    ```javascript title="Syntaxe moderne ES6"
    const saluer = (nom) => `Bonjour ${nom}`;
    ```

---

## 3. Le DOM (Document Object Model)

Le DOM est une interface de programmation qui permet au JavaScript d'accéder et de modifier le contenu HTML et les styles CSS.

!!! info "Le concept du DOM"
    Le navigateur transforme votre code HTML en un "arbre" d'objets que le JavaScript peut manipuler.



```javascript title="Manipulation simple"
// Sélection d'un élément
const titre = document.querySelector('h1');

// Modification du contenu et du style
titre.textContent = "Bienvenue en JS !";
titre.style.color = "orange";
```

---

## 4. Les Événements
Le JavaScript "écoute" ce que fait l'utilisateur (clics, touches du clavier, défilement).
```
const bouton = document.querySelector('#monBouton');

bouton.addEventListener('click', () => {
    alert("Vous avez cliqué !");
});
```