**fazer leitura de dados**

A  função scanf()
É utilizada para fazer a leitura de dados formatados via teclado.

Sintaxe:

scanf(“expressão de controle”, lista de argumentos);

Exemplo:

scanf(“%f”, &salario);

Explicação: este comando efetua uma leitura do teclado onde é esperada uma variável float (indicada por “%f”). O valor lido será armazenado no endereço da variável salário.

Na lista de argumentos devemos indicar os endereços das variáveis. Para fazer isso adicionamos o símbolo  “&”  como prefixo na frente do nome da variável.
Limguagem C| Formato | tipo de dados
:--------- | :------: | --------:
char| %c| caracter
int| %d| inteiro
float| %f|ponto flutuante
char[ ]| %s| cadeia de caracteres(string)

[linguagemc](http://linguagemc.com.br/operacoes-de-entrada-e-saida-de-dados-em-linguagem-c/)