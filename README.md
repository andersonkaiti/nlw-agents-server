# NLW Agents

## 🚀 Projeto

NLW Agents é um projeto desenvolvido durante o evento Next Level Week (NLW) da Rocketseat. Trata-se de uma aplicação backend para gerenciamento de salas e agentes.

## 🛠️ Tecnologias Principais

- **Fastify**: Framework web rápido e eficiente para Node.js
- **Drizzle ORM**: ORM leve e tipo-seguro para PostgreSQL
- **Zod**: Biblioteca de validação de esquemas
- **PostgreSQL**: Banco de dados relacional
- **TypeScript**: Linguagem de programação

## 📦 Dependências

- `@fastify/cors`: Gerenciamento de CORS
- `drizzle-orm`: Mapeamento objeto-relacional
- `zod`: Validação de esquemas
- `postgres`: Cliente PostgreSQL

## 🔧 Configuração e Instalação

### Pré-requisitos

- Node.js (versão compatível com o projeto)
- Docker
- Docker Compose

### Passos de Instalação

1. **Clonar o Repositório**

   ```bash
   git clone https://github.com/seu-usuario/nlw-agents-server.git
   cd nlw-agents-server
   ```

2. **Instalar Dependências**

   ```bash
   npm install
   ```

3. **Configurar Variáveis de Ambiente**

   - Crie um arquivo `.env` na raiz do projeto
   - Adicione as configurações necessárias (exemplo):
     ```
     DATABASE_URL=postgresql://docker:docker@localhost:5432/agents
     ```

4. **Iniciar Banco de Dados**

   ```bash
   # Inicia o container do PostgreSQL em segundo plano
   docker-compose up -d
   ```

5. **Credenciais do Banco de Dados**

   - Usuário: `docker`
   - Senha: `docker`
   - Banco de Dados: `agents`
   - Porta: `5432`

6. **Aplicar Migrations**

   ```bash
   npx drizzle-kit migrate
   ```

7. **Popular Banco de Dados (Opcional)**
   ```bash
   npm run db:seed
   ```

**Nota**: Sempre verifique o arquivo `.env` para configurações personalizadas de conexão.

## 🚀 Scripts Disponíveis

- `npm run dev`: Inicia o servidor em modo de desenvolvimento
- `npm start`: Inicia o servidor em produção
- `npm run db:seed`: Popula o banco de dados com dados iniciais

---

Projeto desenvolvido com amor durante o evento Next Level Week (NLW) da Rocketseat. 🚀
