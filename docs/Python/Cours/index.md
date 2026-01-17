# Apprendre Python : Les Bases

Python est un langage de programmation polyvalent, lisible et très puissant. Il est utilisé aussi bien pour le web que pour l'intelligence artificielle.

!!! quote "Philosophie de Python"
    "Beautiful is better than ugly. Explicit is better than implicit. Simple is better than complex." — *The Zen of Python*

---

## 1. Variables et Types de données

En Python, on ne déclare pas le type d'une variable explicitement, c'est le langage qui le devine.

=== "Exemple de code"
    ```python linenums="1" title="variables.py"
    nom = "Alice"          # String (chaîne)
    age = 25               # Integer (entier)
    taille = 1.75          # Float (nombre à virgule)
    est_etudiant = True    # Boolean (booléen)

    print(f"{nom} a {age} ans.")
    ```

=== "Types principaux"
    | Type | Nom Python | Exemple |
    | :--- | :--- | :--- |
    | Texte | `str` | `"Bonjour"` |
    | Entier | `int` | `42` |
    | Décimal | `float` | `3.14` |
    | Booléen | `bool` | `True` / `False` |

---

## 2. Les Structures de Contrôle

### La condition `if`
Python utilise **l'indentation** (4 espaces) pour définir les blocs de code.



```python title="Conditions"
note = 15

if note >= 16:
    print("Très bien")
elif note >= 12:
    print("Bien")
else:
    print("Peut mieux faire")