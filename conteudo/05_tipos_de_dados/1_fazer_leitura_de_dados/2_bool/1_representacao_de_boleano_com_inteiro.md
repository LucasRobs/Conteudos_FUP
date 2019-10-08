**bool (stdbool.h)**

A interface stdbool.h foi introduzida no padrão C99 da linguagem C. Essa interface define a constante inteira

true
com valor 1 e a constante inteira

false
com valor 0.   Também define o tipo booleano

bool
que ocupa 1 byte e pode assumir os valores false e true apenas.

***declarando e manipulando um booleano***

```c
#include <stdbool.h>
int main(){
    bool x = true; //criando e atribuindo true
    x = 0; //0 == false
    x = 1; //1 == true
    x = false;
}
```