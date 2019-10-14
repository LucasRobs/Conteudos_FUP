**A biblioteca math.h**
Fornece um conjunto de funções para operações matemáticas, tais como funções trigonométricas, hiperbólicas, logaritmos, potência e arredondamentos.

Todas as funções da biblioteca math.h retornam um valor do tipo double.

Na tabela abaixo apresentamos algumas funções presentes na biblioteca math.h

Função | Descrição do comando
:---------: | :------:
floor( ) | arredonda para baixo
ceil( ) | arredonda para cima
sqrt( ) | Calcula raiz quadrada
pow(variável, expoente)| potenciação
sin( ) | seno
cos( ) | cosseno
tan( ) | Tangente
log( ) | logaritmo natural
log10( ) | logaritmo base 10

**uso do -lm no gcc**
o -lm que diz para o
gcc incluir a biblioteca libm responsável por funções matemáticas como sqrt, pow, etc

então ao compilar com a biblioteca math use -lh como parametro
