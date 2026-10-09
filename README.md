# Segmentação de clientes de e-commerce (Olist)

> 🚧 **Em andamento:** SQL, EDA e Machine Learning concluídos; deep learning, IA generativa e painel em construção. Projeto de ponta a ponta, não supervisionado, seguindo o CRISP-DM.

**Cliente (cenário):** marketplace de e-commerce brasileiro.
**Pergunta de negócio:** que perfis de clientes existem e como o CRM deve falar com cada um?

**Ferramentas:** SQL (SQLite) · Python (pandas, scikit-learn, Keras) · IA generativa (LLM) · Tableau Public · Google Colab

## Etapas
| Etapa (CRISP-DM) | Notebook | Status |
|---|---|---|
| Entender os dados com SQL | [00 · carga](notebooks/00_setup_carga_sql.ipynb) · [01 · perguntas de negócio](notebooks/01_sql_perguntas_negocio.ipynb) | ✅ |
| Análise exploratória | [02 · EDA](notebooks/02_eda.ipynb) | ✅ |
| Modelagem (Machine Learning) | [03 · RFM + K-Means](notebooks/03_segmentacao_kmeans.ipynb) | ✅ |
| Modelagem (Deep Learning) | [04 · autoencoder](notebooks/04_deep_learning_autoencoder.ipynb) | ⏳ |
| IA generativa | [05 · personas a partir dos comentários](notebooks/05_ia_generativa_personas.ipynb) | ⏳ |
| Implantação | [06 · dados para o Tableau](notebooks/06_exportar_tableau.ipynb) · painel no Tableau Public | ⏳ |

## Resultados até aqui
- **Retenção é o maior desafio:** só 3,0% dos clientes compraram mais de uma vez, e menos de 1% de cada coorte volta no mês seguinte.
- **Atraso derruba a satisfação:** a nota média cai de 4,29 (no prazo) para 1,70 (mais de 7 dias de atraso).
- **4 segmentos com K-Means:** o segmento *Alto valor* reúne 29,8% dos clientes e 57,5% da receita, mas quase todos com compra única. Converter esse grupo na 2ª compra é a principal alavanca de CRM.

## Dados
[Brazilian E-Commerce Public Dataset by Olist](https://github.com/olist/work-at-olist-data): 9 tabelas, cerca de 99 mil pedidos (2016–2018). Licença MIT, © 2019 Olist. Os arquivos não ficam neste repositório: o notebook 00 baixa direto da fonte oficial.

## Como rodar
1. Abra o notebook 00 no Colab pelo botão "Abrir no Colab" e execute. Ele cria `olist.db` no seu Google Drive.
2. Siga os notebooks na ordem.

---
**Autora:** Jéssica Priscila de Oliveira Martins · [LinkedIn](https://www.linkedin.com/in/jessica-oliveira-martins/) · [Portfólio](https://claude.ai/artifact/YPyaaqo16QuwKBKGw9VF5m)
