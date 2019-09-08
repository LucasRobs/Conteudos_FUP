## Parametros úteis do GCC

>-Wall 
>ativa vários avisos que não são ativados normalmente. Pode dar alguns conselhos úteis.
>ex: ```gcc -Wall -o prog prog.c```

>-ansi
>compila seu programa estritamente de acordo com o padrão ANSI, desativando qualquer extensão específica do gcc. Tenha cuidado com essa opção pois até mesmo os comentarios com // vão produzir erros.
>ex: ```gcc -Wall -o prog prog.c```

>-lm Se o programa emprega funções da biblioteca de matemática #include <math.h>, então esta biblioteca deve ser indicada na linha de comando.prompt: ```gcc prog.o -lm -o prog```
Note a forma abreviada para nominar a biblioteca: -lm indica que a
biblioteca  libm.a  deve ser usada, e esta pode ser
encontrada num dos diretórios normalmente buscados pelo compilador
(/lib e /usr/lib no linux).

>-std=<versão> com essa opção você diz ao gcc qual pradrão do C será adotado, com isso algumas características adicionadas ficam disponiveis. Você pode usar uma versão mais antiga do C, entretanto algumas construções como por exemplo o "for" ficará indisponivel, pois ele so foi adicionado apartir da C99. Ex: `gcc -std=c99 -o prog prog.c`

O gcc pode otimizar o seu programa de modo a aumentar seu desempenho e/ou diminuir o tamanho do código de máquina gerado. Por omissão, o gcc não realiza nenhuma otimização. Há três níveis de otimização: 1, 2 e 3. Quanto maior o nível, maior deve ser a melhora no desempenho; mas também deve ser maior o tempo de compilação.

Para ativar a otimização, use as opções -O1, -O2 ou -O3 (a letra O, não o número zero), de acordo com o nível de otimização que você desejar. Também existe a opção -Os, que realiza as mesmas otimizações de -O2, excetuando as que costumam aumentar o tamanho do executável gerado.

