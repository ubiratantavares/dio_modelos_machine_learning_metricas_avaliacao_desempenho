# DIO - Modelos de Machine Learning - Métricas de Avaliação de Desempenho

## Introdução para métricas de avaliação

O desempenho de um modelo de machine learning é um fator crucial que determina sua utilidade em aplicações reais. 

Métricas de avaliação são ferramentas quantitativas que permitem medir a eficácia de um modelo ao realizar previsões. 

Elas fornecem uma base objetiva para comparar diferentes algoritmos, ajustar hiperparâmetros e determinar se um modelo atende aos requisitos do problema em questão. 

A escolha das métricas depende do tipo de problema: classificação, regressão ou clustering, por exemplo. 

Além disso, fatores como o equilíbrio entre classes, impacto de falsos positivos ou negativos e requisitos de precisão versus robustez podem influenciar na seleção da métrica mais apropriada.

## Tipos de métricas de avaliação de desempenho

### 1. Métricas para problemas de classificação
  
- **Acurácia**: Proporção de previsões corretas. Indicada para classes balanceadas, mas pode ser enganosa em datasets desbalanceados.  

- **Precisão**: Proporção de verdadeiros positivos em relação a todas as previsões positivas. Útil quando falsos positivos têm alto custo.  

- **Revocação (Recall)**: Proporção de verdadeiros positivos em relação ao total de exemplos positivos reais. Essencial quando a captura de todos os casos positivos é crucial.  

- **F1-Score**: Média harmônica entre precisão e revocação, balanceando ambos.  

- **Matriz de Confusão**: Apresenta verdadeiros positivos, falsos positivos, verdadeiros negativos e falsos negativos, proporcionando uma visão detalhada do desempenho.  

- **AUC-ROC**: Mede a capacidade do modelo em distinguir entre classes, representando a relação entre taxa de verdadeiros positivos e falsos positivos.

### 2. Métricas para problemas de regressão
  
- **Erro Médio Absoluto (MAE)**: Média das diferenças absolutas entre valores previstos e reais.  

- **Erro Quadrático Médio (MSE)**: Média dos quadrados das diferenças, sensível a grandes erros.  

- **Raiz do Erro Quadrático Médio (RMSE)**: Raiz quadrada do MSE, mantendo as mesmas unidades da variável alvo.  

- **Coeficiente de Determinação (R²)**: Mede a proporção de variação explicada pelo modelo em relação à variação total dos dados.  

### 3. Métricas para problemas de clustering**  

- **Índice de Silhueta**: Avalia a separação entre clusters e a coesão interna.  

- **Coeficiente de Rand Ajustado**: Mede a similaridade entre clusters previstos e verdadeiros.  

- **V-Measure**: Avalia homogeneidade e completude do clustering.

## Métricas de avaliação na prática

Na prática, a escolha de métricas deve alinhar-se ao objetivo do projeto. Por exemplo:  

- Em sistemas de detecção de fraudes, a **revocação** pode ser mais importante do que a precisão, já que é crucial identificar todos os casos suspeitos.  

- Em diagnósticos médicos, o **F1-Score** pode ser preferido para balancear precisão e revocação.  

- Em modelos preditivos financeiros, métricas como **MAE** ou **RMSE** são frequentemente utilizadas para garantir previsões precisas e confiáveis.

Além disso, a validação cruzada é amplamente empregada para garantir que as métricas reflitam o desempenho do modelo em dados não vistos. 

Ferramentas como gráficos de curva ROC, análise residual e interpretação de métricas complementares são práticas recomendadas para obter uma visão abrangente do desempenho do modelo.

Por fim, métricas isoladas nunca devem ser a única base para avaliar um modelo. 

A análise deve considerar o contexto, os objetivos do problema e as possíveis implicações práticas das decisões tomadas com base nas previsões do modelo.
