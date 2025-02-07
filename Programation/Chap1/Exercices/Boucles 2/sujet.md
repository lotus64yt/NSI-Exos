# Exercice : Validation d'une réponse "oui" ou "non"

## Objectif
Écrire un programme en Python qui :
1. Pose une question à l'utilisateur.
2. Attend une réponse de type **"oui"** ou **"non"**.
3. Redemande la question **tant que** l'utilisateur entre autre chose que "oui" ou "non".
4. Affiche un message cohérent en fonction de la réponse.

## Contraintes
- L'entrée utilisateur ne doit pas être sensible à la casse (`"Oui"`, `"OUI"`, `"oui"` sont considérés comme valides).
- L'affichage doit être clair et structuré.

## Exemple d'exécution attendue

### Exemple 1 :
```
Voulez-vous continuer ? (oui/non) : peut-être
Réponse invalide. Veuillez répondre par "oui" ou "non".
Voulez-vous continuer ? (oui/non) : OUI
Vous avez répondu "oui". Continuons !
```

### Exemple 2 :
```
Voulez-vous continuer ? (oui/non) : d'accord
Réponse invalide. Veuillez répondre par "oui" ou "non".
Voulez-vous continuer ? (oui/non) : non
Vous avez répondu "non". Arrêt du programme.
```

Bonne chance ! 🚀