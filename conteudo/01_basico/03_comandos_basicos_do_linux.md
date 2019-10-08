## Comandos básicos do linux
### sudo
O popular comando sudo ou SuperUserDo é o mais importante que os novatos do Linux farão uso. Cada comando que precisa da permissão de administrador precisa desse comando sudo. Você pode usar o sudo antes de cada comando que requer permissões administrativas.

```shell
ufc@ubunto:~$ sudo su
```
### ls
Outro comando bastante conhecido é o ls, muitas vezes você quer ver qualquer coisa no seu diretório. Com o comando list, o terminal mostrará todos os arquivos e pastas do diretório em que você está trabalhando. Digamos que eu esteja na pasta /home e queira ver os diretórios e arquivos em /home. Basta proceder da seguinte maneira e observar a saída:

```shell
ufc@ubunto:~$ ls
```

### cd
O cd é um dos principais comandos do Linux e você deve realmente aprender . Também é um dos mais usados, pois com ele, podemos navegar entre os diretórios. Usá-lo é bastante simples, basta digitar o nome da pasta que você quer acessar do seu diretório atual. Se você quiser regressar, faça isso usando dois pontos (..) ao invés do nome da pasta.

Digamos que eu esteja no diretório /home e eu queira entrar no diretório /usr que está sempre em /home. Posso usá-lo da seguinte forma:
```shell
ufc@ubunto:~/home$ cd usr
```
```shell
ufc@ubunto:~/home/usr$
```
### mkdir
Geralmente, em algumas ocasioes precisamos criar uma nova pasta ou subpasta. Para isso existe o comando mkdir. Basta dar o nome da sua pasta após o comando mkdir no seu terminal.

```shell
ufc@ubunto:~$ mkdir nome_da_pasta
```
### cp
copiar e colar é a tarefa importante que fazemos diariamente via interface gráfica. O comando cp nos auxiliará na função copiar e colar usando o terminal. Primeiro, você determina o arquivo que deseja copiar e digita o local de destino para colar o arquivo.
```shell
ufc@ubunto:~$ cp nome_do_arquivo local_de_destino
```
Nota: Se você estiver copiando arquivos para o diretório que requer permissão de administrador para qualquer novo arquivo, então você precisará usar o comando sudo.
### rm
O rm é usado para excluir um arquivo ou até mesmo um diretório. Você pode usar a flag -r para fazer uma remoção recursiva e apagar pastas, subpastas entre outros arquivos dentro do diretório.
```shell
ufc@ubunto:~$ rm meu_arquivo.txt
```
ou
```shell
ufc@ubunto:~$ rm -R nome_da_pasta
```
### apt
Este comando se difere entre as inúmeras distribuições. Nas distribuições Linux baseadas em Debian, para instalar, remover e atualizar qualquer pacote usamos o gerenciador de pacotes Advanced Packaging Tool (APT). O comando apt irá ajudá-lo a instalar o software que você precisa para executar no seu Linux. É uma poderosa ferramenta de linha de comando que permite a instalação, atualização e remoção do software.
```shell
ufc@ubunto:~$ sudo apt update
```
### grep
Você precisa encontrar um palavra em um arquivo, mas não sabe como? O grep pode resolver este problema. Com ele você pode localizar palavras-chaves dentro de um arquivo, filtrar a saída de comandos que por natureza podem encher o seu terminal de informações, veja abaixo alguns exemplos:
```shell
ufc@ubunto:~$ grep nome_de_usuario /etc/passwd
```
ou
```shell
ufc@ubunto:~$ history | grep git
```
### cat
Outra função bastante usada é consultar o conteúdo de algum arquivo de texto ou script. Para esse fim, o comando cat é um dos primeiros a ser lembrado. Ele mostrará o texto dentro do um arquivo.
```shell
ufc@ubunto:~$ cat nome_do_arquivo.txt
```
### shutdown
E o último comando é o shutdown. Sua importância é simples e de suma importância, com ele você pode desligar ou reiniciar o computador pelo terminal. Não se esqueça de adicionar o sudo no início do comando, pois ele precisa de permissão especiais para ser executado. Para desligar use a flag -h e para reiniciar use a flag -r.
```shell
ufc@ubunto:~$ sudo shutdown -h now
ufc@ubunto:~$ sudo shutdown -r now
```

[sempreupdate](https://sempreupdate.com.br/10-comandos-basicos-que-todo-iniciante-deve-conhecer/)