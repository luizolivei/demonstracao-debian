# Demonstração: Docker + Debian + Vue.js

Este repositório mostra como subir uma aplicação Vue 3 dentro de um ambiente Debian utilizando Docker (perfeito para apresentar o fluxo com WSL no Windows 11). A aplicação roda em modo de desenvolvimento e fica acessível no navegador pela porta **3000**.

## Requisitos

- [Node.js 20+](https://nodejs.org/) (apenas se desejar rodar sem Docker)
- [Docker](https://docs.docker.com/engine/install/) e [Docker Compose](https://docs.docker.com/compose/install/)

## Executando com Docker

```bash
docker compose up --build
```

Após o build a aplicação ficará disponível em [http://localhost:3000](http://localhost:3000).

Se fizer alterações no código, basta reiniciar o serviço (`Ctrl+C` e `docker compose up --build` novamente) para atualizar o que está no container.

## Execução direta (opcional)

```bash
npm install
npm run dev -- --host
```

O servidor local também usará a porta [http://localhost:3000](http://localhost:3000).

## Build de produção

```bash
npm run build
```

Os arquivos gerados ficarão em `dist/`.
