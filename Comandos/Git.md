### Lista de Comandos do Git

#### Configuração Inicial
- `git config --global user.name "Seu Nome"`: Define o nome de usuário globalmente.
- `git config --global user.email "seu_email@example.com"`: Define o endereço de e-mail globalmente.
- `git config --global core.editor "editor_preferido"`: Define o editor de texto preferido.
- `git config --list`: Lista as configurações do Git.

#### Inicialização de Repositório
- `git init`: Inicializa um novo repositório Git local.
- `git clone URL`: Clona um repositório Git remoto para o diretório local.

#### Controle de Alterações
- `git status`: Mostra o status das alterações no repositório.
- `git add arquivo`: Adiciona um arquivo ao índice (staging area).
- `git add .`: Adiciona todas as alterações ao índice.
- `git reset arquivo`: Remove um arquivo do índice.
- `git commit -m "Mensagem do commit"`: Cria um novo commit com as alterações no índice.
- `git commit -a -m "Mensagem do commit"`: Adiciona e faz commit de todas as alterações (ignorando o índice).

#### Histórico e Ramificações
- `git log`: Mostra o histórico de commits.
- `git log --graph --oneline`: Mostra o histórico de commits de forma simplificada e gráfica.
- `git branch`: Lista as ramificações locais.
- `git branch nome_da_ramificacao`: Cria uma nova ramificação.
- `git checkout nome_da_ramificacao`: Muda para uma ramificação existente.
- `git merge nome_da_ramificacao`: Realiza a mesclagem de uma ramificação com a ramificação atual.
- `git remote -v`: Lista os repositórios remotos vinculados.
- `git pull`: Atualiza o repositório local com as alterações do repositório remoto.
- `git push origin nome_da_ramificacao`: Envia uma ramificação local para o repositório remoto.

#### Resolução de Conflitos
- `git diff`: Mostra as diferenças entre os arquivos no diretório de trabalho e o índice.
- `git diff --staged`: Mostra as diferenças entre os arquivos no índice e o último commit.
- `git mergetool`: Abre uma ferramenta de mesclagem configurada para resolver conflitos.
- `git commit -m "Mensagem"`: Conclui a resolução de conflitos com um novo commit.

#### Desfazendo Alterações
- `git checkout -- arquivo`: Descarta as alterações não commitadas em um arquivo.
- `git reset HEAD arquivo`: Remove um arquivo do índice, mas mantém as alterações no diretório de trabalho.
- `git reset --hard HEAD`: Desfaz todas as alterações locais e volta ao último commit.
- `git revert SHA`: Cria um novo commit que reverte as alterações introduzidas por um commit específico.

#### Gerenciamento de Tags
- `git tag nome_da_tag`: Cria uma nova tag para o commit atual.
- `git tag -l`: Lista todas as tags existentes.
- `git push origin nome_da_tag`: Envia uma tag para o repositório remoto.
- `git push --tags`: Envia todas as tags para o repositório remoto.