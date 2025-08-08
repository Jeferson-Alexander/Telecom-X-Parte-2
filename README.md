# Telecom-X-Parte-2
Telecom X - Previsão de Cancelamento de Clientes (Churn)
Projeto completo de Data Science para previsão de evasão (churn) de clientes da Telecom X utilizando Python e Scikit-learn.
Autor: Jeferson Alexander
Descrição do Projeto
Este projeto tem como objetivo prever a evasão de clientes na empresa Telecom X, utilizando dados históricos dos clientes com informações demográficas, de consumo e pagamento. São aplicados processos de pré-processamento, modelagem utilizando diversos algoritmos (Regressão Logística, Random Forest, KNN e SVM), análise da importância das variáveis e avaliação dos modelos.
Bibliotecas Utilizadas
•	pandas, numpy: manipulação de dados
•	matplotlib, seaborn: visualização gráfica
•	scikit-learn: modelagem, preprocessamento e métricas
•	imblearn: balanceamento com SMOTE
•	joblib: salvamento dos modelos treinados
Estrutura do Código
1.	Importação das Bibliotecas
Importação de pacotes essenciais para análise, modelagem e visualização.
2.	Carregamento e Renomeação da Base de Dados
Leitura do arquivo CSV, renomeação das colunas para melhor entendimento.
3.	Análise Inicial
Exploração das variáveis, distribuição do target (churn), boxplots para variáveis numéricas.
4.	Visualizações Adicionais
Análise gráfica das variáveis categóricas relacionadas ao churn.
5.	Pré-processamento
Codificação das variáveis categóricas com one-hot encoding, conversão do target para formato numérico e verificação de valores nulos.
6.	Correlação
Matriz de correlação para verificar relações entre variáveis numéricas.
7.	Divisão Feature/Target e Balanceamento com SMOTE
Separação dos dados em features e target, balanceamento da base para evitar viés.
8.	Divisão Treino/Teste
Separação dos dados balanceados em conjuntos de treino e teste.
9.	Modelagem e Avaliação
Treinamento e avaliação dos modelos: Regressão Logística, Random Forest, KNN e SVM.
10.	Interpretação e Importância das Variáveis
Avaliação da importância das variáveis para cada modelo, utilizando coeficientes e permutação.
11.	AUC-ROC e Curvas ROC
Avaliação comparativa da performance dos modelos via AUC e curvas ROC.
12.	Exportação dos Modelos
Salvamento dos modelos treinados e arquivo CSV com importância das variáveis do Random Forest.
Como Usar
1.	Coloque o arquivo telecomx_data_gold.csv no caminho especificado no código ou ajuste o caminho na linha de leitura do CSV.
2.	Execute o script em um ambiente Python com as bibliotecas listadas instaladas.
3.	Os gráficos e métricas serão exibidos para análise.
4.	Os modelos serão salvos em arquivos .pkl para uso futuro.
5.	O arquivo importancia_rf.csv será gerado com a importância das variáveis do modelo Random Forest.
Principais Resultados e Insights
•	Clientes que permanecem menos tempo e aqueles com cobrança mensal maior têm maior probabilidade de cancelamento.
•	Tipos de contrato, método de pagamento e suporte técnico são variáveis importantes para previsão.
•	O modelo Random Forest apresentou melhor desempenho geral comparado à Regressão Logística.
•	KNN e SVM também foram treinados, com análise da importância via permutação e coeficientes.
Dependências e Instalação
Recomenda-se usar um ambiente virtual. Para instalar as bibliotecas necessárias:
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn joblib

Estrutura de Arquivos
|-- telecomx_previsao_churn.py  # Script principal com todo o código
|-- telecomx_data_gold.csv      # Base de dados (não incluída no repositório)
|-- modelo_logistica.pkl        # Modelo Regressão Logística salvo
|-- modelo_randomforest.pkl     # Modelo Random Forest salvo
|-- importancia_rf.csv          # Importância das variáveis do RF

Caso queira, posso ajudar a organizar esse projeto com notebooks ou até scripts separados para análise, modelagem e avaliação.
Quer que eu gere algo mais para complementar seu repositório GitHub?


