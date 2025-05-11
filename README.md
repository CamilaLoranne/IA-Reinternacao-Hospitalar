🏥 Predição de Reinternações Hospitalares com IA
Este projeto aplica Machine Learning supervisionado para prever se um paciente será reinternado em até 30 dias, com base em dados clínicos e funcionais. É voltado para fins educacionais e demonstra como técnicas de IA podem apoiar a tomada de decisão em contextos hospitalares.

📌 Objetivo
Utilizar algoritmos de aprendizado supervisionado para prever a reinternação hospitalar precoce, um dos principais desafios para a qualidade do cuidado e a sustentabilidade dos sistemas de saúde.

📊 Conjunto de Dados
O dataset contém informações de 1.000 pacientes hospitalizados, com variáveis como:
    Idade
    Sexo
    Tempo de internação
    Mobilidade
    Fisioterapia realizada
    Número de medicamentos
    Alta para casa
    Reinternado em até 30 dias (variável-alvo)

🧪 Metodologia
    Pré-processamento
        Codificação de variáveis categóricas com LabelEncoder
        Remoção de colunas irrelevantes (id_paciente, comorbidades)

    Treinamento
        Divisão dos dados (80% treino, 20% teste)
        Classificador: RandomForestClassifier (com pesos balanceados)

    Avaliação
        Matriz de confusão
        Relatório de classificação (accuracy, precision, recall, f1-score)

    Explicabilidade
        Importância das variáveis (feature_importances_)
        Visualizações com seaborn e matplotlib

📈 Resultados
    Acurácia geral: 85,5%
    Recall da classe reinternado: 49%
    Principais preditores: Idade, tempo de internação, mobilidade

🔍 Exemplos de visualizações:
Distribuição da Idade dos Pacientes
Mostra que a maioria dos pacientes tem entre 50 e 90 anos.

Importância das Variáveis segundo o Random Forest
Destaca que idade, tempo de internação e mobilidade foram os fatores mais importantes para o modelo.

💡 Conclusões e Aplicações Clínicas
Apesar de ainda limitado, o modelo apresenta desempenho razoável e pode ser útil como suporte à triagem hospitalar, ajudando a identificar pacientes com maior risco de reinternação. Isso pode orientar ações preventivas, como maior acompanhamento pós-alta ou fisioterapia intensiva.

🛠️ Tecnologias utilizadas
    Python
    pandas, scikit-learn, matplotlib, seaborn
    Google Colab
