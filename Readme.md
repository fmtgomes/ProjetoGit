Olá, esse projeto ensina a usar o GIT/GitHub

- Criar pasta com nome do projeto
- Abrir com VSC
- Criar arquivo Readme.md (md = extensão markdown, com informações que não ficam dentro no projeto em si)
- Salvar o arquivo (ctrl + s)

Comandos em ordem:<br>
Cmd: git init = no terminal, inicia um repositório vazio<br>
Cmd: git add . = leva todos os arquivos para preparação(steading) antes de comitar. Caso queira só um arquivo > git add Readme.md<br>
Cmd: git status = mostra o estado do repositório, se o mesmo está no branch master, se há arquivos a serem comitados, etc.<br>
Cmd: git commit -m "" = usado para comitar, sendo "-m" a mensagem do título<br>
Cmd: git branch -M "" = muda a branch (master > main)<br>

- No GitHub, criar um repositório novo, pois o git apenas cria no PC. No GitHub serve parar hospedar os arquivos Git. Nome e descrição. Não adicionar nenhuma arquivo para não dar conflito

Cmd: git remote add origin <link gerado no github.git> = Serve para fazer o link do git com github, SÓ É NECESSÁRIO UMA VEZ. Colar com CTRL + SHIFT + V ou INSERT<br>
Cmd: git push -u origin main = "empurra" os arquivos para o github de fato, faz o upload<br>
Cmd: clear = limpar o terminal<br>

----------------------------------

- Criar um novo projeto "ProjetoDeFato.md"<br>
git add . = Adiciona todos os arquivos<br>
git status = Para ver o estado, se estão todos de fato<br>
git commit -m "Criação do Projeto" = Novo commit com título diferente<br>
git push origin main = Não é necessário o "-u" mais.<br>
clear = limpar o terminal<br>

----------------------------------

Criando uma branch nova (exemplo é um botão)<br>
Cmd: git checkout -b "novo-botao"<br>
- Criar novo arquivo "botao.md" e escrever "Aqui desenvolvo o botão"<br>
Cmd: git add .<br>
Cmd: git commit -m "novo botao"<br>
Cmd: git push origin novo-botao<br>
Cmd: git checkout main = Para sair da branch e voltar a main<br>
Cmd: git merge novo-botao = Funde as branchs, faz com que a branch "novo-botao" vá para a branch "main"<br>
Cmd: git push origin main = Para enviar pro GitHub<br>

------------------------------------

Clonar arquivos do GitHub para o PC<br>
- Entrar no repositório, e copiar o link do mesmo<br>
- Criar uma pasta para os arquivos, clicar com botão direito dentro e abrir o Git Bash<br>
Cmd: git clone link.git = Colar o link com CTRL + SHIFT + V<br>
- Caso queria a versão atualizada do arquivo/novo commit:<br>
Cmd: cd gittutorial = Entrar no projeto<br>
Cmd: git pull = "Puxa" da internet, faz download do novo arquivo<br>
- Pode usar o Fork no GitHub caso queira copiar o projeto para seu próprio repositório<br>