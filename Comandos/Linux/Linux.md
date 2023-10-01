### Lista de Comandos do Linux

#### Gerenciamento de Arquivos e Diretórios
  ##### Navegação e Manipulação de Diretórios
  - `cd pasta`: Navega para uma pasta específica.
  - `cd ..`: Retrocede um nível de diretório.
  - `ls`: Lista arquivos e pastas no diretório atual.
  - `mkdir nome_da_pasta`: Cria uma nova pasta.
  - `rmdir nome_da_pasta`: Remove uma pasta vazia.
  - `rm -r nome_da_pasta`: Remove uma pasta e seu conteúdo de forma recursiva.

  ##### Manipulação de Arquivos
  - `cp arquivo_origem arquivo_destino`: Copia um arquivo.
  - `mv arquivo_origem arquivo_destino`: Move ou renomeia um arquivo.
  - `rm arquivo`: Exclui um arquivo.

#### Gerenciamento de Processos
  ##### Gerenciamento de Tarefas
  - `ps`: Lista os processos em execução.
  - `top`: Exibe informações detalhadas sobre os processos em execução.
  - `kill PID`: Encerra um processo com base no seu ID de processo (PID).

  ##### Execução de Programas
  - `./nome_do_programa`: Executa um programa no diretório atual.
  - `sudo comando`: Executa um comando com privilégios de superusuário.

#### Redes e Conectividade
  ##### Rede e IP
  - `ifconfig`: Exibe informações sobre interfaces de rede.
  - `ping endereço_ip`: Testa a conectividade com um endereço IP.

  ##### Conexões de Rede
  - `netstat`: Mostra conexões de rede ativas.
  - `ss`: Mostra informações detalhadas sobre sockets de rede.

#### Gerenciamento de Pacotes
  ##### Pacotes e Repositórios
  - `sudo apt update`: Atualiza a lista de pacotes disponíveis (apenas para sistemas baseados no Debian, como o Ubuntu).
  - `sudo apt upgrade`: Atualiza todos os pacotes instalados (apenas para sistemas baseados no Debian).
  - `sudo apt install pacote`: Instala um pacote (apenas para sistemas baseados no Debian).

#### Contas e Senhas
  ##### Contas de Usuário
  - `sudo adduser nome_de_usuario`: Adiciona um novo usuário.
  - `sudo passwd nome_de_usuario`: Altera a senha de um usuário.

#### Outros Comandos Úteis
- `man comando`: Exibe o manual de um comando específico.
- `df`: Mostra informações sobre o uso de disco.
- `du`: Exibe o tamanho de diretórios e arquivos.
- `grep padrão arquivo`: Procura um padrão em um arquivo.
- `chmod permissões arquivo`: Altera permissões de arquivo.