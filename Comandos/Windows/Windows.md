### Lista de Comandos do Windows (Seleção)

#### Gerenciamento de Arquivos e Diretórios
  ##### Navegação e Manipulação de Diretórios
  - `cd pasta`: Navega para uma pasta específica.
  - `cd ..`: Retrocede um nível de diretório.
  - `cd \`: Vai direto para o diretório raiz do sistema.
  - `cd /d caminho_para_pasta`: Acessa diretamente uma pasta específica.
  - `dir`: Lista arquivos e pastas no diretório atual.
  - `mkdir nome_da_pasta`: Cria uma nova pasta.
  - `rmdir /s /q nome_da_pasta`: Remove uma pasta e seu conteúdo de forma recursiva.

  ##### Manipulação de Arquivos
  - `copy arquivo_origem arquivo_destino`: Copia um arquivo.
  - `move arquivo_origem arquivo_destino`: Move um arquivo.
  - `del arquivo`: Exclui um arquivo.
  - `ren arquivo_novo_nome`: Renomeia um arquivo.

#### Gerenciamento de Processos
  ##### Gerenciamento de Tarefas
  - `tasklist`: Lista os processos em execução.
  - `taskkill /F /IM nome_do_processo.exe`: Encerra um processo de forma forçada.

  ##### Execução de Programas
  - `start programa`: Inicia um programa ou arquivo.
  - `shutdown /s /t 0`: Desliga o computador.

#### Redes e Conectividade
  ##### Rede e IP
  - `ipconfig`: Exibe informações sobre configuração de rede.
  - `ping endereço_ip`: Testa a conectividade com um endereço IP.

  ##### Conexões de Rede
  - `netstat`: Mostra conexões de rede ativas.

#### Configurações do Sistema
  ##### Contas e Senhas
  - `net user nome_de_usuario nova_senha`: Altera a senha de um usuário.

  ##### Data e Hora
  - `time`: Exibe ou configura a hora do sistema.
  - `date`: Exibe ou configura a data do sistema.

  ##### Configurações do Sistema
  - `control`: Abre o Painel de Controle do Windows.

#### Outros Comandos Úteis
- `help comando`: Exibe informações de ajuda para um comando específico.
- `systeminfo`: Exibe informações detalhadas sobre o sistema.
- `sfc /scannow`: Verifica e repara arquivos de sistema corrompidos.
- `chkdsk /f`: Verifica e repara erros em unidades de disco.
- `gpupdate /force`: Atualiza as políticas de grupo imediatamente.
- `regedit`: Abre o Editor de Registro do Windows (tenha cuidado ao usá-lo).