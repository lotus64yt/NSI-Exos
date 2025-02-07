# Réponse : Affichage des entiers de 0 à n

## Code Python

```python
def afficher_entiers(n):
    """Affiche tous les entiers de 0 à n."""
    for i in range(n + 1):
        print(i)

# Exemple d'utilisation
nombre = int(input("Entrez un entier positif : "))
afficher_entiers(nombre)
```

---

## Simulation d'exécution (Shell)

### Exécution 1 :
```shell
$ python affichage_entiers.py
Entrez un entier positif : 5
0
1
2
3
4
5
```

---

### Exécution 2 :
```shell
$ python affichage_entiers.py
Entrez un entier positif : 3
0
1
2
3
```