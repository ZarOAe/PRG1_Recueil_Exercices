# Opérations sur le type char

Que va afficher le programme C++ suivant ?

~~~cpp
char x = 'A'; // 65
char y = '0'; // 48
char z;

z = x + 4;
cout << "1. " << z << endl;
cout << "2. " << ++z << endl;

z = x + 0;
cout << "3. " << z << endl;

z = x + '0';
cout << "4. " << z << endl;
~~~

1. E //num 69 table ascii
2. F
3. A
4. q // 65 + 48 =113 table ascii

    

<details>
<summary>Solution</summary>

1. E   
2. F
3. A
4. q
   



</details>
