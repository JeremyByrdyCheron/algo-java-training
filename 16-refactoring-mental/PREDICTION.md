# Ma prédiction - Exercice 16

## Fonction `estPositif`

**Version actuelle :** 5 lignes

**Ma version simplifiée :**

```java
public static boolean estPositif(int n) {
    return n>0?true:false;
}
```

---

## Fonction `valeurAbsolue`

**Version actuelle :** 7 lignes

**Ma version simplifiée :**

```java
public static int valeurAbsolue(int n) {
    n=n<0?n*-1:n;
    return n;

}
```

---

## Fonction `estPair`

**Version actuelle :** 7 lignes

**Ma version simplifiée :**

```java
public static boolean estPair(int n) {
    int reste = n % 2;
    return reste==0?true:false;
}
```

---

## Fonction `max`

**Version actuelle :** 8 lignes

**Ma version simplifiée :**

```java
public static int max(int a, int b) {
    return a>b?a:b;
}
```

---

## Fonction `signe`

**Version actuelle :** 12 lignes

**Ma version simplifiée :**

```java
public static String signe(int n) {
    return n>0?"positif":n<0?"négatif":"zero";
}
```
