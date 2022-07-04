Olá, esse projeto ensina a usar o GIT/GitHub

- Criar pasta com nome do projeto
- Abrir com VSC
- Criar arquivo Readme.md (md = extensão markdown, com informações que não ficam dentro no projeto em si)
- Salvar o arquivo (ctrl + s)

Comandos em ordem:
Cmd: git init = no terminal, inicia um repositório vazio
Cmd: git add . = leva todos os arquivos para preparação(steading) antes de comitar. Caso queira só um arquivo > git add Readme.md
Cmd: git status = mostra o estado do repositório, se o mesmo está no branch master, se há arquivos a serem comitados, etc.
Cmd: git commit -m "" = usado para comitar, sendo "-m" a mensagem do título
Cmd: git branch -M "" = muda a branch (master > main)

- No GitHub, criar um repositório novo, pois o git apenas cria no PC. No GitHub serve parar hospedar os arquivos Git. Nome e descrição. Não adicionar nenhuma arquivo para não dar conflito

Cmd: git remote add origin <link gerado no github.git> = Serve para fazer o link do git com github, SÓ É NECESSÁRIO UMA VEZ. Colar com CTRL + SHIFT + V ou INSERT
Cmd: git push -u origin main = "empurra" os arquivos para o github de fato, faz o upload
Cmd: clear = limpar o terminal

----------------------------------

- Criar um novo projeto "ProjetoDeFato.md"
git add . = Adiciona todos os arquivos
git status = Para ver o estado, se estão todos de fato
git commit -m "Criação do Projeto" = Novo commit com título diferente
git push origin main = Não é necessário o "-u" mais.
clear = limpar o terminal

----------------------------------

Criando uma branch nova (exemplo é um botão)
Cmd: git checkout -b "novo-botao"
- Criar novo arquivo "botao.md" e escrever "Aqui desenvolvo o botão"
Cmd: git add .
Cmd: git commit -m "novo botao"
Cmd: git push origin novo-botao
Cmd: git checkout main = Para sair da branch e voltar a main
Cmd: git merge novo-botao = Funde as branchs, faz com que a branch "novo-botao" vá para a branch "main"
Cmd: git push origin main = Para enviar pro GitHub

------------------------------------

Clonar arquivos do GitHub para o PC
- Entrar no repositório, e copiar o link do mesmo
- Criar uma pasta para os arquivos, clicar com botão direito dentro e abrir o Git Bash
Cmd: git clone link.git = Colar o link com CTRL + SHIFT + V
- Caso queria a versão atualizada do arquivo/novo commit:
Cmd: cd gittutorial = Entrar no projeto
Cmd: git pull = "Puxa" da internet, faz download do novo arquivo
- Pode usar o Fork no GitHub caso queira copiar o projeto para seu próprio repositório