# Análise Exploratória 

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/scof-fernandes/Trabalho-Academico_-Analise-Exploratoria-de-Dados_Python/blob/main/Análise_Exploratoria,_EAP_EMPÓRIO_Estacio,_Liberdade_stefany_coelho.ipynb)

## Como executar o projeto
Para visualizar e interagir com o código:
1. Clique no botão **"Open in Colab"** no topo desta página.
2. No Colab, vá em `Ambiente de Execução` > `Reiniciar e rodar tudo`.
*Obs: O projeto consome dados diretamente do GitHub via links Raw, não sendo necessário upload manual.*

## Sobre o Projeto
Este projeto foi desenvolvido como parte de um trabalho acadêmico. O objetivo principal é realizar uma Análise Exploratória de Dados (EDA) utilizando Python para extrair insights sobre .


## tecnologias Utilizadas
O projeto utilizou principalmente a linguagem Python e as bibliotecas:
* Pandas para manipulação e análise de dados.
* Numpy para cálculos numéricos e simulações de Monte Carlo.
* Seaborn e Matplotlib.pyplot para visualização de dados.
* Odfpy e Defusedxml para leitura de arquivos .ods.

## Análises Realizadas e Resultados
* Limpeza e Preparação de Dados
A coluna NCM (Nomenclatura Comum do Mercosul) foi considerada inútil para a análise de negócios e foi removida de ambos os DataFrames.

* Identificação de Erros e Discrepâncias
Valores Zero (2022 vs 2023): O inventário de 2022 apresentou 495 zeros na coluna Preço Compra e 498 em Custo Médio, o que indica produtos com custos já amortizados (vendidos anteriormente). No entanto, um erro de precificação foi identificado no produto Campari 900ml, que tinha Preço Venda igual a R$ 0,00. O inventário de 2023 não apresentou valores zero nas colunas financeiras, indicando melhores processos de registro.

* Códigos de Barras Repetidos: Nenhuma duplicidade de códigos de barra associados a produtos diferentes foi encontrada em ambos os inventários (pp. 8-9).
Validade dos Produtos: Nenhuma cerveja estava fora do prazo de validade nos anos de 2022 e 2023.

* Análise de Estoque e Precificação: número de itens únicos diminuiu de 954 (2022) para 655 (2023), sugerindo otimização de portfólio. O Preço Compra médio aumentou significativamente de 2022 para 2023, enquanto o Preço Venda médio diminuiu, indicando um estreitamento da margem de lucro por produto.

* Análise de Monte Carlo (Simulação de Lucro e Risco)
A simulação de Monte Carlo foi utilizada para estimar o lucro potencial total e o risco de prejuízo.

<img width="624" height="172" alt="image" src="https://github.com/user-attachments/assets/3e8e6391-cad4-43f8-8b37-c6be0cb2d143" />

## Conclusão
O inventário de 2023 demonstrou uma base de dados mais confiável, com a eliminação de erros de registro e a garantia de lucro total em todos os cenários simulados. No entanto, houve uma redução considerável no lucro esperado em comparação com 2022, devido a uma diminuição no número de itens e mudanças na dinâmica de preços e custos.
Produtos específicos com alto risco de prejuízo individual foram identificados em ambos os anos e requerem atenção imediata da gestão para otimizar a rentabilidade.



---
Desenvolvido por [Seu Nome] - [Seu LinkedIn ou E-mail]
