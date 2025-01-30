# Relatório de Teste de carga

## Resumo do Teste

- **Total de Requisições**: 5.471
- **Total de Falhas**: 0
- **90th**: 1.070 ms

---

## Detalhamento das Requisições

| Requisição             | Total de requisições | Taxa de erro | Latência p90  |
|------------------------|-------------|--------|---------------|
| Geral                  | 5.471       | 0%      | 1.070 ms      |
| GET - /index.php       | 1.370       | 0%      | 1.111 ms      |
| POST - /reserve.php    | 1.368       | 0%      | 1.037 ms      |
| POST - /purchase.php   | 1.367       | 0%      | 1.051 ms      |
| POST - /confirmation.php | 1.366     | 0%      | 1.049 ms      |

---

## Conclusão

- O teste foi executado com sucesso, sem falhas.
- O tempo médio de resposta do 90º percentil para todas as requisições estão dentro dos limites aceitáveis, com 1.070 ms.
- Em relação ao numero de requisições por segundo, está abaixo do esperado, acredito que a aplicação não suporte tal carga matendo o tempo médio de resposta de forma aceitavel.

[Relatório de Teste](https://latencylingo.com/test-runs/786ec2b4-061a-48af-9058-e574d868e56f)