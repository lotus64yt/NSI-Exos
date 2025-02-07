# Explications : Affichage des entiers de 0 à n

## Décomposition du code

### **1. Définition de la fonction**
```python
def afficher_entiers(n):
    """Affiche tous les entiers de 0 à n."""
    for i in range(n + 1):
        print(i)
```
- La fonction `afficher_entiers(n)` prend un **entier positif `n`** en paramètre.
- La **boucle `for`** parcourt les valeurs de **0 à n** grâce à `range(n + 1)`.
- `print(i)` affiche chaque valeur de `i` sur une **nouvelle ligne**.

---

### **2. Interaction avec l'utilisateur**
```python
nombre = int(input("Entrez un entier positif : "))
afficher_entiers(nombre)
```
- `input()` permet à l'utilisateur de **saisir un nombre**.
- `int(input(...))` convertit l'entrée en un **nombre entier**.
- La fonction `afficher_entiers(nombre)` est appelée avec cet entier.

---

## **Pourquoi `range(n + 1)` ?**
- `range(x)` génère une séquence de **0 à x-1**.
- En utilisant `range(n + 1)`, on affiche **jusqu'à `n` inclus**.

### **Exemple avec `range(5)`**
```python
for i in range(5):
    print(i)
```
Sortie :
```
0
1
2
3
4
```
Ici, le `5` n'est **pas inclus** ! On doit donc utiliser `range(n + 1)`.

---

## **Autres façons d'écrire la fonction**
### **Utilisation d'une boucle `while`**
```python
def afficher_entiers(n):
    """Affiche tous les entiers de 0 à n en utilisant une boucle while."""
    i = 0
    while i <= n:
        print(i)
        i += 1
```
Cette version fonctionne **de la même manière**, mais utilise une **boucle `while`** au lieu de `for`.

---

## **Erreurs possibles**
1. **Saisie invalide**  
   ❌ Si l'utilisateur entre un texte (`abc`), l'exécution plantera.  
   ✅ Une solution est de vérifier que l'entrée est un nombre valide.

2. **Nombre négatif**  
   ❌ Si `n` est négatif, la boucle ne s'exécute pas correctement.  
   ✅ On peut ajouter une **vérification** avant d'appeler la fonction :
   ```python
   if nombre >= 0:
       afficher_entiers(nombre)
   else:
       print("Erreur : Veuillez entrer un entier positif.")
   ```

---

## **Conclusion**
Ce programme est un bon exercice sur :
- **Les boucles (`for`, `while`)**
- **Les entrées utilisateur (`input()`)**
- **Les conditions (`if`)**
- **L'affichage avec `print()`**

🚀 **Mission accomplie !** 🎉