# Explications du programme

### 1. Demande du nombre de baguettes
```python
quantite = int(input("Combien de baguettes souhaitez-vous acheter ? "))
```
- La fonction `input()` permet de demander une valeur à l'utilisateur.
- `int()` est utilisé pour convertir la réponse de l'utilisateur en entier, car `input()` retourne une chaîne de caractères.

### 2. Définition du prix unitaire
```python
prix_unitaire = 1.13
```
- Une baguette coûte **1,13€**, donc nous stockons cette valeur dans une variable.

### 3. Calcul du prix total
```python
prix_total = round(quantite * prix_unitaire, 2)
```
- La multiplication `quantite * prix_unitaire` donne le prix total.
- La fonction `round(..., 2)` est utilisée pour arrondir le résultat à **deux décimales**.

### 4. Affichage du prix total
```python
print(f"Vous souhaitez acheter {quantite} baguettes.")
print(f"Le prix total à payer est de {prix_total}€.")
```
- `print()` est utilisé pour afficher des messages clairs à l'utilisateur.
- `f"..."` permet d’insérer directement des variables dans la chaîne de caractères.

---

## Pourquoi utiliser `round()` ?
En Python, les calculs en **virgule flottante** peuvent produire des valeurs imprécises.
Exemple sans `round()` :
```python
print(3 * 1.13)  # Affiche 3.3899999999999997 au lieu de 3.39
```
Avec `round()` :
```python
print(round(3 * 1.13, 2))  # Affiche 3.39
```
Cela garantit un affichage correct du prix final.