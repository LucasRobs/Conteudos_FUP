## Compilando programas em C com o GCC

>**Atenção:** este artigo assume que você está usando um sistema do tipo Unix (Linux, Mac OS). Se estiver no Windows, consulte a seção sobre o uso do gcc no Windows para saber o que você deve fazer de diferente.
>
>**Observação importante:** o caractere $ que aparece no início das linhas de comando é apenas uma ilustração do prompt que costuma aparecer no terminal. Você não deve digitá-lo. (No Windows, usamos o caractere > com o mesmo significado.)

Com o gcc já instalado no seu sistema, é muito simples usá-lo para compilar programas em C. Se o programa consistir de um único arquivo, você pode simplesmente executar este comando no terminal:
```
$ gcc prog.c -o prog
```
onde prog.c é o nome do arquivo que contém o código. Os outros dois parâmetros, -o prog, indicam o arquivo de saída do compilador — o arquivo executável que conterá o programa. Você não verá nenhuma mensagem na tela se a compilação ocorrer sem problemas; o compilador diz onde ocorreu o erro e descreve brevemente. Também pode ocorrer do compilador mostrar uma mensagem de **warning** que é um problema que as vezes não impede do programa funcionar, entretanto esse tipo de problema ainda necessita da atenção do programador;

>Dica, você pode criar seus proprios warnings, isso é util quando você quer deixar algum aviso para outros programadores, quando eles forem compilar o codigo a mensagem vai aparecer.
Só basta você colocar da forma abaixo em qualquer linha. 
>
>```#warning "você coloca aqui a msg de aviso."```

Você precisa especificar o nome do arquivo executável de saída pois o padrão, por razões históricas, é usar o arquivo a.out. Em geral, usamos o mesmo nome do arquivo de código, tirando a extensão .c. Veja que, ao contrário do Windows, o Linux não precisa da extensão .exe para reconhecer um arquivo executável; ele utiliza os atributos de permissão do arquivo para saber se ele é executável, dos quais o gcc já cuida automaticamente.

Para executar o programa, a maneira mais “universal” é digitar o seguinte comando no terminal:
```
$ ./prog
```
no qual os caracteres ./ indicam que o programa está no diretório (pasta) atual. É possível também configurar o shell para que não seja necessário fazer essa indicação, imitando o comportamento do Windows (os computadores da Pró-Aluno do IF estão configurados assim). Dessa maneira, você precisaria digitar apenas prog para executar o programa.

Para mudar de pasta no terminal, use o comando cd seguido da pasta para onde você quer ir. Por exemplo, se você salvou seu programa na pasta mac115 dentro da sua pasta pessoal, digite
```
$ cd mac115
```

[fig.if](https://fig.if.usp.br/~esdobay/c/gcc.html)