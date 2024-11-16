# Desafio 01 - Fundamentos do Node.js

Repositório do primeiro desafio da trilha de **Node.js** do **Ignite**! Este projeto é uma API que implementa um CRUD para gerenciamento de tarefas (*tasks*) e a funcionalidade de importação de dados em massa a partir de arquivos CSV.

## 🚀 Funcionalidades

### Estrutura de uma Task
Cada tarefa contém as seguintes propriedades:
- **id**: Identificador único.
- **title**: Título da tarefa.
- **description**: Descrição detalhada.
- **completed_at**: Data de conclusão (*null* inicialmente).
- **created_at**: Data de criação.
- **updated_at**: Data de última atualização.

### Rotas Implementadas
1. **`POST /tasks`**  
   - Criação de uma nova tarefa com os campos `title` e `description`.
   - Os campos `id`, `created_at`, `updated_at` e `completed_at` são gerados automaticamente.

2. **`GET /tasks`**  
   - Listagem de todas as tarefas.
   - Suporte à filtragem por `title` ou `description`.

3. **`PUT /tasks/:id`**  
   - Atualização de uma tarefa pelo `id`.
   - Permite alterar somente o `title` e/ou `description`.

4. **`DELETE /tasks/:id`**  
   - Remoção de uma tarefa específica pelo `id`.

5. **`PATCH /tasks/:id/complete`**  
   - Alterna o estado de conclusão de uma tarefa. Se concluída, volta ao estado não concluído e vice-versa.

6. **Importação de Tasks via CSV**  
   - Importa várias tarefas de um arquivo CSV.
   - Utiliza *streams* para processar o arquivo eficientemente.

## 🛠 Tecnologias Utilizadas

- **Node.js**
- **Express**: Framework para criação da API.
- **Streams**: Manipulação eficiente de arquivos CSV.
- **UUID**: Geração de identificadores únicos.
- **fs**: Manipulação de arquivos.

## 📦 Como Executar o Projeto

### Pré-requisitos
- Node.js (versão 16 ou superior)
- Gerenciador de pacotes (NPM ou Yarn)

### Passo a Passo
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/desafio-01-fundamentos-nodejs.git](https://github.com/AlexandreNMota/Desafio-01---Trilha-Node---Rocketseat.git
   cd desafio-01-fundamentos-nodejs
