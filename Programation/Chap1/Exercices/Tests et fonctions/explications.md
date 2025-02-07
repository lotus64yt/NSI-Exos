# Explications : Fonctions et conditions en Python

## Partie 1 : Fonction de parité

```python
def fnex6(n):
   """Retourne True si n est un nombre pair, sinon False."""
   if n % 2 == 0:
      reponse = True
   else:
      reponse = False
   return reponse
```
- `n % 2 == 0` vérifie si `n` est divisible par **2** (donc pair).
- On stocke `True` si `n` est pair, sinon `False`.
- On retourne cette valeur pour être utilisée ailleurs dans le programme.

```python
if fnex6(nombre) == True:
   print("Le nombre", nombre, "est pair.")
else:
   print("Le nombre", nombre, "est impair.")
```
- On appelle `fnex6(nombre)` pour savoir si le nombre est pair ou impair.
- L'affichage est complété avec `"pair"` ou `"impair"`.

---

## Partie 2 : Calcul du prix en période de soldes

### 1. Définition de la fonction

```python
def prix_apres_reduction(pourcentage, prix_initial):
   """Calcule le prix final après réduction."""
   return round(prix_initial * (1 - pourcentage / 100), 2)
```
- `pourcentage / 100` transforme la réduction en un facteur décimal.
- `1 - (réduction en décimal)` donne le coefficient multiplicatif.
- `round(..., 2)` arrondit à **deux décimales** pour un affichage propre.

---

### 2. Vérification de l'entrée utilisateur

```python
couleur = input("Quelle est la couleur de la pastille (verte/rouge) ? ").lower()
if couleur not in ["verte", "rouge"]:
   print("Erreur : couleur invalide.")
```
- `input()` récupère la couleur donnée par l'utilisateur.
- `.lower()` permet d'accepter "Verte", "VERTE", etc.
- On vérifie que la couleur est bien `"verte"` ou `"rouge"`, sinon on affiche une **erreur**.

---

### 3. Calcul et affichage du prix

```python
# Définition de la réduction selon la couleur
if couleur == "verte":
   reduction = 30
else:  # couleur == "rouge"
   reduction = 50

# Calcul et affichage du prix final
prix_final = prix_apres_reduction(reduction, prix_initial)
print(f"Le prix final après réduction est de {prix_final}€.")
```
- On associe chaque couleur à un **taux de réduction**.
- On appelle la fonction `prix_apres_reduction()` pour obtenir le **prix final**.
- `print(f"...")` affiche proprement le résultat.

---

## Pourquoi vérifier la couleur ?
Si l'utilisateur entre une couleur inconnue (`bleu` par exemple), cela éviterait une erreur lors du calcul.

Exemple sans vérification :
```shell
Quelle est la couleur de la pastille (verte/rouge) ? bleu
Traceback (most recent call last):
  File "soldes.py", line 10, in <module>
    if couleur == "verte":
NameError: name 'reduction' is not defined
```
Avec vérification :
```shell
Quelle est la couleur de la pastille (verte/rouge) ? bleu
Erreur : couleur invalide.
```
Cela empêche le programme de **planter** ! ✅

---