
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
2. Informar um usuário válido.
3. Informar a senha válida correspondente.
4. Clicar em Login.

Resultado esperado:
O usuário deve acessar a área de produtos e visualizar a lista de itens disponíveis.

Resultado obtido: A preencher após execução.

Status: Não executado.

---

3. CT-002 — Login com senha inválida

Objetivo: Verificar o tratamento de credenciais incorretas.

Pré-condições:
- A aplicação deve estar acessível.
- Utilizar um usuário de demonstração conhecido.

Passos:
1. Acessar a aplicação.
2. Informar um usuário válido.
3. Informar uma senha incorreta.
4. Clicar em Login.

Resultado esperado:
O acesso deve ser negado e uma mensagem de erro deve ser exibida.

Resultado obtido: A preencher após execução.

Status: Não executado.

---

4. CT-003 — Login sem preencher os campos

Objetivo: Validar a obrigatoriedade dos campos de autenticação.

Pré-condições:
A página de login deve estar acessível.

Passos:
1. Acessar a aplicação.
2. Deixar usuário e senha vazios.
3. Clicar em Login.

Resultado esperado:
O acesso não deve ser realizado e a aplicação deve informar que o usuário é obrigatório ou apresentar a validação correspondente.

Resultado obtido: A preencher após execução.

Status: Não executado.

---

5. CT-004 — Visualizar a lista de produtos

Objetivo: Validar a exibição dos produtos após autenticação.

Pré-condições:
Estar autenticado com uma conta de demonstração que permita acessar a página de produtos.

Passos:
1. Realizar login.
2. Observar a página de produtos.
3. Verificar nomes, imagens e preços dos itens apresentados.

Resultado esperado:
A lista de produtos deve ser exibida com as informações disponíveis em cada item.

Resultado obtido: A preencher após execução.

Status: Não executado.

---

6. CT-005 — Adicionar produto ao carrinho

Objetivo: Verificar se um produto pode ser adicionado ao carrinho.

Pré-condições:
Estar autenticado e na página de produtos.

Passos:
1. Selecionar um produto disponível.
2. Clicar em Add to cart.
3. Verificar o indicador do carrinho.
4. Abrir o carrinho.

Resultado esperado:
O produto selecionado deve aparecer no carrinho e o indicador deve refletir a quantidade de itens, quando aplicável.

Resultado obtido: A preencher após execução.

Status: Não executado.
