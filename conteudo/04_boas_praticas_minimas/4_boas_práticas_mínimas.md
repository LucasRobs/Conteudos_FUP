**inicialize todas as variáveis que criar**

Declare as variáveis logo após o título da rotina. Não declare as variáveis “soltas” no meio do código da função.

Organize seu código, sempre declarando as variáveis logo após o título da rotina e em seguida inicialize-as.

****
**Sempre idente corretamente**

O objectivo da indentação é o de tornar os programas mais facilmente legíveis. A utilização de regras de indentação consistentes permite tornar evidente a estrutura global do programa através de uma simples inspecção visual.

 

A ideia geral é a de tornar claramente visíveis todas as instruções compostas (conjunto de instruções entre chavetas) indentando (precedendo de espaços) todas as instruções que as compõem um número fixo de espaços.

 

De seguida são ilustrados os dois estilos de indentação mais frequentes. O número espaços utilizados pode variar entre 2 e 8. Deve escolher o estilo que mais lhe agrada e utilizá-lo de forma uniforme em todos os programas.

**Exemplo eparadas**

Exemplo 1
```c
if (condição)
{
    instruções
}
```
Exemplo 2
```
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
```
for (inicialização; teste; incremento)
{
    instruções
}
```
Exemplo 4
```
while (condição)
{
    instruções
}
```
Exemplo 5
```
do
{
    instruções
}while (condição);
```
Exemplo 6
```
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
```
if (condição){
    instruções
}
```
Exemplo 2
```
if (condição){
    instruções
}else if (condição){
    instruções
}else{
    instruções
}

```
Exemplo 3
```
for (inicialização; teste; incremento){
    instruções
}
```
Exemplo 4
```
while (condição){
    instruções
}
```
Exemplo 5
```
do{
    instruções
}while (condição);
```
Exemplo 6
```
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
*****
**Escolha variáveis e funções com nomes descritivos**

[link](https://dev.to/gabrielcoelho/como-nomear-variveis-5bao)

**Variáveis comuns**

- Utilizo nomes totalmente descritivos, pegando de duas a cinco ou seis palavras para o nome de uma variável.
- sempre começo com letra minúscula, alternando para a primeira letra da próxima palavra maiúscula.
- exemplo: nomeUsuario, estaLogado (isLogged), diaDaSemana, dadosQueryTabela...

**Variáveis Globais**
- Faço o mesmo que as comuns, apenas adicionando a palavra "global" no final
- exemplo: nomeUsuarioGlobal

**Variáveis de loop (For, While)**

- Utilizo apenas um único caractere (normalmente "i", "j", "l").
- Quando há a necessidade de ter uma variável única para aquele loop, palavras pequenas ou abreviadas sobre o que ela faz (normalmente "cont", "adic").

**Variáveis dos Métodos**

- Vejo o que exatamente o método fará e trago uma única palavra que exprima o conteúdo a ser retornado/calculado.
- Exemplo: Se o método faz o calculo da variável externa mais algum valor interno, utilizo "valor" ou "x" mesmo, por se tratar apenas daquele método e não de todo o programa.
  
**Constantes**

- Para constantes, utilizo sempre letras maiúsculas e a separação de frases com um underscore (_).
- Exemplo: EMAIL_CONTATO

****
**Funções devem ter nomes que representam ações**

não existe regra, mas é recomendável seguir um padrão. Mesmo assim, existem diferentes padrões para diferentes contextos que, aliados a diferentes técnicas, permitem um modelo de classes coerente.

- A pergunta que se deva fazer a cada método criado é:
```
Do ponto de vista do código cliente (que chama o método), este nome faz sentido e deixa claro o propósito do método, incluindo seus efeitos colaterais?
```
