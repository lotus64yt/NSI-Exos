# Réponse : Calcul du prix des baguettes

Voici une solution possible au problème.

```python
# Demande du nombre de baguettes
quantite = int(input("Combien de baguettes souhaitez-vous acheter ? "))

# Prix d'une baguette
prix_unitaire = 1.13

# Calcul du prix total
prix_total = round(quantite * prix_unitaire, 2)

# Affichage du prix total
print(f"Vous souhaitez acheter {quantite} baguettes.")
print(f"Le prix total à payer est de {prix_total}€.")
```

---

## Exemple d'exécution

```shell
$ python baguettes.py
Combien de baguettes souhaitez-vous acheter ? 5
Vous souhaitez acheter 5 baguettes.
Le prix total à payer est de 5.65€.
```

```shell
$ python baguettes.py
Combien de baguettes souhaitez-vous acheter ? 10
Vous souhaitez acheter 10 baguettes.
Le prix total à payer est de 11.3€.
```