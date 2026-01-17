#  Flash Cards : Maîtriser Python

Testez vos connaissances sur le langage Python. Cliquez sur chaque carte pour voir la réponse.

---

##  Syntaxe et Concepts de Base

??? note "Carte 1 : Quelle est la différence entre une liste `[]` et un tuple `()` ?"
    **Réponse :**
    - La **liste** est **mutable** (on peut modifier, ajouter ou supprimer des éléments après sa création).
    - Le **tuple** est **immuable** (une fois créé, son contenu ne peut plus être changé).
    - *Usage :* Les tuples sont souvent plus rapides et sécurisent les données qui ne doivent pas changer.

??? note "Carte 2 : Qu'est-ce que la PEP 8 ?"
    **Réponse :**
    C'est le **guide de style** officiel pour le code Python. 
    Il recommande par exemple :
    - 4 espaces pour l'indentation.
    - Des noms de variables en `snake_case`.
    - Des lignes de maximum 79 caractères.

??? note "Carte 3 : Que fait l'opérateur `//` ?"
    **Réponse :**
    C'est l'opérateur de **division entière**. Il renvoie le quotient de la division sans la partie décimale.
    ```python
    print(7 // 2)  # Affiche 3 (et non 3.5)
    ```

---

##  Structures de Données

??? tip "Carte 4 : Qu'est-ce qu'une 'List Comprehension' ?"
    **Réponse :**
    C'est une syntaxe concise pour créer des listes à partir d'itérables.
    ```python
    # Au lieu de :
    carres = []
    for x in range(5):
        carres.append(x**2)
        
    # On écrit :
    carres = [x**2 for x in range(5)]
    ```

??? tip "Carte 5 : Quelle est la particularité des clés d'un dictionnaire (`dict`) ?"
    **Réponse :**
    - Elles doivent être **uniques**.
    - Elles doivent être de type **immuable** (comme une chaîne, un nombre ou un tuple). On ne peut pas utiliser une liste comme clé.

---

##  Fonctions et Logique

??? abstract "Carte 6 : À quoi sert le mot-clé `lambda` ?"
    **Réponse :**
    Il sert à créer des **fonctions anonymes** (fonctions sans nom) sur une seule ligne.
    ```python
    multiplier_par_deux = lambda x: x * 2
    print(multiplier_par_deux(5)) # 10
    ```

??? abstract "Carte 7 : Quelle est la différence entre `range(5)` et `list(range(5))` ?"
    **Réponse :**
    - `range(5)` est un **générateur** (objet itérable) qui produit les nombres à la demande pour économiser de la mémoire.
    - `list(range(5))` convertit ce générateur en une véritable **liste** en mémoire : `[0, 1, 2, 3, 4]`.

??? abstract "Carte 8 : Que signifie `*args` dans la définition d'une fonction ?"
    **Réponse :**
    Cela permet à une fonction de recevoir un **nombre variable d'arguments** positionnels sous forme de tuple.
    ```python
    def ma_fonction(*args):
        for arg in args:
            print(arg)
    ```

---

!!! success "Méthode de révision"
    Pour une efficacité maximale, essayez d'expliquer la réponse à haute voix avant de cliquer. Si vous vous trompez, revenez sur cette carte dans 10 minutes !