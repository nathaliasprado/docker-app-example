# Docker App Example

Este repositório contém um exemplo de aplicação configurada com Docker, incluindo uso de volumes e `docker-compose`, desenvolvido como parte de um curso de Docker na Alura.

## 🛠️ Tecnologias Utilizadas
- **Docker:** Para criar, gerenciar e executar contêineres.
- **Docker Compose:** Para orquestrar os contêineres necessários.

## 📂 Estrutura do Repositório
- **`app-exemplo/`**: Código da aplicação (HTML, CSS, JS) que é empacotado no contêiner.
- **`node_modules/`**: Dependências do Node.js necessárias para o app.
- **`dockerfile`**: Arquivo de configuração para criar a imagem Docker da aplicação.
- **`index.html`**, **`index.js`**, **`main.css`**: Arquivos da aplicação web.
- **`package.json`**: Define as dependências e scripts da aplicação.
- **`volume-docker/`**: Diretório para testes com volumes no Docker, contendo um arquivo de exemplo.
- **`ymls/`**: Arquivo `docker-compose.yml` para orquestrar os serviços.

## 🚀 Como Utilizar
### Pré-requisitos
1. **Docker** instalado ([guia de instalação](https://docs.docker.com/get-docker/)).
2. **Docker Compose** instalado (geralmente incluso com o Docker Desktop).

### Passos
1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/docker-app-example.git
   cd docker-app-example
   ```
2. Crie a imagem Docker a partir do `dockerfile`:
   ```bash
   docker build -t app-exemplo .
   ```
3. Execute a aplicação com o Docker Compose:
   ```bash
   docker-compose -f ymls/docker-compose.yml up
   ```
4. Acesse a aplicação no navegador, geralmente em `http://localhost:3000` (dependendo da porta configurada).

### Testando Volumes
- O diretório `volume-docker/` é usado para testar a persistência de dados utilizando volumes no Docker.
- Para verificar, acesse os volumes configurados no contêiner.

## 📖 Funcionalidades
- Exemplo de aplicação web simples empacotada em um contêiner Docker.
- Uso de `docker-compose` para orquestrar os serviços.
- Demonstração de volumes para persistência de dados.

## 📚 Origem do Projeto
Este projeto foi desenvolvido como parte do curso **"Docker: criando e gerenciando containers"** da Alura.

## 🤝 Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.
