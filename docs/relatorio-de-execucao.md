
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
| Casos de teste executados | 3 |
| Aprovados | 3 |
| Reprovados | 0 |
| Bloqueados | 0 |
| Não executados neste conjunto | 0 |
| Taxa de aprovação | 100% |

Observação: os números representam os três casos CT-001, CT-002 e CT-003 relatados como executados. O percentual não representa a cobertura total da aplicação.

4. Resultados por caso de teste

| ID | Cenário | Resultado | Status |
|---|---|---|---|
| CT-001 | Login com credenciais válidas | Página de produtos exibida | Aprovado |
| CT-002 | Login com senha inválida | Acesso negado e mensagem de erro exibida | Aprovado |
| CT-003 | Login com campos vazios | Acesso bloqueado e validação de usuário obrigatório exibida | Aprovado |

5. Escopo coberto

- Autenticação com credenciais válidas
- Rejeição de senha incorreta
- Validação de campos obrigatórios no login

6. Evidências

As capturas de tela dos casos executados devem ser armazenadas na pasta `evidence/` e vinculadas aos respectivos casos de teste.

- CT-001: `evidence/ct-001-login-aprovado.png`
- CT-002: `evidence/ct-002-login-senha-invalida.png`
- CT-003: `evidence/ct-003-login-campos-vazios.png`

Nota: confirmar os nomes e a existência dos arquivos no repositório antes de considerar todas as evidências vinculadas.

7. Defeitos identificados

Nenhum defeito foi registrado neste conjunto de testes.

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
