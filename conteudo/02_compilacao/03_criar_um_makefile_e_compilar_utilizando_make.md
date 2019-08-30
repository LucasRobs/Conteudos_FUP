**MAKEFILE**

O objetivo de Makefile é definir regras de compilação para projetos de software. Tais regras são definidas em arquivo chamado Makefile. O programa make interpreta o conteúdo do Makefile e executa as regras lá definidas. Alguns Sistemas Operacionais trazem programas similares ao make, tais como gmake, nmake, tmake, etc. O programa make pode variar de um sistema a outro pois não faz parte de nenhuma normalização .

**Como Criar**
- Abra a pasta do seu projeto.
- Abra o terminal integrado com **ctrl + alt + t**
- Crie o arquivo Makefile
```
CC = gcc
CFLAGS = -Wall -std=c99 -g
```

- Compile seu código e execute
```
$ ls
main.c Makefile
$ make main
gcc -Wall -std=c99 -g main.c -o main
$ ./main
hello world
```

[WikiLivros](https://pt.wikibooks.org/wiki/Programar_em_C/Makefiles)