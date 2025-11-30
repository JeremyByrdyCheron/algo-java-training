# Ma prédiction - Exercice 11

## Analyse des fonctions

### Fonction `xxx(int[] t)`

**Que fait cette fonction ?**

- Analyse le code ligne par ligne :
  - r = t[0] → 3
  - Boucle : si t[i] > r alors r = t[i] → 9
  - return r → 9

**En une phrase, cette fonction :** sert à trouver le plus grand nombre d'une liste

**xxx({3, 7, 2, 9, 1, 5}) = 9**

---

### Fonction `yyy(int[] t)`

**Que fait cette fonction ?**

- Analyse :
  - r = 0 → 0
  - Boucle : r = r + t[i] → 3+7+2+9+1+5
  - return r → 27

**En une phrase, cette fonction :** calcule la somme des nombres d'une liste

**yyy({3, 7, 2, 9, 1, 5}) = 27**

---

### Fonction `zzz(int[] t, int v)`

**Que fait cette fonction ?**

- Première boucle : compte les éléments où t[i] < v → 3, 2, 1
- Crée un nouveau tableau de taille c → []
- Deuxième boucle : remplit le tableau avec les éléments < v → [3, 2, 1]

**En une phrase, cette fonction :** cherche dans un tableau les nombres inférieurs à un nombre

**zzz({3, 7, 2, 9, 1, 5}, 4) = {3,2,1}**

---

### Fonction `aaa(int[] t)`

**Que fait cette fonction ?**

- Double boucle imbriquée → \_\_\_
- Compare t[j] et t[j+1], échange si t[j] > t[j+1] →

**En une phrase, cette fonction :** classe dans l'ordre croissant les nombres d'un tableau

**Après aaa({3, 7, 2, 9, 1, 5}) : {1, 2, 3, 5, 7, 9}**
