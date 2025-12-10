# Ma prédiction - Exercice 18

## Architecture

**Classes présentes :**

- Main → lance le programme
- Banque → représente une banque
- Client → représente un client
- Compte → représente un compte

**Qui contient quoi ?**

- Banque contient : la gestion des clients
- Client contient : la gestion d'un client
- Compte contient : la gestion d'un compte

---

## Traçage de l'exécution

### Création des objets

**Ligne 3 :** `new Banque("MaBanque")`

- Crée une Banque avec clients[] vide

**Lignes 5-6 :** `new Client(...)`

- Alice créé avec un Compte (solde = 0)
- Bob créé avec un Compte (solde = 0)

**Lignes 8-9 :** `ajouterClient(...)`

- clients[0] = alice, nbClients = 1
- clients[1] = bob, nbClients = 2

---

### Dépôts

**Ligne 11 :** `alice.deposer(100)`

- Appelle compte.crediter(100)
- Alice.compte.solde = 100

**Ligne 12 :** `bob.deposer(50)`

- Bob.compte.solde = 50

---

### Affichage initial

```
Alice : 100
Bob : 50

```

---

### Transfert

**Ligne 17 :** `alice.transferer(bob, 30)`

Que se passe-t-il dans transferer() ?

1. `this.retirer(30)` → Alice.compte.solde = 70
2. `destinataire.deposer(30)` → Bob.compte.solde = 80

---

### Affichage après transfert

```
Alice : 70
Bob : 80

```

---

### Total en banque

**Ligne 22 :** `banque.totalDepots()`

- total = 80 + 70 = 150

```

```
