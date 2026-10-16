
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

Evidência: Capturada. Arquivo a vincular: `evidence/ct-002-login-senha-invalida.png`.

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

Evidência: Capturada. Arquivo a vincular: `evidence/ct-003-login-campos-vazios.png`.

Observações: O comportamento observado correspondeu ao resultado esperado.

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
