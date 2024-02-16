# Modelo de Previsão com Microsoft Azure - Utilizando o Aprendizado de Máquina Automatizado no Azure Machine Learning

ℹ️ Utilização do recurso de aprendizado de máquina automatizado no Azure Machine Learning para treinar, avaliar, implantar e testar um modelo de previsão de alugueis de bicicletas.

📝 **Objetivos:**
- Treinar um modelo de previsão de alugueis de bicicletas.
- Avaliar o desempenho do modelo.
- Implantar e testar o modelo.

ℹ️ **Passo a Passo:**

1. **Criação de um espaço de trabalho no Azure Machine Learning:**
   - Acessei o portal do Azure e naveguei até o serviço Azure Machine Learning.
   - Criei um novo espaço de trabalho ou selecionei um espaço de trabalho existente.

2. **Criação de um novo trabalho de ML automatizado:**
   - Acessei a página ML Automatizado no Azure Machine Learning Studio.
   - Criei um novo trabalho de ML automatizado com as configurações especificadas, avançando quando necessário pela interface do usuário.

3. **Avaliação do melhor modelo:**
   - Quando o trabalho automatizado de aprendizado de máquina foi concluído, revisei o melhor modelo treinado.
   - Na guia Visão geral do trabalho automatizado de aprendizado de máquina, observei o melhor resumo do modelo.
   - Selecionei o texto em Nome do algoritmo do melhor modelo para visualizar seus detalhes.
   - Selecionei a guia Métricas e selecionei os gráficos residuais e predito_true se eles ainda não estivessem selecionados.
   - Revisei os gráficos que mostram o desempenho do modelo.

4. **Implantação e teste do modelo:**
   - Na guia Modelo do melhor modelo treinado pelo trabalho automatizado de machine learning, selecionei Implantar e usei a opção de serviço Web para implantar o modelo com as configurações especificadas.
   - Aguardei o início da implantação e aguardei até que o status da implantação mudasse para Succeeded.
   - No Azure Machine Learning Studio, no menu esquerdo, selecionei Endpoints e abri o ponto final em tempo real de previsão de alugueis.
   - Na página do endpoint em tempo real de previsão de alugueis, visualizei a guia Teste.
   - No painel Dados de entrada para testar o endpoint, substituí o modelo JSON pelos dados de entrada especificados.
   - Cliquei no botão Testar.
   - Revisei os resultados do teste, que incluem um número previsto de aluguéis com base nos recursos de entrada.
