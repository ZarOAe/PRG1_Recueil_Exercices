# Evaluation d'expressions - Opérateurs logiques

Que va afficher le programme C++ suivant ?

~~~cpp
#include <cstdlib>
#include <iostream>
using namespace std;

int main() {

   int i, j, k;

   i = j = k = 1; //i,j,k =1
   i += j += k; //j=2, i =3
   //k=1
   //j=2
   //i=3
   cout << "A : i = " << i << " j = " << j << " k = " << k << endl;

   i = 3; j = 2;
   k = i++ > j || j++ != 3;
   cout << "B : i = " << i << " j = " << j << " k = " << k << endl;
   
   i = 3; j = 2;
   k = i++ < j || j++ != 3;
   cout << "C : i = " << i << " j = " << j << " k = " << k << endl;

   i = 3; j = 2;
   k = ++i == 3 && ++j == 3;
   cout << "D : i = " << i << " j = " << j << " k = " << k << endl;

   i = 3; j = 2;
   k = ++i > 3 && ++j == 3;
   cout << "E : i = " << i << " j = " << j << " k = " << k << endl;
     
   return EXIT_SUCCESS;
}
~~~
A : i = 3 j = 2 k = 1

B : i = 4 j = 2 k = 1 // k = 1 car i(=3)>2, cette condition est vrai, on fait un test booleen sur k = condition || condition, le test va nous retourner 0 si faux, 1 si vrai, le test ici est vrai, donc k = 1, de plus, vu que la première condition est vraie, la 2ème partie de l'expression, n'est pas évaluée, donc la valeur de j, reste a 2

C : i = 4 j = 3 k = 1

D : i = 4 j = 2 k = 0 //La première partie, 4==3, c'est faux, la deuxième partie ne sera pas calculée

E : i = 4 j = 3 k = 1


    

<details>
<summary>Solution</summary>

- A : i = 3 j = 2 k = 1
- B : i = 4 j = 2 k = 1
- C : i = 4 j = 3 k = 1
- D : i = 4 j = 2 k = 0
- E : i = 4 j = 3 k = 1



</details>