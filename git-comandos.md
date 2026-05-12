# A1.06 PrettyFlights - Fluxo de Trabalho pela Estratégia GitFlow

Configuração e Inicialização

`git config` Configura variáveis de ambiente do Git.
Exemplo: git config --global user.name "Seu Nome"
Exemplo: git config --global user.email "seuemail@exemplo.com"

`git init` Inicia um novo repositório Git em um diretório local existente.
Exemplo: git init
Exemplo: git init meu-projeto

`git clone` Copia um repositório remoto existente para sua máquina local. 
Exemplo: git clone [https://github.com/usuario/repo.git](https://github.com/usuario/repo.git)
Exemplo: git clone [https://github.com/usuario/repo.git](https://github.com/usuario/repo.git) pasta-destino

Fluxo de Trabalho

`git status` Exibe o estado atual do diretório de trabalho.
Exemplo: git status
Exemplo: git status -s

`git commit` Remove arquivos do diretório de trabalho e do índice do Git.
Exemplo: git rm arquivo-velho.txt
Exemplo: git rm -r pasta-desnecessaria/

Branches

`git branch` Lista, cria ou exclui branches.
Exemplo: git branch
Exemplo: git branch nova-funcionalidade

`git checkout` Alterna entre branches ou restaura arquivos no diretório de trabalho.
Exemplo: git checkout main
Exemplo: git checkout -b feature-login

`git merge` Une o histórico de uma branch específica na branch em que você está atualmente.
Exemplo: git merge feature-login
Exemplo: git merge --abort

`git switch` Comando moderno dedicado exclusivamente à troca de branches.
Exemplo: git switch desenvolvimento
Exemplo: git switch -c hotfix-urgente

Repositórios Remotos

`git remote` Gerencia conexões com repositórios remotos.
Exemplo: git remote -v
Exemplo: git remote add origin [https://github.com/user/repo.git](https://github.com/user/repo.git)

`git push` Envia seus commits locais para o repositório remoto.
Exemplo: git push origin main
Exemplo: git push -u origin feature-x

`git pull` Busca as alterações do servidor remoto e as mescla automaticamente na branch atual.
Exemplo: git pull origin main
Exemplo: git pull --rebase origin main

`git fetch` Busca as novidades do repositório remoto, mas não as aplica na sua branch atual.
Exemplo: git fetch origin
Exemplo: git fetch --all

Histórico

`git log` Lista o histórico de commits do projeto.
Exemplo: git log
Exemplo: git log --oneline --graph

`git diff` Mostra a diferença detalhada entre o que foi alterado e o que ainda não foi adicionado ao stage.
Exemplo: git diff
Exemplo: git diff main..feature-x

`git show` Exibe os detalhes de um objeto específico, como um commit ou uma tag.
Exemplo: git show d34f1a2
Exemplo: git show HEAD

Correção

`git reset` Desfaz commits ou remove arquivos do stage, alterando o histórico local.
Exemplo: git reset HEAD~1
Exemplo: git reset --hard origin/main

`git stash` Guarda temporariamente as alterações não finalizadas para que você possa limpar seu diretório sem perder o trabalho.
Exemplo: git stash
Exemplo: git stash pop

Tags

`git tag` Cria pontos de referência específicos no histórico, geralmente usados para marcar versões de lançamento (v1.0, v2.0).
Exemplo: git tag v1.0.0
Exemplo: git tag -a v1.1.0 -m "Versão de produção"

`git clean` Remove arquivos não monitorados (untracked) do seu diretório de trabalho para "limpar" a casa.
Exemplo: git clean -n
Exemplo: git clean -f