# Que produit ce code

Déterminer "à la main" ce que va afficher, à l'exécution, le programme ci-dessous.

~~~cpp
#include <cstdlib>
#include <iostream>
using namespace std;

void f(int n) {
   n *= n + 1; // 2 * (2+1)
   cout << "B : n = " << n << endl;
}

int main() { 
   int n = 2;
   cout << "A : n = " << n     << endl;
   f(n);
   cout << "C : n = " << 2 * n << endl;
   return EXIT_SUCCESS;
}
~~~


A: 2
B: 6
C: 4 //vu que n passé en paramètre est une copie, la valeur de n reste inchangée, donc au point C la valeur de n vaut toujours 2



<details>
<summary>Solution</summary>

~~~
A : n=2
B : n=6
C : n=4
~~~

### Explications
La fonction reçoit le paramètre *n* par valeur. Il peut être modifié en interne * n *= n + 1* mais ceci n'a aucun effet sur le paramêtre effectif qui n'est pas modifié. 
</details>
