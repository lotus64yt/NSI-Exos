# Réponse : Fonctions et conditions en Python

## Partie 1 : Fonction de parité

```python
def fnex6(n):
   """Retourne True si n est un nombre pair, sinon False."""
   if n % 2 == 0:
      reponse = True
   else:
      reponse = False
   return reponse

nombre = int(input("Entrer un entier : "))
if fnex6(nombre) == True:
   print("Le nombre", nombre, "est pair.")
else:
   print("Le nombre", nombre, "est impair.")
```

### Exemple d'exécution :

```shell
$ python parite.py
Entrer un entier : 4
Le nombre 4 est pair.

$ python parite.py
Entrer un entier : 7
Le nombre 7 est impair.
```

---

## Partie 2 : Calcul du prix en période de soldes

```python
def prix_apres_reduction(pourcentage, prix_initial):
   """Calcule le prix final après réduction."""
   return round(prix_initial * (1 - pourcentage / 100), 2)

# Demande à l'utilisateur la couleur de la pastille
couleur = input("Quelle est la couleur de la pastille (verte/rouge) ? ").lower()

# Vérification de la couleur
if couleur not in ["verte", "rouge"]:
   print("Erreur : couleur invalide.")
else:
   # Demande du prix initial
   prix_initial = float(input("Quel est le prix initial de l'article ? "))

   # Définition de la réduction selon la couleur
   if couleur == "verte":
      reduction = 30
   else:  # couleur == "rouge"
      reduction = 50

   # Calcul et affichage du prix final
   prix_final = prix_apres_reduction(reduction, prix_initial)
   print(f"Le prix final après réduction est de {prix_final}€.")
```

### Exemple d'exécution :

```shell
$ python soldes.py
Quelle est la couleur de la pastille (verte/rouge) ? verte
Quel est le prix initial de l'article ? 100
Le prix final après réduction est de 70.0€.

$ python soldes.py
Quelle est la couleur de la pastille (verte/rouge) ? rouge
Quel est le prix initial de l'article ? 200
Le prix final après réduction est de 100.0€.

$ python soldes.py
Quelle est la couleur de la pastille (verte/rouge) ? bleu
Erreur : couleur invalide.
```