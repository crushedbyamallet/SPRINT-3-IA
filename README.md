O projeto IASI tem como objetivo transformar a gestão industrial através da aplicação de Inteligência Artificial e Machine Learning. Ele foca em três áreas críticas para a eficiência operacional e sustentabilidade das indústrias: otimização do consumo energético, manutenção preditiva de equipamentos e gestão inteligente de resíduos.

1. Previsão de Consumo Energético:
Utilizamos uma Rede Neural Densa (DNN) para prever o consumo futuro de energia com base em dados históricos de consumo, variáveis climáticas e operacionais. O modelo foi treinado com o dataset Energy Consumption Prediction do Kaggle. Sua arquitetura inclui camadas ocultas que capturam relações não lineares nos dados, possibilitando otimizar o uso de energia e reduzir custos. Isso é essencial para manter a eficiência energética em fábricas, evitando desperdícios e ajustando a produção com base nas previsões geradas.

2. Manutenção Preditiva de Equipamentos:
Esse modelo, também desenvolvido com TensorFlow, utiliza uma Rede Neural Densa (DNN) para prever falhas em equipamentos industriais, a partir de dados de sensores como temperatura e vibração. Treinado com o dataset Machine Predictive Maintenance Classification do Kaggle, ele permite identificar padrões sutis que antecedem falhas mecânicas, possibilitando a implementação de estratégias de manutenção preditiva. Com isso, as empresas podem agir de maneira proativa, reduzindo paradas inesperadas e prolongando a vida útil dos equipamentos.

3. Gestão e Classificação de Resíduos:
Para promover uma gestão sustentável dos resíduos gerados na produção industrial, desenvolvemos um modelo de classificação baseado em Redes Neurais Convolucionais (CNN). Treinado com mais de 2.000 imagens do dataset Garbage Classification do Kaggle, o modelo classifica resíduos em categorias como papel, vidro, plástico e outros, facilitando a separação e reciclagem dos materiais. Essa solução automatiza o processo de triagem de resíduos, contribuindo para práticas mais sustentáveis e redução de impactos ambientais.

Arquitetura e Justificativa:
Otimização do Consumo de Energia:
Utilizamos uma DNN com camadas totalmente conectadas. A arquitetura do modelo é composta por uma camada de entrada com variáveis como consumo histórico e condições climáticas, duas camadas ocultas com 64 e 32 neurônios usando a função de ativação ReLU, e uma camada de saída linear para prever o consumo energético. Para evitar overfitting, aplicamos regularização com dropout.

Manutenção Preditiva de Equipamentos:
O modelo de manutenção preditiva foi construído com uma DNN para classificação binária. Ele recebe dados de sensores industriais, passa por camadas ocultas que extraem padrões temporais e gera previsões de falha utilizando uma função de ativação sigmoid. Dropout e normalização de lote foram implementados para melhorar a generalização e prevenir overfitting.

Classificação de Resíduos:
O modelo de classificação de resíduos utiliza uma CNN com várias camadas convolucionais e de pooling, seguido por camadas densas para a identificação de resíduos. A arquitetura inclui três camadas convolucionais e duas densas, configuradas para classificar imagens em 12 categorias diferentes de materiais recicláveis.

![image](https://github.com/user-attachments/assets/cf5fd933-63cf-460e-a197-fd5ddbe30e1b)
![image](https://github.com/user-attachments/assets/12082e84-a43f-4a28-9266-f7c080a6fdad)
![image](https://github.com/user-attachments/assets/868ca77e-ea33-4438-976b-e61ea22f00e8)
![image](https://github.com/user-attachments/assets/585c9071-7567-45ff-88b8-5c138f4b5b81)
![image](https://github.com/user-attachments/assets/33fc2bf9-5d05-442b-8494-40f966bd736c)
![image](https://github.com/user-attachments/assets/3ba29430-ae95-4ae6-8fa5-4cc36e17dd14)
![image](https://github.com/user-attachments/assets/391cf7aa-f562-4b17-a0f3-af5193bf12a2)
![image](https://github.com/user-attachments/assets/832274f7-8613-426a-89fa-9148d1490fa4)








Bases de Dados:
Energy Consumption Prediction Dataset: Dados históricos de consumo de energia, condições climáticas e variáveis operacionais, essenciais para o modelo de previsão de consumo energético.
Machine Predictive Maintenance Classification Dataset: Registros de falhas e condições de operação de equipamentos industriais, utilizados no treinamento do modelo de manutenção preditiva.
Garbage Classification Dataset: Conjunto de dados de imagens de diferentes tipos de resíduos, utilizado para treinar o modelo de classificação.
Conclusão:
O IASI integra esses três modelos de Machine Learning em um protótipo funcional voltado para a indústria, promovendo tanto a eficiência operacional quanto a sustentabilidade. Ao aplicar essas soluções, o projeto busca não só melhorar a gestão de energia e equipamentos, mas também incentivar práticas responsáveis de reciclagem e gestão ambiental. Os resultados obtidos até o momento demonstram que a aplicação de técnicas de IA pode trazer impactos positivos significativos para a operação industrial e a sustentabilidade do setor.
