# 🔐 Predição de Fraudes Financeiras

Projeto desenvolvido como trabalho final do curso de **Cientista de Dados** da EBAC.

---

## 📌 Sobre o Projeto

Projeto de Machine Learning para detecção de fraudes em transações financeiras, utilizando técnicas avançadas de ciência de dados e algoritmos de classificação. Desenvolvido para compor meu portfólio, este projeto demonstra habilidades em análise de dados, engenharia de features, modelagem, avaliação e comunicação de resultados.

## 🎯 Objetivo
Desenvolver um modelo preditivo capaz de identificar transações fraudulentas com alta precisão e recall, minimizando falsos positivos e negativos. O objetivo é propor uma solução que possa ser integrada a sistemas de monitoramento financeiro, contribuindo para a segurança das operações e redução de perdas causadas por fraudes.

## 🧾 Base de Dados

Utilizei um conjunto de dados real de transações de cartão de crédito, altamente desbalanceado, contendo apenas 0,17% de casos de fraude. As variáveis sensíveis foram transformadas por PCA, preservando a confidencialidade. As principais variáveis são:
- **Time**: tempo em segundos desde a primeira transação
- **Amount**: valor da transação
- **Class**: alvo (0 = legítima, 1 = fraude)
- 28 componentes principais (PCA)

##  🗂️ Estrutura do Projeto

- Análise exploratória e visualização de dados
- Engenharia de features (ex: criação de variáveis temporais e de risco)
- Pré-processamento e balanceamento das classes (SMOTE)
- Modelagem com Regressão Logística e XGBoost
- Otimização de hiperparâmetros
- Avaliação com validação cruzada e holdout
- Visualização de métricas e resultados

## 📈 Resultados
- O modelo XGBoost, após tuning, apresentou:
  - **Precisão (fraude)**: 85,15%
  - **Recall (fraude)**: 82,65%
  - **F1-score**: 81,00%
  - **AUC-ROC**: 0.9810
  - Baixa taxa de falsos positivos e alta capacidade de generalização
- Insights relevantes: fraudes ocorrem com maior frequência na madrugada e em valores baixos.

## 🧪 Tecnologias e Bibliotecas
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Imbalanced-learn
- XGBoost

## ▶️ Como Rodar
1. Clone o repositório:
   ```bash
   git clone https://github.com/anapaulads/predicao-fraude-financeira.git
   cd predicao-fraude-financeira
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute o notebook `Projeto_Final_Predicao_Fraude_Bancaria.ipynb` em seu ambiente Jupyter.

## 💡 Insights
- Fraudes tendem a ocorrer em horários de menor movimentação e em transações de baixo valor.
- A engenharia de features temporais e o balanceamento das classes foram essenciais para o sucesso do modelo.
- O XGBoost se mostrou superior à Regressão Logística, conciliando precisão e recall.

## 🫱🏾‍🫲🏽 Contribuições
Sugestões, melhorias e novas ideias são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

## ✍🏾 Autoria
Projeto desenvolvido por Ana Paula Dias, como parte da formação em Ciência de Dados pela EBAC.
