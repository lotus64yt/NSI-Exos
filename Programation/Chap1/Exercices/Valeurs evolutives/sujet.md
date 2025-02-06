# Exercice : Suivi de l'évolution des variables

## Objectif
Observer comment les valeurs des variables `x` et `y` évoluent au cours de l'exécution du programme.

### Programme :
```python
x = 8
x = x ** 2
y = x % 3 + x
x = y - x
y = x + y
```

## Consigne :
1) Complétez le tableau ci-dessous avec les valeurs successives de x et y à chaque étape.
2) Identifiez les mises à jour des variables.

|Étape	        | x | y	|   Explication                              |
|---------------|---|---|--------------------------------------------|
|Initialisation	| 8 | - |	x est défini à 8, y n'existe pas encore. |
|x = x ** 2		|   |	|   x devient son carré.                     |
|y = x % 3 + x	|   | 	|   y est calculé à partir de x.             |
|x = y - x		|   |	|   x est mis à jour en fonction de y.       |
|y = x + y		|   |	|   y est mis à jour en fonction de x.       |