## RELAÇÃO ENTRE OS METÓDOS HTTP E CRUD...

O termo CRUD vem das operações que podem ser executadas em um banco de dados:

C - Create == CRIAR
R - Read   == LER
U - Update == ATUALIZAR
D - Delete == EXCLUIR

Quando temos uma tela que é capaz de ver, localizar e atualizar informações também é chamado CRUD.

Esse conceito foi traduzido para operações do protocolo HTTP onde temos:

C - Create == POST
R - Read   == GET
U - Update == PUT
D - Delete == DELETE


## DIFERENÇA ENTRE PUT E PATCH...

PUT: É um método de modificação de recurso onde o cliente envia dados que atualizam todo o recurso. PUT é semelhante ao POST no sentido de que pode criar recursos, mas o faz quando há uma URL definida em que PUT substitui todo o recurso, se existir, ou cria novos, se não existir.

Exemplo: quando você deseja atualizar o nome e e-mail do Candidato, deve-se enviar todos os parâmetros do Candidato incluindo aqueles que não devem ser atualizados no corpo da solicitação, caso contrário, ele simplesmente substituirá todo o recurso pelo nome e e-mail.


PATCH: Ao contrário da Solicitação PUT, PATCH faz atualização parcial, por exemplo, Campos que precisam ser atualizados pelo cliente, apenas esse campo é atualizado sem modificar o outro campo.

Exemplo:Você deseja atualizar apenas um ou alguns dados e não a informação completa.


## IDEMPOTÊNCIA...

É a propriedade que algumas operações têm de poder ser aplicadas várias vezes sem alterar o valor do resultado após a aplicação inicial. Métodos seguros são aqueles que não alteram o estado servidor ou seja somente executa operações de leitura.
Quando falamos em idempotência em API’s REST, podemos concluir que os seguintes os verbos:

GET, PUT, DELETE, HEAD e OPTIONS são idempotentes.

POST não é idempotente.


## PADRÕES DE OBJETOS...

Criacionais: padrões que propõem soluções flexíveis para criação de objetos. 

Estruturais: padrões que propõem soluções flexíveis para composição de classes e objetos. 

Comportamentais: padrões que propõem soluções flexíveis para interação e divisão de responsabilidades entre classes e objetos.


