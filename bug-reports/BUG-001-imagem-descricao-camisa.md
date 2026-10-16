BUG-001 — Divergência entre imagem e descrição da camisa

Identificação
- Projeto: QA Manual — E-commerce
- Caso relacionado: CT-004
- Tipo: Consistência de conteúdo
- Status: Aberto para investigação
- Severidade: A definir após análise do impacto

Descrição
A imagem do segundo produto foi observada como uma camisa preta, enquanto a descrição textual informa uma camisa cinza com raio vermelho.

Pré-condições
Acessar a aplicação e visualizar a lista de produtos.

Passos para reproduzir
1. Realizar login.
2. Abrir a lista de produtos.
3. Localizar o segundo produto.
4. Comparar a imagem com a descrição textual.

Resultado esperado
A imagem e a descrição devem representar características compatíveis do mesmo produto.

Resultado obtido
Foi observada uma possível divergência entre a cor da camisa na imagem e a cor informada na descrição.

Evidência

- Captura: `../evidence/BUG-001-imagem-descricao-camisa.png`
- Caso de teste relacionado: CT-004.
- Observação: captura compartilhada entre os três registros de possíveis defeitos.

Observações
Defeito pendente de confirmação e investigação.
