### Lista de Comandos do Advanced Package Tools (apt)

#### Pesquisa e Listagem
##### Pesquisa
- `apt search pacote`: Procura por um pacote.
- `apt show pacote`: Mostra informações sobre um pacote.
- `apt depends pacote`: Mostra as dependências de um pacote.
- `apt rdepends pacote`: Mostra as dependências recursivas de um pacote.

##### Listagem
- `apt list`: Lista pacotes disponíveis.
- `apt list | grep pacote`: Lista um pacote específico.
- `apt list --installed`: Lista pacotes instalados.
- `apt list --upgradeable`: Lista pacotes que podem ser atualizados.

#### Instalação
- `apt install pacote`: Instala um pacote.
- `apt install pacote1 pacote2`: Instala vários pacotes.
- `apt install /caminho/para/pacote.deb`: Instala um pacote a partir de um arquivo.

#### Atualização
- `apt update`: Atualiza a lista de pacotes disponíveis.
- `apt upgrade`: Atualiza todos os pacotes.
- `apt upgrade pacote`: Atualiza um pacote específico.

#### Remoção
- `apt remove pacote`: Remove um pacote.
- `apt remove pacote1 pacote2`: Remove vários pacotes.
- `apt purge pacote`: Remove um pacote com todos os arquivos.
- `apt autoremove` ou `apt --purge autoremove`: Remove pacotes não utilizados.

#### Marcação
- `apt-mark showhold`: Mostra uma lista de pacotes ignorados.
- `apt-mark hold pacote`: Marca um pacote para ser ignorado em futuras atualizações.
- `apt-mark unhold pacote`: Remove a marcação de um pacote.