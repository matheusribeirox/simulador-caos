# Simulador do Caos

### Variáveis de Ambiente

**SIGTERM_SECONDS**

Segundos para encerrar a aplicação
# Simulador Caos

Este projeto é um simulador de caos para ambientes de desenvolvimento e testes, focado em práticas de DevOps.

## Estrutura do Projeto

- `compose.yaml`, `docker-compose.yaml`: Arquivos de configuração para orquestração de containers.
- `devcontainer.json`: Configuração para ambiente de desenvolvimento em containers.
- `Dockerfile`, `Dockerfile.dev`: Imagens Docker para produção e desenvolvimento.
- `main.yml`: Workflow de CI/CD (GitHub Actions ou similar).
- `src/`: Código fonte do simulador.
  - `server.ts`: Servidor principal (Node.js/TypeScript).
  - `package.json`: Dependências e scripts do projeto.
  - `tsconfig.json`: Configuração TypeScript.
  - `views/index.ejs`: Template de visualização.

## Como executar

### Requisitos
- Docker
- Node.js (versão recomendada: 18+)

### Passos rápidos

1. **Instale as dependências:**
	```bash
	cd src
	npm install
	```

2. **Execute localmente:**
	```bash
	npm run start
	```

3. **Via Docker Compose:**
	```bash
	docker-compose up --build
	```

4. **Ambiente DevContainer:**
	Use o VS Code com Dev Containers para rodar o ambiente pré-configurado.

## Funcionalidades
- Simulação de falhas e cenários de caos.
- Interface web (EJS).
- Configuração flexível via containers.

## Scripts disponíveis
Veja o `package.json` para scripts como:
- `start`: Inicia o servidor.
- `dev`: Modo desenvolvimento.

## Contribuição
Pull requests são bem-vindos. Para contribuir:
1. Crie uma branch.
2. Faça suas alterações.
3. Envie um PR.

## Licença
Este projeto está sob a licença MIT.

## Autor
Matheus Ribeiro

---
Dúvidas ou sugestões? Abra uma issue!
