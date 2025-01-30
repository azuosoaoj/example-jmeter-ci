# Relatório de Teste de carga

## Resumo do Teste

Foi realizado um teste de carga no site [blazedemo.com](https://blazedemo.com/), simulando a compra de passagens com 10 usuários virtuais, com o objetivo de avaliar a performance da aplicação.

- **Total de Requisições**: 3.396
- **Total de Falhas**: 0
- **90th**: 1.685 ms

---

## Detalhamento das Requisições

| Requisição             | Total de requisições | Taxa de erro | 90th  |
|------------------------|-------------|--------|---------------|
| Geral                  | 3.396       | 0      | 1.685 ms      |
| GET - /index.php       | 853         | 0      | 1.659 ms      |
| POST - /reserve.php    | 851         | 0      | 1.645 ms      |
| POST - /purchase.php   | 848         | 0      | 1.712 ms      |
| POST - /confirmation.php | 844       | 0      | 1.745 ms      |

---

## Conclusão

- O teste foi executado com sucesso, sem falhas.
- O tempo médio de resposta do 90º percentil para todas as requisições estão dentro dos limites aceitáveis, com 1.685 ms.
- Em relação ao numero de requisições por segundo, está abaixo do esperado, acredito que a aplicação não suporte tal carga mantendo o tempo médio de resposta de forma aceitavel.

[Relatório de execução](https://latencylingo.com/test-runs/c9496e02-64ce-47cf-ae65-41aeb2303825?version=3)