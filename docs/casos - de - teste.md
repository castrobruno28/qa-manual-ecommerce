
Casos de Teste — SauceDemo

1. Informações gerais

- Projeto: QA Manual — E-commerce
- Aplicação: SauceDemo
- Tipo: Testes funcionais manuais
- Responsável: Bruno Castro
- Status da execução: Não executado


2. CT-001 — Login com credenciais válidas

Objetivo: Validar o acesso com um usuário autorizado.

Pré-condições:
- A aplicação deve estar acessível.
- Utilizar uma conta de demonstração válida disponibilizada pela aplicação.

Passos:
1. Acessar https://www.saucedemo.com/.
2. Informar o usuário `standard_user`.
3. Informar a senha válida correspondente.
4. Clicar em Login.

Resultado esperado:
O usuário deve acessar a área de produtos e visualizar a lista de itens disponíveis.

Resultado obtido:
Login realizado com sucesso e página com produtos exibida.

Status: Aprovado.

Evidência: evidence/ct-001-login-aprovado.png

Observações: O comportamento observado correspondeu ao resultado esperado.

---

3. CT-002 — Login com senha inválida

Objetivo: Verificar o tratamento de credenciais incorretas.

Pré-condições:
- A aplicação deve estar acessível.
- Utilizar um usuário de demonstração conhecido.

Passos:
1. Acessar a aplicação.
2. Informar o usuário `standard_user`.
3. Informar uma senha incorreta: `senha_errada_123`.
4. Clicar em Login.

Resultado esperado:
O acesso deve ser negado e uma mensagem de erro deve ser exibida.

Resultado obtido:
O acesso foi negado e a aplicação exibiu a mensagem: "Que triste: o nome de usuário e a senha não correspondem a nenhum usuário neste serviço."

Status: Aprovado.

Evidência: [CT-002 — Login com senha inválida](evidence/ct-002-login-senha-invalido.png)

Observações: O comportamento observado correspondeu ao resultado esperado.

---

4. CT-003 — Login sem preencher os campos

Objetivo: Validar a obrigatoriedade dos campos de autenticação.

Pré-condições:
- A página de login deve estar acessível.

Passos:
1. Acessar a aplicação.
2. Deixar os campos de usuário e senha vazios.
3. Clicar em Login.

Resultado esperado:
O acesso não deve ser realizado e a aplicação deve informar que o nome de usuário é obrigatório.

Resultado obtido:
O acesso foi bloqueado e a aplicação exibiu a mensagem: "Cara triste épica: É necessário nome de usuário."

Status: Aprovado.

Evidência: [CT-003 — Login com campos vazios](evidence/ct-003-login-campos-vazios.png)

Observações: O comportamento observado correspondeu ao resultado esperado.

---

5. CT-004 — Visualizar a lista de produtos

Objetivo: Validar a exibição dos produtos e a consistência entre imagens e descrições.

Pré-condições:
- Aplicação acessível.
- Usuário autenticado.

Passos:
1. Realizar login na aplicação.
2. Acessar a lista de produtos.
3. Comparar as imagens com as respectivas descrições.
4. Registrar divergências observadas.

Resultado esperado:
Os produtos devem apresentar imagens e descrições coerentes entre si, incluindo características visuais e informações sobre o produto.

Resultado obtido:
Foram observadas três possíveis inconsistências:

1. Segundo produto: a imagem mostra uma camisa preta, enquanto a descrição informa uma camisa cinza com raio vermelho.
2. Terceiro produto: a imagem mostra um body infantil com quatro botões de pressão, enquanto a descrição informa três botões na parte inferior.
3. Sexto produto: a imagem mostra uma camisa laranja, enquanto a descrição informa a cor vermelha.

Status: Reprovado.

Evidência: [BUG-001 — Divergências entre imagens e descrições](evidence/BUG-001-imagem-descricao-camisa.png)

Observações: As divergências precisam ser verificadas individualmente e reproduzidas para confirmar os defeitos.

---

6. CT-005 — Ordenação de produtos por preço crescente

Objetivo: Validar se os produtos são ordenados do menor para o maior preço.

Pré-condições:
- A aplicação deve estar acessível.
- O usuário deve estar autenticado.
- A lista de produtos deve estar visível.

Passos:
1. Acessar a página de produtos.
2. Localizar o menu de ordenação.
3. Selecionar `Price (low to high)`.
4. Verificar os preços apresentados.
5. Conferir se os produtos estão em ordem crescente.

Resultado esperado:
Os produtos devem ser apresentados do menor para o maior preço.

Resultado obtido:
O primeiro produto apresentou o preço de US$ 7,99 e o último, US$ 49,99.

Status: Aprovado.

- Evidência: [CT-005 — Ordenação por preço crescente](evidence/ct-005-ordenacao-preco-crescente.png)

Observações: Os preços inicial e final corresponderam ao comportamento esperado. Recomenda-se verificar também os preços intermediários.

7. CT-006 — Adicionar produto ao carrinho

Objetivo: Verificar se o usuário consegue adicionar um produto ao carrinho de compras.

Pré-condições:
- Usuário autenticado no sistema.
- Página de produtos aberta.

Passos para execução:
1. Acessar a página de produtos.
2. Localizar o produto "Sauce Labs Backpack".
3. Clicar no botão "Add to cart".
4. Verificar o botão do produto e o indicador do carrinho.

Resultado esperado:
- O produto é adicionado ao carrinho.
- O botão muda de "Add to cart" para "Remove".
- O indicador do carrinho apresenta o número "1".

Resultado obtido:
- O produto foi adicionado com sucesso.
- O botão mudou para "Remove".
- O indicador do carrinho apresentou o número "1".

Status: Aprovado.

Evidência: [CT-006 — Produto adicionado ao carrinho](evidence/ct-006-produto-adicionado-carrinho.png)

8. CT-007 — Remover produto do carrinho

Objetivo: Verificar se o usuário consegue remover um produto do carrinho de compras.

Pré-condições:
- Usuário autenticado no sistema.
- Produto *Sauce Labs Backpack* adicionado ao carrinho.

Passos para execução:
1. Acessar a página do carrinho.
2. Localizar o produto "Sauce Labs Backpack".
3. Clicar no botão "Remove".
4. Verificar se o produto foi removido da lista e se o carrinho ficou vazio.

Resultado esperado:
- O produto é removido do carrinho.
- O carrinho fica vazio.

Resultado obtido:
- O produto foi removido com sucesso.
- O carrinho ficou vazio.

Status: Aprovado.

Evidência: [CT-007 — Produto removido do carrinho](evidence/ct-007-produto-removido-carrinho.png)

9. CT-008 — Continuar comprando a partir do carrinho

Objetivo: Verificar se o usuário consegue retornar à lista de produtos a partir do carrinho e continuar comprando.

Pré-condições:
- Usuário autenticado no sistema.
- Produto *Sauce Labs Backpack* adicionado ao carrinho.

Passos para execução:
1. Acessar o carrinho de compras.
2. Confirmar que o produto aparece no carrinho.
3. Clicar no botão "Continue Shopping".
4. Verificar se o sistema retorna à lista de produtos.
5. Conferir se o indicador do carrinho continua mostrando 1 produto.

Resultado esperado:
- O sistema retorna à lista de produtos.
- A lista é exibida normalmente.
- O produto permanece no carrinho.

Resultado obtido:
- O sistema retornou à lista de produtos.
- Os produtos foram exibidos normalmente.
- O produto permaneceu no carrinho.

Status: Aprovado.

Evidência: [CT-008 — Continuar comprando](evidence/ct-008-continuar-comprando.png)

10. CT-009 — Acessar os detalhes de um produto

Objetivo: Verificar se o usuário consegue acessar a página de detalhes de um produto.

Pré-condições:
- Usuário autenticado no sistema.
- Lista de produtos disponível.

Passos para execução:
1. Localizar o produto "Sauce Labs Backpack".
2. Clicar no nome ou na imagem do produto.
3. Verificar as informações exibidas na página de detalhes.

Resultado esperado:
- A página de detalhes é aberta corretamente.
- Nome, imagem, descrição e preço do produto são exibidos.
- O botão "Add to cart" está disponível.

Resultado obtido:
- A página de detalhes foi exibida normalmente.

Status: Aprovado.

Evidência: [CT-009 — Detalhes do produto](evidence/ct-009-detalhes-produto.png)

11. CT-010 — Checkout com campos obrigatórios vazios

Objetivo: Verificar se o sistema impede o avanço no checkout quando os campos obrigatórios não são preenchidos.

Pré-condições:
- Usuário autenticado no sistema.
- Produto adicionado ao carrinho.
- Página de informações do checkout aberta.

Passos para execução:
1. Acessar o carrinho.
2. Clicar em "Checkout".
3. Deixar os campos First Name, Last Name e Zip/Postal Code vazios.
4. Clicar em "Continue".
5. Verificar a mensagem exibida pelo sistema.

Resultado esperado:
- O sistema impede o avanço para a próxima etapa.
- Uma mensagem de validação informa que há um campo obrigatório não preenchido.

Resultado obtido:
- O sistema bloqueou o avanço e exibiu uma mensagem de validação.

Status: Aprovado.

Evidência: [CT-010 — Checkout com campos vazios](evidence/ct-010-checkout-campos-vazios.png)

12. CT-011 — Finalizar uma compra com dados válidos

Objetivo: Verificar se o usuário consegue concluir uma compra preenchendo corretamente as informações obrigatórias do checkout.

Pré-condições:
- Usuário autenticado no sistema.
- Produto adicionado ao carrinho.

Passos para execução:
1. Acessar o carrinho de compras.
2. Clicar em "Checkout".
3. Preencher First Name, Last Name e Zip/Postal Code com dados fictícios válidos.
4. Clicar em "Continue".
5. Conferir o resumo do pedido.
6. Clicar em "Finish".
7. Verificar a mensagem de confirmação.

Resultado esperado:
- O checkout permite avançar com os dados preenchidos.
- O pedido é concluído.
- A mensagem "Thank you for your order!" é exibida.

Resultado obtido:
- Compra finalizada com sucesso e mensagem de confirmação exibida.

Status: Aprovado.

Evidência: [CT-011 — Compra finalizada](evidence/ct-011-compra-finalizada.png)

13. CT-012 — Cancelar checkout e retornar aos produtos

Objetivo: Verificar se o usuário consegue cancelar o checkout e retornar à lista de produtos.

Pré-condições:
- Usuário autenticado no sistema.
- Produto adicionado ao carrinho.
- Tela de informações do checkout aberta.

Passos para execução:
1. Acessar o carrinho.
2. Clicar em "Checkout".
3. Na tela "Checkout: Your Information", clicar em "Cancel".
4. Verificar a página exibida após o cancelamento.

Resultado esperado:
- O sistema retorna à lista de produtos.
- A página é exibida normalmente, sem erros visíveis.

Resultado obtido:
- O sistema retornou à lista de produtos normalmente.

Status: Aprovado.

Evidência: [CT-012 — Cancelar checkout](evidence/ct-012-cancelar-checkout.png)
