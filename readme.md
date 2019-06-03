# Teste de Full-Stack / Back-End / Front-End (NodeJS / Java)
### Proposta
Uma empresa vai lançar um novo app para venda de celulares e com isso gostaríamos que você construísse uma API para gerenciar o cadastro de novos celulares.

### Solução
A solução consistirá em criar uma API REST escrita em Java (ou NodeJS) e uma aplicação frontend usando React.

### Descrição do modelo
| Campo | Tipo | Descrição | Restrições |
| ------ | ------ | ------ | ------ |
| model | Texto | Nome do modelo do celular | Alfanumérico com no mínimo 2 e no máximo 255 caracteres, desprezando espaço em branco. |
| price | Número real | Preço do celular | Número positivo |
| brand | Texto | Nome da marca do celular | Alfanumérico com no mínimo 2 e no máximo 255 caracteres, desprezando espaço em branco. |
| photo | Texto | URL contendo uma imagem que representa o celular | Máximo 255 caracteres, desprezando espaço em branco. |
| startDate | Data | Data de início da venda do celular | Data no formato “dd/MM/yyyy” (31/12/2018). A data de início deve ser posterior ao dia 25/12/2018. |
| endDate | Data | Data de fim da venda do celular | Data no formato “dd/MM/yyyy” (31/12/2018). A data de fim deve ser posterior a data de início. |
| color | Lista fixa | Cor do celular | Essa campo admite apenas os seguintes valores: BLACK, WHITE, GOLD, PINK. |
| code | Texto | Código de identificação do celular | Alfanumérico de 8 caracteres. Não deve se repetir. |

### Operações
Deve ser possível **cadastrar, pesquisar, editar, excluir e listar** todos os celulares. 

### Busca
Deve ser possível buscar celulares por **qualquer combinação** de seus atributos. Por exemplo, buscar um celular por modelo, ou por marca e cor.

### Validação
O sistema deve validar todas as entradas, tanto no backend quanto no frontend.

O backend deve retornar um resposta com o código HTTP adequado, de acordo com o resultado da validação, além de incluir uma mensagem para cada violação.

O frontend deve validar os campos à medida que o usuário preenche o formulário, e exibir as mensagens de erro correspondentes.

### Outros testes

Teste Front-End Dev (https://github.com/melhorcom/front-end-teste)

Teste Back-End Dev (https://github.com/melhorcom/back-end-teste)
