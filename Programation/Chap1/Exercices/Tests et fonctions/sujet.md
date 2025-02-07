# Exercice : Fonctions et conditions en Python

## Partie 1 : Fonction de parité

On vous donne le programme suivant :

```python
def fnex6(n):
   """............................."""
   if n % 2 == 0:
      reponse = True
   else:
      reponse = False
   return reponse

nombre = int(input("Entrer un entier : "))
if fnex6(nombre) == True:
   print("Le nombre", nombre, "est ....")
```

### Questions :
1) Dans ce programme, on a défini une fonction `fnex6(n)` qui dépend d'un paramètre `n`, puis on appelle cette fonction en passant une valeur entière saisie par l'utilisateur.

   a) Que fait la fonction `fnex6` ? Complétez la **docstring**.
   
   b) Que faut-il écrire à la place des pointillés (`....`) dans l'affichage pour que le programme donne un résultat correct ?

---

## Partie 2 : Calcul du prix en période de soldes

Un magasin applique des réductions sur certains articles :
- Une **pastille verte** indique une réduction de **30%**.
- Une **pastille rouge** indique une réduction de **50%**.

### Questions :
2) 
   a) Écrivez une fonction qui prend en paramètres :
      - Le pourcentage de réduction.
      - Le prix initial.
      
      Cette fonction devra retourner le **prix final** à payer après réduction.

   b) Complétez un programme pour :
      - Demander à l'utilisateur la couleur de la pastille.
      - Demander le prix initial de l'article.
      - Afficher le prix final à payer après réduction.

   c) **Bonus** : Améliorez votre programme pour vérifier si la couleur indiquée est correcte et éviter les erreurs.

---

Bonne chance ! 🚀
