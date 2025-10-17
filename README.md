# Avaliação Prática — Sistema de Turmas e Atividades

### Objetivo
Desenvolver um sistema web full-stack para gerenciar turmas e atividades, permitindo que professores autentiquem-se, registrem, consultem e excluam turmas e atividades associadas.

### Contexto
A organização das atividades aplicadas pelos professores é essencial para o acompanhamento do aprendizado e para a gestão do conteúdo já trabalhado. Em muitas escolas de regiões remotas do Brasil, a falta de um sistema acessível prejudica docentes, estudantes e o processo educativo como um todo. Este projeto busca reduzir esse problema com uma solução simples e prática.

### Desafio
Construir uma aplicação que ofereça ao professor as seguintes funcionalidades:
- Autenticação segura;
- Visualização, cadastro e remoção de turmas;
- Registro de atividades vinculadas às turmas;
- Logout seguro.

---

## Requisitos de Infraestrutura

Para executar o projeto localmente, atenda aos requisitos abaixo:

### 1. Banco de Dados
- SGBD: MySQL  
- Versão recomendada: 8.0 ou superior  
- Observação: crie um banco de dados dedicado ao projeto e configure usuário e senha apropriados.

### 2. Ambiente e Servidor
- Sistema operacional: Windows 10/11  
- Runtime: Node.js  
- Versão recomendada do Node.js: 18 ou superior

### 3. Tecnologias
- Back-end: JavaScript (Node.js, Express, Prisma ORM)  
- Front-end: HTML, CSS  
- Banco de dados: MySQL

---

## Instalação e Execução

Siga estes passos para configurar e testar o sistema em sua máquina:

### 1. Clonar o repositório

```bash
git clone https://github.com/LohaineMattos/escola_avaliacao.git
cd escolaavaliacao
```

### 2. Instalar dependências

```bash
npm install
# ou
npm i
```

### 3. Configurar o banco de dados
- Crie um banco MySQL para o projeto.  
- Atualize o arquivo `.env` com a connection string:

```env
DATABASE_URL="mysql://root@localhost:3306/nome_do_banco"
```

### 4. Executar migrations do Prisma

```bash
npx prisma migrate dev --name init
```

### 5. Iniciar o servidor

```bash
npm run dev
```

O servidor ficará disponível em: http://localhost:3001

### 6. Testar a aplicação
- Abra o navegador ou use Insomnia/Postman para testar a API.  
- Funcionalidades a verificar:
	- CRUD de turmas (criar, listar, editar e excluir);
	- CRUD de atividades (criar, listar, editar e excluir);
	- Login e logout de professor.

---

Se quiser, eu posso:
- Gerar um `README.md` já gravado no repositório com esse conteúdo;
- Ajustar o texto para um tom mais técnico, ou mais voltado ao público leigo;
- Incluir seções adicionais (ex.: diagrama da arquitetura, endpoints principais, exemplos de requests).

Qual opção prefere que eu execute a seguir?
