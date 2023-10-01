### Lista de Comandos do Node.js e npm

#### Gerenciamento de Pacotes (npm - Node Package Manager)

##### Instalação e Gerenciamento de Pacotes
- `npm install | npm i pacote`: Instala um pacote Node.js localmente no projeto.
- `npm install -g pacote`: Instala um pacote globalmente no sistema.
- `npm install --save pacote`: Instala um pacote e o adiciona como dependência no arquivo `package.json`.
- `npm install --save-dev pacote`: Instala um pacote e o adiciona como dependência de desenvolvimento no arquivo `package.json`.

##### Atualização de Pacotes
- `npm update pacote`: Atualiza um pacote específico para a versão mais recente.
- `npm update`: Atualiza todos os pacotes do projeto para suas versões mais recentes, respeitando as restrições de versão definidas no arquivo `package.json`.

##### Remoção de Pacotes
- `npm uninstall | npm un pacote`: Remove um pacote específico do projeto.
- `npm uninstall -g pacote`: Remove um pacote globalmente.
- `npm uninstall --save pacote`: Remove um pacote e suas dependências do arquivo `package.json`.
- `npm uninstall --save-dev pacote`: Remove um pacote de desenvolvimento e suas dependências do arquivo `package.json`.

##### Instalação Automática de Dependências
- `npm install`: Instala todas as dependências listadas no arquivo `package.json`.
- `npm install --only=production`: Instala apenas as dependências de produção (ignora as dependências de desenvolvimento).
- `npm ci`: Realiza uma instalação limpa das dependências, usando o arquivo `package-lock.json` para garantir uma instalação consistente.

##### Outros Comandos
- `npm start`: Inicia um projeto Node.js usando o script "start" definido no arquivo `package.json`.
- `npm test`: Executa testes definidos no arquivo `package.json`.
- `npm run nome_script`: Executa um script personalizado definido no arquivo `package.json`.
- `npm ls`: Lista as dependências instaladas no projeto.
- `npm help`: Exibe a ajuda do npm com informações sobre comandos e opções disponíveis.
- `npm --version`: Exibe a versão do npm instalada.
- `npm init`: Inicializa um novo projeto Node.js e cria um arquivo `package.json` interativamente.