# Modulo

Soient les déclarations suivantes :

~~~cpp
int i = 5, j = 11, n = 10;
double x = 5, y = 11;
~~~

Quel est le résultat d'évaluation des expressions suivantes ?\
En cas d'erreur, indiquez la raison.\
**NB** : les questions sont indépendantes les unes des autres.

| # | Expression | Résultat |
|---| ---------- |---|
| 1 | `j % i` | 1 |
| 2 | `n % i`  | 0|
| 3 | `y % x`  | Erreur, le modulo ne marche qu'avec des entiers|
| 4 | `y % i` | Erreur le modulo ne marche qu'avec des entiers|
| 5 | `-j % i` | -1|
| 6 | `n % ++i` |4 |
| 7 | `n++ % ++i` |4 | Le n++, n'est effectué qu'après le calcul, donc on a 10%6, ce qui est égal a 4, n est ensuite incrémenté et devient 11.


    

<details>
<summary>Solution</summary>

| # | Expression | Résultat |
|---| ---------- |---|
| 1 | `j % i` | 1 |
| 2 | `n % i`  | 0 |
| 3 | `y % x`  | Erreur, le modulo n'est pas défini pour les réels |
| 4 | `y % i` | Erreur, le modulo n'est pas défini pour les réels |
| 5 | `-j % i` | -1 |
| 6 | `n % ++i` | 4 |
| 7 | `n++ % ++i` | 4 |


</details>
