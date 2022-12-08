# Projeto-11-FrontEnd-Online-Store

Neste projeto você criará uma versão simplificada, sem persistência no banco de dados, de uma loja online, desenvolvendo em grupo suas funcionalidades de acordo com demandas definidas em um quadro Kanban, em um cenário próximo ao do mercado de trabalho.

A partir dessas demandas, teremos uma aplicação em que pessoas usuárias poderão:

Buscar produtos por termos e categorias a partir da API do Mercado Livre;
Interagir com os produtos buscados de modo a adicioná-los e removê-los de um carrinho de compras em diferentes quantidades;
Visualizar detalhes e avaliações prévias de um produto, bem como criar novas avaliações e;
Simular a finalização da compra dos itens selecionados.

Neste projeto você será irá:

Entender o que são Métodos Ágeis;
Entender o que é Kanban;
Entender o que é Scrum;
Trabalhar em equipes utilizando Kanban ou Scrum de maneira eficaz;
Praticar todas as habilidades desenvolvidas até agora no módulo de Front-end.
Comunicação Eficaz - Assertividade & Prática de feedbacks
Gerenciamento de Conflitos
Colaboração

Requisitos
warning ATENÇÃO - 01 Pull Requests com erros de linter não serão avaliados.

warning ATENÇÃO - 02 As imagens são meramente ilustrativas para visualizar o fluxo da aplicação, os nomes devem seguir os requisitos e não as imagens.

warning ATENÇÃO - 03 Para que os testes funcionem corretamente, é necessario que o seu BrowserRouter fique dentro do arquivo index.js, envolvendo o componente .

warning ATENÇÃO - 04 Não recomendamos utilizar o localStorage para guardar e compartilhar dados entre componentes. Faça isso apenas quando o requisito pedir explicitamente a persistência de dados.

1. Implemente o módulo de acesso à api do Mercado Livre
PRIORIDADE 0

Implemente um módulo que acessa a API do Mercado Livre:

O que será verificado

2. Crie uma página de listagem de produtos vazia
PRIORIDADE 0

A tela principal da plataforma é a de listagem de produtos, onde a pessoa usuária poderá buscar produtos para adicionar ao carrinho, além de filtrar suas buscas.

Crie o campo de busca da tela principal, que será utilizado para listar os produtos encontrados:
Exemplo de página de listagem de produtos antes da busca

O que será verificado

3. Crie a página do carrinho de compras
PRIORIDADE 1

A pessoa usuária poderá adicionar produtos em seu carrinho de compras, a partir da listagem dos produtos.

Crie uma tela que representará o carrinho de compras da aplicação. Além disso, na tela principal, crie um botão que redireciona à página do carrinho de compras. Inicialmente, o carrinho deve estar vazio.

Crie uma tela que represente o carrinho de compras:
Na tela principal, crie um elemento que redirecione a pessoa usuária à página do carrinho de compras:

O que será verificado

4. Liste as categorias de produtos disponíveis via API na página principal
PRIORIDADE 1

A tela principal (listagem dos produtos) deve conter uma lista de categorias, que será utilizada para filtrar a busca por categoria. As categorias podem ser obtidas pela API do Mercado Livre. A requisição para essa API deve ser feita uma única vez, após o carregamento da tela.

Na tela principal, liste as categorias obtidas pela API do Mercado Livre:

O que será verificado

5. Liste os produtos buscados por termos, com os dados resumidos, associados a esses termos
PRIORIDADE 1

A alma da aplicação é a sua lógica de busca e listagem de produtos. Após digitar seus termos no input da tela principal e clicar no botão de busca, uma requisição deverá ser feita à API do Mercado Livre, tendo como parâmetros a frase digitada. Os produtos retornados pela API devem ser listados na tela.

Na tela principal, crie a listagem dos produtos recebidos pela API do Mercado Livre ao clicar no botão de busca:

Exemplo da tela principal após uma busca por produtos:
Exemplo da tela principal caso a busca não retorne resultados:

O que será verificado

6. Selecione uma categoria e mostre somente os produtos daquela categoria
PRIORIDADE 2

Quando a pessoa usuária clicar em uma das categorias listadas na tela principal, a aplicação deverá listar todos os produtos encontrados daquela categoria.

Na tela principal, ao clicar em uma das categorias listadas, crie a listagem dos produtos dessa categoria:

O que será verificado

7. Redirecione para uma tela com a exibição detalhada ao clicar na exibição resumida de um produto
PRIORIDADE 3

Agora que a listagem dos produtos está criada, você deverá criar a página de detalhes de um produto.

Ao clicar "no card" de um produto, a pessoa usuária deve ser direcionada para uma página contendo o nome, uma imagem, o preço e a especificação técnica desse produto. Além disso, essa página deve ter um botão que, ao clicar, a pessoa usuária deve ser redirecionada para a página do carrinho de compras.

Exemplo da tela de detalhes de um produto:

Ao clicar em "um card" de um produto (o elemento com data-testid="product"), a pessoa usuária deve ser redirecionada para uma página contendo os detalhes do produto:

O que será verificado

8. Adicione produtos ao carrinho a partir da tela de listagem de produtos
PRIORIDADE 3

A pessoa usuária pode adicionar um produto ao carrinho de compras a partir da página principal contendo a listagem dos produtos.

Todos os produtos que foram adicionados ao carrinho devem aparecer na tela do Carrinho de Compras.

Lembrete: Quando renderizamos os itens da categoria, os dados dos produtos já estão dentro da sua aplicação. Pense em como armazenar eles sem a necessidade de fazer outra requisição.
Exemplo da página principal

Na tela principal, crie um elemento em cada produto que, ao ser clicado, adiciona o produto ao carrinho de compras:
Na tela do Carrinho de Compras, renderize todos os produtos que foram adicionados ao carrinho:

O que será verificado

9. Adicione um produto ao carrinho a partir de sua tela de exibição detalhada
PRIORIDADE 3

A partir da tela de detalhes de um produto, deve ser possível adicioná-lo ao carrinho de compras.

Na tela de detalhes de um produto, crie um elemento que adicione o produto ao carrinho:
Na tela do carrinho de compras, renderize todos os produtos adicionados ao carrinho:
O que será verificado

10. Visualize a lista de produtos adicionados ao carrinho em sua página e permita a manipulação da sua quantidade
PRIORIDADE 3

Ao entrar na página, todos os produtos salvos no local storage devem ser renderizados.

Na tela do Carrinho de Compras, deve ser possível aumentar e/ou diminuir a quantidade do produto. Também deve ser possível excluir um produto do carrinho.

Exemplo da tela do carrinho de compras:

Na página do carrinho de compras, crie dois elementos para cada produto que, ao serem clicados, diminuem ou aumentam a quantidade desse produto presente no carrinho:

O que será verificado

11. Avalie e comente acerca de um produto em sua tela de exibição detalhada
PRIORIDADE 3

Na tela de detalhes de um produto, deve existir um formulário para adicionar avaliações sobre ele. Este formulário deve conter um campo para o e-mail da pessoa avaliadora, uma nota entre 1 e 5 e um campo para comentários sobre o produto. Além disso, os campos e-mail e nota devem ser obrigatórios e o e-mail deve ser válido (exemplo: teste@trybe.com).

A lista de avaliações já realizadas devem ser renderizadas na tela de detalhes do produto caso a pessoa usuária recarregue a página.

Exemplo da tela de detalhes contendo o formulário para adicionar avaliações:

Exemplo da tela de detalhes contendo avaliações:

Na tela de detalhes de um produto, crie um formulário para adicionar avaliações:

Avalie se o formulário é valido:

Renderize as avaliações criadas a partir do formulário:

O que será verificado

12. Finalize a compra vendo um resumo dela, preenchendo os seus dados e escolhendo a forma de pagamento
PRIORIDADE 4

Crie uma tela para a finalização da compra, que deve ser acessada a partir da tela do Carrinho de Compras. A tela deve conter um formulário para adicionar as informações do comprador e um resumo dos produtos que foram adicionados ao carrinho. Após finalizar a compra, caso o formulário esteja validado, o carrinho deve ser esvaziado e a pessoa usuária deve ser redirecionada pala a tela principal (listagem dos produtos).

Exemplo de processo completo da finalização:

Na tela do carrinho de compras, crie um elemento para finalizar a compra:
Na tela de checkout, mostre um resumo dos produtos adicionados ao carrinho
Na tela de checkout, crie um formulário para a pessoa usuária adicionar os seus dados pessoais:
Ao clicar no botão para submeter o formulário:

O que será verificado
