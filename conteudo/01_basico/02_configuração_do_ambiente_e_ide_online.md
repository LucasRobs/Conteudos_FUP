## Configurar ambiente

- Instalar linux
    - visual studio code
    - sudo apt install build-essential git
- Instalação windows
    - Vscode
        - https://code.visualstudio.com/docs/?dv=win
    - Git for windows
        - https://gitforwindows.org/
    - Mingw
        - https://osdn.net/frs/redir.php?m=c3sl&f=mingw%2F68260%2Fmingw-get-setup.exe

## Instalando o MinGW
- Execute o instalador do Mingw
    - instale no destino padrão C:\MinGW
- Escolha os pacotes
    - mingw-developer-tookit-bin
    - mingw32-gc-g++-bin
- Vá em Instalação
    - Apply Changes
    - Apply
- Espere e tenha fé

## Configurando o MinGW no Path

- Control Panel, Advanced System Settings
- Advanced tab, Environment Variables
- System Variables (no quadrado de baixo, não no de cima)
- Selecione a variável "PATH" (no quadrado de baixo)
- Edit
- Adicione em novas linhas 
    - C:\MinGW\bin
    - C:\MinGW\msys\1.0\bin
- abra um **NOVO** cmd e teste os seguintes comandos
    - bash
    - gcc --version
    - make --version

## Visual Studio Code
- Rode o instalador do vscode.

##### arquivos do sena