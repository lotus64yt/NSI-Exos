# Réponse : Validation d'une réponse "oui" ou "non"

## Code Python

```python
def demander_confirmation():
    """Demande une réponse 'oui' ou 'non' à l'utilisateur jusqu'à ce qu'il réponde correctement."""
    while True:
        reponse = input("Voulez-vous continuer ? (oui/non) : ").strip().lower()
        if reponse == "oui":
            print('Vous avez répondu "oui". Continuons !')
            break
        elif reponse == "non":
            print('Vous avez répondu "non". Arrêt du programme.')
            break
        else:
            print('Réponse invalide. Veuillez répondre par "oui" ou "non".')

# Exécution du programme
demander_confirmation()
```

---

## Simulation d'exécution (Shell)

### Exécution 1 :
```shell
$ python confirmation.py
Voulez-vous continuer ? (oui/non) : peut-être
Réponse invalide. Veuillez répondre par "oui" ou "non".
Voulez-vous continuer ? (oui/non) : oui
Vous avez répondu "oui". Continuons !
```

---

### Exécution 2 :
```shell
$ python confirmation.py
Voulez-vous continuer ? (oui/non) : d'accord
Réponse invalide. Veuillez répondre par "oui" ou "non".
Voulez-vous continuer ? (oui/non) : NON
Vous avez répondu "non". Arrêt du programme.
```