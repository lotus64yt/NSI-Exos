
---

### 2. **Correction (`corrige_types_variables.md`)**
```markdown
# Correction : Identifier le type et la valeur des variables

## Réponses

| Variable | Valeur | Type     |
|----------|--------|----------|
| a        | 8.0    | float    |
| b        | 6.5    | float    |
| c        | 6      | int      |
| d        | 11.0   | float    |
| e        | 12     | int      |
| f        | 2      | int      |
| g        | 32     | int      |
| h        | 10.0   | float    |

## Explication
- `+`, `/` et `**` produisent des `float` si au moins un opérande est un `float`.
- `//` force une division entière et retourne un `int`.
- `%` retourne le reste de la division entière.
- `int()` convertit un `float` en `int` en supprimant la partie décimale.