*O IASI (Inteligência de Avaliação de Sustentabilidade Industrial) busca melhorar a gestão industrial utilizando Inteligência Artificial e Machine Learning para ampliar processos em três áreas principais: consumo de energia, manutenção de equipamentos e gestão de resíduos.*


***Entendendo conceitos de arquitetura***


Em aprendizado de máquina e da inteligência artificial, arquitetura de rede neural refere-se à estrutura e organização dos componentes de uma rede neural. Essa estrutura é essencial para definir como os dados são processados, transformados e utilizados para fazer previsões ou classificações. Entre as diversas arquiteturas de redes neurais, duas das mais comuns são a Rede Neural Densa (DNN) e a Rede Neural Convolucional (CNN). Cada uma dessas arquiteturas é projetada para atender a necessidades específicas de processamento de dados.

***DNN (Deep neural network) - Rede neural densa***

A DNN, ou Rede Neural Densa, é uma arquitetura composta por múltiplas camadas de neurônios, onde cada neurônio de uma camada está completamente conectado a todos os neurônios da próxima camada. Essa conexão total é a razão pela qual ela é chamada de "densa". As DNNs são particularmente eficazes para lidar com dados estruturados e tabulares, como tabelas de dados e séries temporais.

**Características:**

Camadas densas: Cada camada está totalmente conectada à camada seguinte. Isso permite que a rede capture interações complexas entre variáveis.
Camadas ocultas: As redes possuem múltiplas camadas ocultas entre a entrada e a saída, que introduzem não-linearidades através de funções de ativação como ReLU (Rectified linear unit) ou Sigmoid.
Regularização: Técnicas como Dropout são usadas para evitar overfitting, garantindo que o modelo generalize bem para novos dados.
Aplicações comuns: A DNN é ideal para tarefas como previsão de valores numéricos e classificação de dados tabulares. Por exemplo, no projeto de previsão de consumo de energia, uma DNN é utilizada para analisar dados históricos e prever demandas futuras com base em variáveis como temperatura e ocupação.

***CNN (Convolutional neural network) - Rede neural convolucional***

A CNN, ou rede neural convolucional, é uma arquitetura projetada para processar dados com uma estrutura espacial, como imagens e vídeos. Em vez de usar conexões totalmente densas, as CNNs empregam camadas convolucionais para detectar e extrair características locais dos dados.

**Características:**

Camadas convolucionais: Aplicam filtros para detectar características locais, como bordas e texturas em imagens. Esses filtros ajudam a capturar padrões espaciais.
Pooling: Camadas de pooling são usadas para reduzir a dimensionalidade dos dados e manter as características mais relevantes.
Camadas densas: Após a extração de características, camadas densas são usadas para a classificação final ou outras tarefas.
Aplicações comuns: As CNNs são ideais para tarefas de reconhecimento de padrões visuais e análise de imagens. No projeto de gestão e classificação de resíduos, uma CNN é treinada para identificar e classificar diferentes tipos de lixo a partir de imagens, facilitando a triagem automatizada e a gestão eficiente dos resíduos.

A Importância das arquiteturas
A escolha da arquitetura de rede neural é fundamental para o sucesso de um projeto de aprendizado de máquina. A arquitetura deve ser alinhada com o tipo de dados e a tarefa específica a ser realizada. Enquanto as DNNs são adequadas para dados tabulares e numéricos, as CNNs são a escolha ideal para dados espaciais e visuais. 


****Como isso se aplica no nosso projeto?****

***1. Previsão de consumo energético***

Utilizamos uma Rede Neural Densa (DNN) para prever o consumo futuro de energia com base em dados históricos de consumo, variáveis climáticas e operacionais. O modelo foi treinado com o dataset Energy Consumption Prediction do Kaggle. Sua arquitetura inclui camadas ocultas que capturam relações não lineares nos dados, possibilitando otimizar o uso de energia e reduzir custos. Isso é essencial para manter a eficiência energética em fábricas, evitando desperdícios e ajustando a produção com base nas previsões geradas.

***2. Manutenção preditiva de equipamentos***

Esse modelo, também desenvolvido com TensorFlow, utiliza uma Rede Neural Densa (DNN) para prever falhas em equipamentos industriais, a partir de dados de sensores como temperatura e vibração. Treinado com o dataset Machine Predictive Maintenance Classification do Kaggle, ele permite identificar padrões sutis que antecedem falhas mecânicas, possibilitando a implementação de estratégias de manutenção preditiva. Com isso, as empresas podem agir de maneira proativa, reduzindo paradas inesperadas e prolongando a vida útil dos equipamentos.

***3. Gestão e classificação de resíduos***

Para promover uma gestão sustentável dos resíduos gerados na produção industrial, desenvolvemos um modelo de classificação baseado em Redes Neurais Convolucionais (CNN). Treinado com mais de 2.000 imagens do dataset Garbage Classification do Kaggle, o modelo classifica resíduos em categorias como papel, vidro, plástico e outros, facilitando a separação e reciclagem dos materiais. Essa solução automatiza o processo de triagem de resíduos, contribuindo para práticas mais sustentáveis e redução de impactos ambientais.

![image](https://github.com/user-attachments/assets/cf5fd933-63cf-460e-a197-fd5ddbe30e1b)
![image](https://github.com/user-attachments/assets/12082e84-a43f-4a28-9266-f7c080a6fdad)
![image](https://github.com/user-attachments/assets/868ca77e-ea33-4438-976b-e61ea22f00e8)
![image](https://github.com/user-attachments/assets/585c9071-7567-45ff-88b8-5c138f4b5b81)
![image](https://github.com/user-attachments/assets/33fc2bf9-5d05-442b-8494-40f966bd736c)
![image](https://github.com/user-attachments/assets/3ba29430-ae95-4ae6-8fa5-4cc36e17dd14)
![image](https://github.com/user-attachments/assets/391cf7aa-f562-4b17-a0f3-af5193bf12a2)
![image](https://github.com/user-attachments/assets/832274f7-8613-426a-89fa-9148d1490fa4)


***Bases de Dados***

**Energy Consumption Prediction Dataset:** https://www.kaggle.com/datasets/mrsimple07/energy-consumption-prediction

Dados históricos de consumo de energia, condições climáticas e variáveis operacionais, essenciais para o modelo de previsão de consumo energético.

**Machine Predictive Maintenance Classification Dataset:** https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification

Registros de falhas e condições de operação de equipamentos industriais, utilizados no treinamento do modelo de manutenção preditiva.

**Garbage Classification Dataset:** https://www.kaggle.com/datasets/mostafaabla/garbage-classification

Conjunto de dados de imagens de diferentes tipos de resíduos, utilizado para treinar o modelo de classificação.



