# <img width="100" height="100" alt="image" src="https://github.com/user-attachments/assets/100f3c21-cd6a-49f3-8223-2274cfb507a0" />Análise de Desempenho Financeiro e Compliance

Este projeto tem como objetivo apresentar de forma visual, interativa e estratégica os principais indicadores financeiros e de conformidade de diversos projetos em execução. Desenvolvido com foco em análise de dados, o painel visa auxiliar gestores e stakeholders na tomada de decisões assertivas com base em evidências financeiras e de compliance.

## Objetivo do Projeto

Desenvolver um dashboard dinâmico e visual para monitoramento:

. Do desempenho financeiro total dos projetos;

. Da situação de conformidade dos projetos com critérios pré-estabelecidos;

. Da distribuição de lucros, despesas e impostos por projeto;

. Da proporção de projetos em conformidade e fora de conformidade;

. Da performance individual de cada projeto de forma comparativa.


## Tecnologias Utilizadas

Power BI: para visualização de dados interativa e criação de relatórios dinâmicos.

Excel / CSV: como fonte de dados simulada para os projetos.

Análise de Indicadores: aplicação de métricas de desempenho financeiro e compliance.

# <img width="100" height="100" alt="image" src="https://github.com/user-attachments/assets/e011e60a-57ea-43bf-b998-ce8cf4318c30" />Layout do Projetos
![Análise-de-Dados-Cosmos-Advisors-_1_-2025-07-25-12-35-41](https://github.com/user-attachments/assets/64497099-e27b-4174-b568-12269e74892e)

# <img width="100" height="100" alt="image" src="https://github.com/user-attachments/assets/413312d3-44f1-41d9-86cc-fce890650b45" />Medidas DAX

## Lucro Bruto
```DAX
Lucro Bruto = SUM(Sheet1[Receita])
```
## Impostos Totais
```DAX
Impostos Totais = (SUM(Sheet1[Receita]) * SUM(Sheet1[Impostos (%)]) )
/ 100
```
## Lucro Líquido
```DAX
Lucro Líquido = SUM(Sheet1[Receita]) - SUM(Sheet1[Despesas]) -
[Impostos Totais]
```
## Total de Projetos em Conformidade
```DAX
Projetos em Conformidade = CALCULATE(COUNT(Sheet1[Projeto]),
Sheet1[Status de Compliance] = "Em Conformidade")
```
## Total de Projetos Fora de Conformidade
```DAX
Projetos Fora de Conformidade = CALCULATE(COUNT(Sheet1[Projeto]),
Sheet1[Status de Compliance] = "Fora de Conformidade")
```
## Criar a Coluna Calculada de Valor de Imposto por Projeto
```DAX
Valor de Imposto = (Sheet1[Receita] * Sheet1[Impostos (%)]) / 100
```
## Atualizar a Medida de Impostos Totais
```DAX
Impostos Totais = SUM(Sheet1[Valor de Imposto])
```
## Revisar a Medida de Lucro Líquido
```DAX
Lucro Líquido = SUM(Sheet1[Receita]) - SUM(Sheet1[Despesas]) -
[Impostos Totais]
```

# <img width="100" height="100" alt="image" src="https://github.com/user-attachments/assets/dbb1cc44-737d-441e-8e5e-316b8c8bcc9d" />Diferenciais do Projeto
. Interface intuitiva com foco em clareza e usabilidade.

. Comparação entre múltiplos projetos em uma única visualização.

. Filtros dinâmicos para análise personalizada por compliance, lucro e tipo de despesa.

. Indicadores de performance com apelo visual e informativo.

. Ideal para áreas de controladoria, compliance, PMOs e gestão financeira.

# <img width="100" height="100" alt="image" src="https://github.com/user-attachments/assets/f723a55b-35ed-462a-be15-37830ac80f44" /> Autor
Thiago Klebis

Cientista de Dados | Especialista em Inteligência Artificial e Banco de Dados

[Linkdin](https://www.linkedin.com/in/thiagoklebis/) | [GitHub](https://github.com/TKlebis)
