# Ma prédiction - Exercice 14

## BUG 1 : fonction `moyenne`

**Ligne suspecte :** for (int i = 0; i <= t.length; i++) {

**Description du bug :** le tableau faisant x en taille, i prendra les valeurs de 0 à x or l'index x n'existera jamais

**Ce qui va se passer :** une erreur indiquant que l'index est trop élevé

**Correction proposée :** for (int i = 0; i <= t.length-1; i++) {

---

## BUG 2 : fonction `estTrie`

**Ligne suspecte :** for (int i = 0; i < t.length; i++) {

**Description du bug :** le tableau faisant x en taille, i prendra les valeurs de 0 à x or l'index x n'existera jamais

**Ce qui va se passer :** une erreur indiquant que l'index est trop élevé

**Correction proposée :** for (int i = 0; i < t.length-1; i++) {

---

## BUG 3 : fonction `inverse`

**Ligne suspecte :** for (int i = 0; i < t.length; i++) {

**Description du bug :** On échange les cases de manière symétrique or en parcourant tout le tableau car on rééchange ce qui a déjà été inversé

**Ce qui va se passer :** On ne verra aucune différence car on remet la tableau dans le même ordre qu'au départ

**Correction proposée :** for (int i = 0; i < t.length/2; i++) {

---

## BUG 4 : fonction `compter`

**Ligne suspecte :** return count; de la ligne 59

**Description du bug :** Dès que le programme trouve une occurence, il retourne son nombre (1 par conséquent) or return arrêtant la fonction, la boucle for ne continue pas et le compteur ne peut pas augmenter

**Ce qui va se passer :** Le nombre peut être présent autant de fois qu'on veut, le programme retournera juste 1 s'il est présent

**Correction proposée :** retirer ce return count; à la ligne 59
