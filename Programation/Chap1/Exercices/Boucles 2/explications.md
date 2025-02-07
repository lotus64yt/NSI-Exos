# Explications : Validation d'une réponse "oui" ou "non"

## Décomposition du code

### **1. Utilisation d'une boucle `while`**
```python
while True:
```
- Cette boucle **s'exécute indéfiniment** jusqu'à ce que l'utilisateur entre une réponse valide.

---

### **2. Gestion des entrées utilisateur**
```python
reponse = input("Voulez-vous continuer ? (oui/non) : ").strip().lower()
```
- `input()` permet à l'utilisateur d'entrer une réponse.
- `.strip()` supprime les espaces inutiles avant/après.
- `.lower()` convertit tout en **minuscules** (`"OUI"` devient `"oui"`).

---

### **3. Vérification de la réponse**
```python
if reponse == "oui":
    print('Vous avez répondu "oui". Continuons !')
    break
elif reponse == "non":
    print('Vous avez répondu "non". Arrêt du programme.')
    break
else:
    print('Réponse invalide. Veuillez répondre par "oui" ou "non".')
```
- Si la réponse est `"oui"`, le programme **continue** et quitte la boucle (`break`).
- Si la réponse est `"non"`, le programme **s'arrête**.
- Sinon, un message d'erreur s'affiche et **la question est reposée**.

---

## **Pourquoi utiliser `.lower()` et `.strip()` ?**
### **Sans `.lower()`**
```
Voulez-vous continuer ? (oui/non) : OUI
Réponse invalide. Veuillez répondre par "oui" ou "non".
```
Le programme **ne reconnaîtrait pas** `"OUI"`, d'où la nécessité de `.lower()`.

### **Sans `.strip()`**
```
Voulez-vous continuer ? (oui/non) :   oui  
Réponse invalide. Veuillez répondre par "oui" ou "non".
```
Les **espaces autour** de `"oui"` empêcheraient la reconnaissance de la réponse.

---

## **Erreurs possibles et solutions**
| Erreur | Cause | Solution |
|--------|-------|----------|
| L'utilisateur tape `"OUI"` | Différence de casse | Utiliser `.lower()` |
| L'utilisateur tape `" oui "` | Espaces involontaires | Utiliser `.strip()` |
| L'utilisateur ne tape pas `"oui"` ou `"non"` | Mauvaise saisie | Vérification avec `if` |

---

## **Conclusion**
Ce programme permet de :
- **Gérer les entrées utilisateur**
- **Boucler jusqu'à obtenir une réponse correcte**
- **Afficher un message adapté à la réponse**
- **Éviter les erreurs classiques d'entrée utilisateur**

🚀 **Mission accomplie !** 🎉