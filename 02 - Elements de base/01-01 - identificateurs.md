# Identificateurs (noms des variables) en c++
Pour chacun des cas ci-dessous, indiquez s'il s'agit d'un identificateur C++ légal ou non. Justifiez votre réponse si celle-ci est "Non"

|  #  | Identificateur | Oui / Non | Explication | 
| --- | -------------- | --------- | ----------- |
| 1 | `007` |Non |On ne peut pas commencer par un chiffre | 
| 2 | `james_bond_007`  | oui|Commence par une miniscule comporte des soulignées |
| 3 | `james_bond__007`  |oui |commence par une miniscule comporte des soulignées |
| 4 | `james bond` |non |On ne peut pas mettre des espaces |
| 5 | `sOs` |oui |commence par une miniscule |
| 6 | `SOS` | oui|on peut commencer par une majuscule |
| 7 | `_007` |oui | Commence par un souligné|
| 8 | `__007` |Oui |commence par un souligné |
| 9 | `_007_` | oui|commence par un souligné, comporte des chiffres, qui ne sont pas en premier caractère |
| 10 | `bond-007` | non|comporte un caractère spécial |
| 11 | `tom&jerry` | non|comporte un caractère spécial |
| 12 | `int` |non |C'est un mot réservé |
| 13 | `INT` |non |On ne précise pas le type dans le nom et c'est en majuscule |
| 14 | `André` |non |comporte un caractère spécial |
| 15 | `_` |oui |On peut commencer par un souligné |



<details>
<summary>Solution</summary>

|  #  | Identificateur | Oui / Non | Explication | 
| --- | -------------- | --------- | ----------- |
|1 | `7` | Non | Un identificateur ne peut pas commencer par un chiffre |
|2 | `james_bond_007` | Oui |  |
|3 | `james_bond__007` | Oui | Plusieurs _ peuvent se suivre |
|4 | `james bond` | Non | Pas d'espace dans un identificateur |
|5 | `sOs` | Oui |  |
|6 | `SOS` | Oui | Vu que C++ tient compte de la casse, 5) est un identificateur différent de 6) |
|7 | `_007` | Oui | Un identificateur peut commencer par _ |
|8 | `__007` | Oui |  |
|9 | `_007_` | Oui |  |
|10 | `bond-007` | Non | Le caractère '-' n'est pas autorisé |
|11 | `tom&jerry` | Non | Le caractère '&' n'est pas autorisé |
|12 | `int` | Non | Mot réservé |
|13 | `INT` | Oui | Déconseillé toutefois ! |
|14 | `André` | Non | Les lettres accentuées ne sont pas autorisées |
|15 | `_` | Oui | … mais pas des plus parlants (!) |


</details>