# Ma prédiction - Exercice 17

## Fonction `moyenneInef`

**Problème identifié :** la boucle j n'est pas utile

**Nombre d'opérations actuelles (pour n éléments) :** n(n+1)/2

**Version optimisée :**
```java
public static double moyenneEff(int[] t) {
    double moyenne= 0;
    int somme = 0;
    for (int i = 0; i < t.length; i++) {
        somme = somme + t[i];
    moyenne = (double) somme / (i + 1);
    }
    return moyenne;
}
```

---

## Fonction `contientDoublonInef`

**Problème identifié :** Les paires sont comparées 2 fois, quand i prend une valeur x, j la prendra aussi

**Version optimisée :**
```java
public static boolean contientDoublonEff(int[] t) {
    for (int i = 0; i < t.length; i++) {
            for (int j = i+1; j < t.length; j++) {
                if (t[i] == t[j]) {
                    return true;
                }
            }
        }
        return false;
}
```

---

## Fonction `premierEtDernierInef`

**Problème identifié :** On réutilise 2 fois une boucle for pour parcourir le même tableau.

**Version optimisée :**
```java
public static String premierEtDernierEff(int[] t) {
    return t[0] + " et " + t[t.length-1];   
}
```

---

## Fonction `rechercheInef`

**Problème identifié :** ne s'arrête qu'une fois le tableau entièrement parcouru, même si la valeur à trouver est la première du tableau

**Version optimisée :**
```java
public static int rechercheEff(int[] t, int val) {
    int index = -1;
    for (int i = 0; i < t.length; i++) {
        if (t[i] == val) {
            return i;
        }
    }
    return index;
}
```
