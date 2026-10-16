
Relatório de Execução de Testes — SauceDemo

1. Identificação

- Projeto: QA Manual — E-commerce
- Aplicação: SauceDemo
- Responsável: Bruno Castro
- Tipo de teste: Testes funcionais manuais
- Status: Execução parcial concluída

2. Objetivo

Consolidar os resultados dos testes executados na funcionalidade de autenticação, comparando os resultados observados com os resultados esperados.

3. Resumo da execução

| Indicador | Resultado |
|---|---:|
| Casos executados | 9 |
| Aprovados | 8 |
| Reprovados | 1 |
| Bloqueados | 0 |
| Não executados neste conjunto | 0 |
| Taxa de aprovação | 88,9% |

Observação: os números representam os doze casos CT-001, CT-002, CT-003, CT-004, CT-005, CT-006, CT-007, CT-008, CT-009, CT-010, CT-011 e CT-012 relatados como executados. A taxa de aprovação representa apenas os casos executados neste conjunto, não a cobertura total da aplicação.

4. Resultados por caso de teste

| ID | Cenário | Resultado obtido | Status |
|---|---|---|---|
| CT-001 | Login com credenciais válidas | Login realizado com sucesso e página de produtos exibida. | Aprovado |
| CT-002 | Login com senha inválida | Acesso negado e mensagem de erro exibida. | Aprovado |
| CT-003 | Login com campos vazios | Acesso bloqueado e mensagem de validação de usuário obrigatório exibida. | Aprovado |
| CT-004 | Visualizar lista de produtos | Foram observadas três possíveis divergências entre imagens e descrições de produtos. | Reprovado |
| CT-005 | Ordenação de produtos por preço crescente | Menor preço (US$ 7,99) exibido no início e maior preço (US$ 49,99) no final da lista. | Aprovado |
| CT-006 | Adicionar produto ao carrinho | Produto adicionado com sucesso; botão alterado para “Remove” e indicador do carrinho exibindo 1. | Aprovado |
| CT-007 | Remover produto do carrinho | Produto removido com sucesso e carrinho ficou vazio. | Aprovado |
| CT-008 | Continuar comprando a partir do carrinho | Retorno à lista de produtos realizado com sucesso e produto mantido no carrinho. | Aprovado |
| CT-009 | Acessar os detalhes de um produto | Página de detalhes exibida normalmente. | Aprovado |

5. Escopo coberto

- Autenticação com credenciais válidas
- Rejeição de senha incorreta
- Validação de campos obrigatórios no login
- Ordenação de produtos por preço crescente
- Adição de produto ao carrinho
- Remoção de produto do carrinho
- Retorno à lista de produtos pelo botão Continue Shopping
- Acesso à página de detalhes dos produtos
  
6. Evidências

As capturas de tela dos testes estão armazenadas na pasta `evidence/`.

- CT-001: `evidence/ct-001-login-aprovado.png`
- CT-002: `evidence/ct-002-login-senha-invalida.png`
- CT-003: `evidence/ct-003-login-campos-vazios.png`
- CT-004: `evidence/BUG-001-imagem-descricao-camisa.png`
- CT-005: `evidence/ct-005-ordenacao-preco-crescente.png`
- CT-006: `evidence/ct-006-produto-adicionado-carrinho.png`
- CT-007: `evidence/ct-007-produto-removido-carrinho.png`
- CT-008: `evidence/ct-008-continuar-comprando.png`

A captura do CT-004 também é utilizada como evidência compartilhada nos registros BUG-001, BUG-002 e BUG-003, pois apresenta as três divergências observadas.

Nota: confirmar que cada arquivo existe no repositório e que a captura corresponde ao cenário descrito.

7. Defeitos em investigação

Foram documentadas três possíveis inconsistências durante o CT-004. Os registros permanecem pendentes de confirmação.

- BUG-001: Possível divergência entre a imagem e a descrição da camisa.
- BUG-002: Possível divergência na quantidade de botões do body infantil.
- BUG-003: Possível divergência entre a cor aparente da camisa e a cor informada na descrição.

Nenhum desses registros deve ser considerado defeito confirmado até que a ocorrência seja reproduzida e as evidências sejam verificadas.

Isso não comprova ausência de defeitos na aplicação; indica apenas que os três cenários executados apresentaram os comportamentos esperados.

8. Conclusão

Os três casos de teste de autenticação executados apresentaram resultados compatíveis com os critérios definidos.

A execução foi parcial e limitada aos cenários documentados. Recomenda-se ampliar os testes para navegação de produtos, ordenação, carrinho e finalização de compra.

9. Próximas atividades

- Executar testes de visualização e ordenação de produtos
- Validar inclusão e remoção de itens no carrinho
- Testar o fluxo de checkout
- Consolidar as evidências de cada cenário
- Atualizar este relatório conforme novas execuções
