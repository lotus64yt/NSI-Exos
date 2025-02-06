
---

# **Correction (`corrige_evolution_variables.md`)**
## Correction : Suivi de l'évolution des variables

### Réponses

Voici l'évolution des variables `x` et `y` à chaque étape :

| Étape | x  | y  | Explication |
|-------|----|----|-------------|
| Initialisation | 8  | -  | `x` est défini à 8, `y` n'existe pas encore. |
| x = x ** 2 | 64 | -  | `x` devient son carré : `8 ** 2 = 64`. |
| y = x % 3 + x | 64 | 65 | `y` est calculé comme `64 % 3 + 64 = 2 + 64 = 65`. |
| x = y - x | 1  | 65 | `x` devient `y - x = 65 - 64 = 1`. |
| y = x + y | 1  | 66 | `y` devient `x + y = 1 + 65 = 66`. |

---
