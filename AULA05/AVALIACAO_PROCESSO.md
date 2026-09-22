**Cenário A:** Conciliação bancária diária feita a partir do download do extrato `.csv` e comparação das linhas com as baixas do sistema ERP via regras fixas de CNPJ e valor.

1. Nome do Processo
2. É viável para RPA? (Sim / Não)
3. Justificativa baseada nos 4 critérios essenciais (Repetitividade, Regras de Negócio, Tipo de Dados, Volume).
4. Mapeamento Passo a Passo das Ações do Robô

# Ficha de Avaliação de RPA

## 1. Nome do Processo

**Conciliação Bancária Diária**

Processo de comparação entre as movimentações de um extrato bancário em formato `.csv` e as baixas registradas no sistema ERP, utilizando regras fixas de **CNPJ e valor**.

## 2. É viável para RPA?

**Sim.**

## 3. Justificativa baseada nos 4 critérios essenciais

### Repetitividade

**Alta.**

A conciliação bancária é realizada diariamente e segue praticamente os mesmos passos em todas as execuções. O robô pode repetir o processo sem a necessidade de realizar manualmente as mesmas tarefas todos os dias.

### Regras de Negócio

**Bem definidas.**

As regras para comparação são objetivas e podem ser programadas. Por exemplo:

* Comparar o **CNPJ** do registro bancário com o CNPJ cadastrado no ERP.
* Comparar o **valor** da movimentação bancária com o valor da baixa no ERP.
* Considerar o registro conciliado quando CNPJ e valor forem correspondentes.
* Separar os registros que não possuírem correspondência para análise manual.

### Tipo de Dados

**Adequado para RPA.**

O processo utiliza dados estruturados, principalmente informações presentes em arquivos `.csv` e no sistema ERP, como:

* CNPJ;
* Data;
* Valor;
* Número ou identificação da transação;
* Informações da baixa no ERP.

Esses dados podem ser lidos e comparados automaticamente pelo robô.

### Volume

**Alto.**

Uma empresa pode possuir muitas movimentações bancárias diariamente. A automação permite que o robô processe uma grande quantidade de registros de forma mais rápida e padronizada do que uma conferência manual.

## 4. Mapeamento Passo a Passo das Ações do Robô

1. **Iniciar o processo** de conciliação bancária diária.
2. **Acessar o local** onde o extrato bancário está disponível.
3. **Baixar o extrato bancário** no formato `.csv`.
4. **Abrir e ler o arquivo `.csv`**.
5. **Acessar o sistema ERP** com as credenciais configuradas.
6. **Consultar as baixas financeiras** correspondentes ao período analisado.
7. **Ler os registros do ERP**.
8. **Comparar o CNPJ** do extrato bancário com o CNPJ registrado no ERP.
9. **Comparar o valor** da movimentação bancária com o valor da baixa no ERP.
10. **Identificar os registros conciliados** quando CNPJ e valor forem iguais.
11. **Identificar os registros não conciliados** quando não houver correspondência.
12. **Registrar o resultado** da conciliação.
13. **Gerar um relatório** contendo registros conciliados e pendências.
14. **Finalizar o processo** e disponibilizar o relatório para análise dos responsáveis.

## Conclusão

O processo de conciliação bancária diária é **viável para RPA**, pois possui alta repetitividade, regras de negócio objetivas, dados estruturados e potencial para processamento de grande volume de informações. Essas características permitem que grande parte das atividades seja executada automaticamente por um robô.

 