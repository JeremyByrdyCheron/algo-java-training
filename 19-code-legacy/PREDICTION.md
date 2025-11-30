# Ma prédiction - Exercice 19

## Partie 1 : Comprendre l'existant

### Classe `Produit`

**Attributs (noms cryptiques) :**

- `n` représente : le nom du produit
- `p` représente : prix du produit à l'unité
- `q` représente : la quantité du produit

**Méthode `valeur()` :**

- Que calcule-t-elle ? la valeur de l'ensemble des exemplaires d'un produit.

---

### Classe `Inventaire`

**Attributs :**

- `prods` représente : l'ensemble des produits
- `nb` représente : le nombre de produits dans le panier

**Méthodes :**

- `ajouter(Produit p)` : ajoute un produit
- `chercher(String nom)` : Cherche si le produit existe ou non
- `afficher()` : affiche les produits présents dans l'inventaire
- `valeurTotale()` : affiche la valeur totale des articles présents dans l'inventaire

---

## Partie 2 : Prédire la sortie actuelle

```

Pomme : 2.5 x 100
Pain : 1.2 x 50
Lait : 0.95 x 75
Beurre : 2.1 x 30

=== Recherche 'Pain' ===
Trouve : Pain a 1.2 euros

=== Valeur totale ===
Valeur : 444.25 euros


```

---

## Partie 3 : Ajouter la fonctionnalité

**Fonctionnalité demandée :**
Ajouter une méthode `afficherCher(double seuil)` qui affiche les produits dont le prix est supérieur au seuil.

**Ma méthode :**

```java
    public void afficherCher(double seuil) {
        for (int i = 0; i < nb; i++) {
            if (prods[i].getPrix() > seuil) {
                System.out.println(prods[i].getNom() + " : " +
                        prods[i].getPrix() + " x " + prods[i].getQuantite());
            }
        }
    }
```

**Sortie attendue pour `afficherCher(2.0)` :**

```
Pomme : 2.5 x 100
Beurre : 2.1 x 30
```
