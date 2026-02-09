# Análise Exploratória de Dados: Gestão de Inventário EAP Empório

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/scof-fernandes/Trabalho-Academico_-Analise-Exploratoria-de-Dados_Python/blob/main/Análise_Exploratoria,_EAP_EMPÓRIO_Estacio,_Liberdade_stefany_coelho.ipynb)

## Como executar o projeto
Para visualizar e interagir com o código:
1. Clique no botão **"Open in Colab"** no topo desta página.
2. No Colab, vá em `Ambiente de Execução` > `Reiniciar e rodar tudo`.
   
*Obs: O projeto consome dados diretamente do GitHub via links Raw, não sendo necessário upload manual.*

## Sobre o Projeto
Este projeto utiliza técnicas avançadas de **Data Science** e **Estatística** para analisar a saúde financeira de um inventário de varejo, comparando os anos de 2022 e 2023. O foco principal é a identificação de anomalias de precificação, simulação de cenários de lucro e mitigação de riscos operacionais.

## tecnologias e Metodologia
### Ferramentas Utilizadas:
*   **Manipulação de Dados:** `Pandas` e `Numpy`.
*   **Visualização:** `Seaborn` e `Matplotlib` para dashboards estatísticos.
*   **Processamento de Arquivos:** `Odfpy` para leitura de planilhas `.ods`.

## Abordagem Técnica:
* **Data Cleaning:** Identificação de itens com preço zerado e tratamento de custos amortizados.
* **Análise de Margem:** Avaliação do impacto do aumento do custo de compra sobre o preço de venda.
* **Simulação de Monte Carlo:** Geração de milhares de cenários para prever o lucro esperado.
* **Cálculo de VaR (Value at Risk):** Mensuração do risco financeiro máximo com 95% de confiança.

## Análises e Resultados Estratégicos
### Integridade e Qualidade dos Dados (Data Quality)
**Saneamento de Registros :** Evolução crítica entre os anos. Enquanto 2022 possuía inconsistências (como o Campari 900ml a R$ 0,00), o inventário de 2023 apresentou zero falhas de preenchimento, indicando maturidade nos processos de inventário. 

**Conformidade Legal:** Auditoria de códigos de barras e validades confirmou 100% de conformidade com as normas técnicas e o Código de Defesa do Consumidor, sem duplicidades ou produtos vencidos. 

### Dinâmica de Estoque e Margem
**Otimização de Portfólio:** Redução estratégica de 31% no volume de itens únicos (de 954 para 655), focando em um estoque mais enxuto e de maior giro.

**Desafio de Rentabilidade:** Identificou-se um estreitamento de margem perigoso; o custo médio de compra subiu significativamente enquanto o preço de venda médio caiu, exigindo uma revisão imediata da estratégia de precificação. 

## Análise de Monte Carlo (Simulação de Lucro e Risco)
A simulação de Monte Carlo foi utilizada para estimar o lucro potencial total e o risco de prejuízo, A simulação foi configurada com 2.000 iterações, aplicando estresse nas variáveis de preço e custo para modelar o comportamento do mercado

<img width="624" height="172" alt="image" src="https://github.com/user-attachments/assets/3e8e6391-cad4-43f8-8b37-c6be0cb2d143" />

### Conclusão Técnica
A empresa realizou uma transição bem-sucedida de uma gestão reativa (correção de dados em 2022) para uma gestão proativa (processos robustos em 2023), resultando em um inventário financeiramente estável, previsível e com alta segurança estatística.

* **Volatilidade do Preço de Venda:** 10% (distribuição normal). 
* **Volatilidade do Custo Médio:** 8% (distribuição normal). 
* **Tratamento de Dados:** Itens com custo zerado (já amortizados) e erros de precificação (Campari 900ml) foram isolados para não distorcer as projeções.
* **Probabilidade de Prejuízo Total (0.00%):** Em ambos os anos, a simulação indicou que, no agregado, o inventário é extremamente resiliente e gerará lucro em 100% dos cenários simulados.
* **Value at Risk (VaR 95%):** O VaR de 2023 ficou em R$ 183.104,01, o que representa a perda máxima esperada nos 5% piores cenários possíveis.

## Conclusão
O EAP Empório apresenta uma base financeira sólida e resiliente. O sucesso futuro depende agora da manutenção da qualidade dos dados e de uma revisão cirúrgica na precificação dos itens de alta volatilidade, garantindo que o crescimento da empresa continue ininterrupto e sustentável.
---

Desenvolvido por [Stefany Coelho] - [Seu LinkedIn ou E-mail]
