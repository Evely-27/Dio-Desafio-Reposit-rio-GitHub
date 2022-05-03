# Git e GitHub 

Link Git para baixar:
https://git-scm.com/downloads

### Git Bash: O Git Bash é o aplicativo para ambientes do Microsoft Windows que oferece a camada de emulação para a experiência de linha de comando Git. Bash é acrônico para "Bourne Again Shell". Shells são aplicativos terminais usados como interface em sistemas operacionais por meio de comandos gravados.

# Criando um repositório:

*  Criar uma pasta de fácil acesso.
* Abrir o Git Bash (CLI) na pasta.o
* Pode iniciar o git já na pasta, ou se for um diretório, criar pasta do projeto: git init - irá iniciar o gerenciamento e o versionamento na pasta, criando um repositório. 
* Irá criar uma pasta oculta chamada .git/ : visualizar = ls -a
* Configuração login : git config --global user.email “evelysantos27@gmail.com” ( configura em todo o sistema, se for só nessa pasta tira o “--global”)
* Configurando o user : git config --global user.name Evely-27 
* Criar arquivo de texto md
* Comando para pegar esse arquivo e preparar para comitar: git add * (*= geral)
* Comando para comitar:  git commit -m ‘commit inicial’ ( -m= mensagem curta para explicar e tomar como referência o commit)


# Entendendo os bastidores:

## Processo de modificação dos arquivos

* git status : monitora o status dos arquivos
* OBS: um arquivo .md é exibido de forma diferente, fora de uma pasta é mostrado graficamente.
* Quando o se faz uma modificação depois de um commit e que o git não tinha conhecimento, o git status mostra uma observação. No caso a seguir, apaga o arquivo gelatina e criamos uma pasta receitas, onde o git não tinha conhecimento(git coloca como (UNTRACKED)
* Nessa situação, temos que passar os arquivos untracked(modificados) para  a área de staged( mudanças para serem comitadas) = git add gelatina.md receitas/ 
* Agora se forem os arquivos finais, fixo no momento= git commit -m “ cria pasta receitas, move arquivos para receitas”
* Criar arquivo de index, serve para mostrar o que contém no sistema: mostra o arquivo untracked pois é diferente da última foto(comit) do sistema.
* Mandando pra área de staged: * ou . = todos os arquivos 
# Passando o repositório local para um remoto:

*Para verificar as configurações do repositório local :  git config --list , aperte q para sair

* Entrar no GitHub e criar o repo com o mesmo nome, inicializar com README coloca pra ser a primeira coisa a ser mostrada, se já criamos não precisamos marcar.
* Copiar o url criado (está no push pelo command line) =  git remote add origin linkdesejado  , vai adicionar a origem do repositório remoto < o origin pode ser qualquer nome, é mais convenção>
* Para visualizar os repositórios cadastrados: git remote -v 
* Para push(empurrar) o repositório para remoto :  git push origin(apelido repo) main(branch que estamos trabalhando) . >sempre fazer para enviar as novas alterações para o remoto<.
*Definindo branch de repositório clonada para fazer o push : git branch -M main
*Definindo para  onde será enviado: git push -u origin main

# Resolvendo conflitos:

### Em trabalho em equipe, quando ocorre alterações em mesma linhas ou para pegar as alterações que os outros enviaram, é preciso pull (puxar) esse arquivo do remoto para o local.
* Comando para puxar: git pull origin master ,  vai integrar seu local com o remoto , podendo mostrar as divergências para serem concertadas manualmente.
* Vai mostrar onde estão as alterações diferentes do seu local.
* Depois de modificarmos os arquivos com conflitos, é só preparar para a área de estaged, commitar e depois enviar para o remoto. 

# Clonar repositório:
* Escolher um repo no github ou entro local e pegar o URL do código. 
* Vamos pegar de exemplo o python cpython : https://github.com/python/cpython.git
* Abrir em um diretório geral, porque já vamos pegar uma pasta, exemplo : git clone https://github.com/python/cpython.git 






