Projeto de QA Manual — E-commerce

Projeto de portfólio desenvolvido para praticar os fundamentos de **Quality Assurance (QA) e Testes de Software**, utilizando a aplicação de demonstração [SauceDemo](https://www.saucedemo.com/).

O objetivo é demonstrar a aplicação prática de testes manuais, documentação de cenários, registro de evidências, análise de resultados e identificação de possíveis defeitos.

Objetivos do projeto

- Elaborar e executar casos de teste manuais.
- Validar fluxos de autenticação, navegação, carrinho e checkout.
- Comparar resultados esperados com resultados obtidos.
- Registrar evidências de execução.
- Documentar possíveis defeitos encontrados.
- Consolidar os resultados em um relatório de execução.

Escopo dos testes

Os testes abrangem:

- Login com credenciais válidas e inválidas.
- Validação de campos obrigatórios.
- Visualização de produtos e detalhes.
- Ordenação de produtos por preço.
- Adição e remoção de produtos do carrinho.
- Navegação entre carrinho e lista de produtos.
- Validações e conclusão do checkout.

Resultados da execução

Foram planejados e executados "12 casos de teste".

| Indicador | Resultado |
|---|---:|
| Casos executados | 12 |
| Aprovados | 11 |
| Reprovados | 1 |
| Taxa de aprovação | 91,7% |

O CT-004 foi reprovado devido a possíveis divergências entre imagens e descrições de produtos, que foram registradas para investigação.

Estrutura do projeto

- `docs/plano-de-testes.md` — planejamento, escopo e abordagem dos testes.
- `docs/casos-de-teste.md` — cenários, passos, resultados esperados e obtidos.
- `docs/relatorio-de-execucao.md` — resumo e resultados da execução.
- `docs/evidence/` — capturas de tela utilizadas como evidências.
- `docs/bug-reports/` — documentação dos possíveis defeitos identificados.

Como navegar pelo projeto

1. Comece pelo plano de testes para conhecer o escopo.
2. Consulte os casos de teste para entender os procedimentos executados.
3. Acesse as evidências para visualizar os resultados observados.
4. Consulte os relatos de defeitos para conhecer as divergências registradas.
5. Finalize pelo relatório de execução para conferir o balanço geral.

Ferramentas e tecnologias

- Testes: testes manuais funcionais.
- Documentação: Markdown.
- Versionamento: Git e GitHub.
- Aplicação testada: SauceDemo.
- Gestão de testes: estudos de Jira em andamento.

Aprendizados

Este projeto contribuiu para praticar a elaboração de casos de teste, a execução de cenários, a organização de evidências, o registro de resultados e a documentação de possíveis defeitos.

Autor

Estudante de Análise e Desenvolvimento de Sistemas, em desenvolvimento profissional na área de QA e Testes de Software.

[GitHub — castrobruno28](https://github.com/castrobruno28)
