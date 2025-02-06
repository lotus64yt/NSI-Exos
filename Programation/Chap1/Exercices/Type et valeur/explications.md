# Explications détaillées

## Analyse des expressions :

1. `a = 3 + 5.0`
   - `3` est un `int`, `5.0` est un `float`.
   - En Python, un `int` + un `float` donne un `float`.
   - **Valeur :** `8.0` (float).

2. `b = 26 / 4`
   - `/` effectue une division qui retourne toujours un `float`.
   - **Valeur :** `6.5` (float).

3. `c = int(b)`
   - `int()` supprime la partie décimale d'un `float`.
   - **Valeur :** `6` (int).

4. `d = 55 / 5`
   - `/` retourne un `float`, même si la division tombe juste.
   - **Valeur :** `11.0` (float).

5. `e = 87 // 7`
   - `//` effectue une division entière, retournant un `int`.
   - **Valeur :** `12` (int).

6. `f = 8 % 3`
   - `%` retourne le reste de la division `8 / 3`.
   - `8 / 3 = 2` reste `2`.
   - **Valeur :** `2` (int).

7. `g = 2 ** 5`
   - `**` est l'opérateur de puissance.
   - `2 ** 5 = 32`.
   - **Valeur :** `32` (int).

8. `h = 6 + 8 / 2`
   - Priorité : `8 / 2 = 4`, puis `6 + 4 = 10.0`.
   - `+` entre un `int` et un `float` donne un `float`.
   - **Valeur :** `10.0` (float).

---

## Rappel des types de base en Python :
- **`int`** : Nombre entier (ex : `5`, `12`, `-3`).
- **`float`** : Nombre décimal (ex : `3.14`, `2.0`, `-7.5`).
- **`str`** : Chaîne de caractères (ex : `"hello"`, `'Python'`).
- **`bool`** : Valeur booléenne (`True` ou `False`).

## Conclusion :
- Python adapte dynamiquement les types en fonction des opérations.
- La division `/` retourne un `float`, même si le résultat est entier.
- La division `//` retourne un `int`.
- `int()` peut convertir un `float` en `int` en supprimant la partie décimale.