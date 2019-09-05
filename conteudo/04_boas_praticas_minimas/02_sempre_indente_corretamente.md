## Sempre idente corretamente

O objectivo da indentação é o de tornar os programas mais facilmente legíveis. A utilização de regras de indentação consistentes permite tornar evidente a estrutura global do programa através de uma simples inspecção visual.

A ideia geral é a de tornar claramente visíveis todas as instruções compostas (conjunto de instruções entre chavetas) indentando (precedendo de espaços) todas as instruções que as compõem um número fixo de espaços.

De seguida são ilustrados os dois estilos de indentação mais frequentes. O número espaços utilizados pode variar entre 2 e 8. Deve escolher o estilo que mais lhe agrada e utilizá-lo de forma uniforme em todos os programas.

**Exemplo esparados**

Exemplo 1
```c
if (condição)
{
    instruções
}
```
Exemplo 2
```c
if (condição)
{
    instruções
}
else if (condição)
{
    instruções
}
else
{
    instruções
}

```
Exemplo 3
```c
for (inicialização; teste; incremento)
{
    instruções
}
```
Exemplo 4
```c
while (condição)
{
    instruções
}
```
Exemplo 5
```c
do
{
    instruções
}while (condição);
```
Exemplo 6
```c
switch (expressão inteira)  
{
    case constante1:
        instruções
    case constante2:
        instruções
    default:
        instruções
}
```
**Exemplo Junto**

Exemplo 1
```c
if (condição){
    instruções
}
```
Exemplo 2
```c
if (condição){
    instruções
}else if (condição){
    instruções
}else{
    instruções
}

```
Exemplo 3
```c
for (inicialização; teste; incremento){
    instruções
}
```
Exemplo 4
```c
while (condição){
    instruções
}
```
Exemplo 5
```c
do{
    instruções
}while (condição);
```
Exemplo 6
```c
switch (expressão inteira){
    case constante1:
        instruções
    case constante2:
        instruções
    default:
        instruções
}
```
[Estilo de Indentação](http://intprogc.pbworks.com/w/page/11211363/Estilo%20Indenta%C3%A7%C3%A3o)