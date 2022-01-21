
## Para o desenvolvimento do seguinte desafio:

- Utilize Express ou NextJS;
- Utilize framework React ou VueJS;
- Estilo de indentação: 2 espaços;
- Caso preferir poderá utilizar Eslint no padrão que preferir/ (ex: https://standardjs.com/)

### 1. Criar uma página com
	
- Um campo tipo input chamado "Gravar Termo" (save);
- Um campo tipo input chamado "Pesquisar Termo" (search);
- Um bloco para retorno de dados em lista com: título, descrição, imagem e link;
- Um bloco para termos relacionados

### 2. Consumir e gravar dados

Ao escrever um termo no campo de gravação (save) e submeter, executar as seguinte ações:

- Gravar os dados retornados do `endpoint` em banco mysql ou postgres utilizando biblioteca como o prisma ou sequelize ou qualquer uma que preferir. OBS: Gravar somente quando tiver conteúdo;
- Salvar o objeto `term` assim como o objeto `relateds`. A estrutura de relacionamento no banco pode ser definida como desejar;
- Retornar uma mensagem de sucesso

**Endpoints:**

- **Exemplo com conteúdo**: `https://data.easycontent.com/api/v1/wikipedia?term=Matrix`
- **Exemplo com erro/vazio:** `https://data.easycontent.com/api/v1/wikipedia?term=gasdasd`

### 3. Pesquisar dados

Não utilizar os endpoints acima para consulta. A consulta deverá ser consultada direto no banco de dados.

Ao escrever um termo no campo de pesquisar, executar as seguintes ações:

- Pesquisar no banco (postgres ou mysql) por termos relacionados;
- Retornar o termo encontrado no bloco de dados em lista com os ítens já descritos;
- Retornar todos os termos relacionados ao termo pesquisado (já com click de link para uma nova pesquisa)

### 4. Como enviar

- Gere um dump do banco e inclua dentro de uma pasta na raiz do projeto;
- Inclua um readme.md com instrução para instalação;
- Publique no Github e envie para o email do seu recrutador.
