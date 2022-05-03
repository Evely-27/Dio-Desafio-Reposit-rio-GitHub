Link Git para baixar:
https://git-scm.com/downloads

-Git Bash: O Git Bash é o aplicativo para ambientes do Microsoft Windows que oferece a camada de emulação para a experiência de linha de comando Git. Bash é acrônico para "Bourne Again Shell". Shells são aplicativos terminais usados como interface em sistemas operacionais por meio de comandos gravados.

Criando um repositório:

Criar uma pasta de fácil acesso.
Abrir o Git Bash (CLI) na pasta.o
Pode iniciar o git já na pasta, ou se for um diretório, criar pasta do projeto: git init - irá iniciar o gerenciamento e o versionamento na pasta, criando um repositório. 
Irá criar uma pasta oculta chamada .git/ : visualizar = ls -a
Configuração login : git config --global user.email “evelysantos27@gmail.com” ( configura em todo o sistema, se for só nessa pasta tira o “--global”)
Configurando o user : git config --global user.name Evely-27 
Criar arquivo de texto md
Comando para pegar esse arquivo e preparar para comitar: git add * (*= geral)
Comando para comitar:  git commit -m ‘commit inicial’ ( -m= mensagem curta para explicar e tomar como referência o commit)

