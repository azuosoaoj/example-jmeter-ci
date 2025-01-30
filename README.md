# example-jmeter-ci

Este repositório automatiza a execução de testes de performance utilizando o JMeter via GitHub Actions e integra com o Latency Lingo para análise dos resultados.

## Como Rodar os Testes via GitHub Actions

1. **Configuração Inicial**:
   - Faça um **fork** deste repositório para o seu repositório.
   - Crie um arquivo `.jmx` com o teste de performance desejado e faça o **push** para o repositório ou utilize algum `.jmx` dentro da pasta `jmeter-files`.
   - Importante citar que o arquivo `.jmx` deve estar dentro da pasta `jmeter-files`.
   - Para visualizar os resultados no Latency Lingo, é necessário realizar o cadastro no site do [Latency Lingo](https://latencylingo.com/) e obter uma chave de API. Em seguida, adicione a chave de API no GitHub Actions Secrets com o nome `LATENCY_LINGO_API_KEY`.

2. **Rodando o Workflow**:
   - No GitHub, vá para a aba **Actions** do seu repositório.
   - Selecione o workflow `.github/workflows/jmeter-test.yml` do lado esquerdo da tela.
   - Clique em **Run workflow**.
   - Forneça o nome do arquivo `.jmx` que você deseja rodar no campo de entrada `jmx_file`.
   - Clique em **Run workflow** novamente para iniciar a execução.

3. **Análise dos Resultados**:
   - Após a execução, os resultados do teste serão armazenados no arquivo `result.jtl`.
   - O Latency Lingo utilizará esse arquivo para gerar um relátorio contendo as principais métricas da execução.
   - O link do relatório gerado estará disponível nos logs de execução do step Analyze Results with Latency Lingo.

[Relátorio de execução do teste de carga executado](./report/load_test.md)
