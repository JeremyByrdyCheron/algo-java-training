# Ma prédiction - Exercice 15

## Fonction `trouverMax`

```java
int max = ???;      // Trou 1 : 0
for (int i = ???;   // Trou 2 : t.length
    if (t[i] ??? max)  // Trou 3 : >
        max = ???;     // Trou 4 : t[i]
```

**Raisonnement :**

- Trou 1 : 0
- Trou 2 : t.length
- Trou 3 : >
- Trou 4 : t[i]

---

## Fonction `contient`

```java
if (t[i] == val)     // Trou 1 et 2 : t[i] == val
    return true;     // Trou 3 : true
return false;         // Trou 4 : false
```

**Raisonnement :**

- Trous 1-2 : t[i] et val
- Trou 3 : true
- Trou 4 : false

---

## Fonction `sommePairs`

```java
if (t[i] ??? 2 == ???)  // Trou 1 et 2 : % et 0
    somme = somme + ???; // Trou 3 : t[i]
```

**Raisonnement :**

- Trou 1 : %
- Trou 2 : 0
- Trou 3 : t[i]

---

## Fonction `dupliquer`

```java
int[] res = new int[t.length ??? 2];  // Trou 1 : *
res[i ??? 2] = t[i];                   // Trou 2 : *
res[i ??? 2 ??? 1] = t[i];              // Trou 3 et 4 : * et +
```

**Raisonnement :**

- Trou 1 : \*
- Trou 2 : \*
- Trous 3-4 : \* et +
