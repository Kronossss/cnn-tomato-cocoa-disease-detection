# cnn-tomato-cocoa-disease-detection
CNN-based model for plant disease and pest diagnosis in tomato and cocoa crops, focusing on class imbalance and balanced performance metrics.

📊 Diagnóstico Agrícola com CNN
Classificação de Pragas e Doenças em Culturas de Tomate e Cacau

Este repositório contém o código-fonte desenvolvido no contexto de um Trabalho de Conclusão de Curso (TCC), cujo objetivo é a implementação, otimização e avaliação de um modelo de Inteligência Artificial baseado em Redes Neurais Convolucionais (CNNs) para o diagnóstico automatizado de pragas e doenças em culturas agrícolas, utilizando imagens digitais.

O trabalho está alinhado aos princípios da Agricultura 4.0, com foco na automação, eficiência e confiabilidade do diagnóstico agrícola.

🎯 Objetivo do Projeto

Desenvolver e validar um modelo de Deep Learning (CNNs) capaz de identificar, a partir de imagens, quatro condições distintas em culturas de tomate e cacau, garantindo desempenho equilibrado entre precisão e recall, mesmo em cenários de desbalanceamento de classes.

🌱 Classes Consideradas

O modelo realiza a classificação das seguintes categorias:

TomateSaudavel – folhas de tomate sem sinais de pragas

LeafMiner – infestação por minador de folhas no tomate

CacauSaudavel – frutos de cacau saudáveis

black_pod_rot – podridão-parda do cacau (Phytophthora spp.)

🧱 Construção e Caracterização do Dataset

Os datasets específicos que formaram a base deste estudo foram:

a) Do repositório Kaggle:
- PlantVillage Dataset: Uma coleção extensa e popular de imagens de folhas de plantas
saudáveis e doentes, da qual foram extraídas as imagens de tomateiro.
- Cacao Diseases Dataset: Um conjunto de dados focado especificamente em imagens
de frutos de cacau, contendo tanto exemplares saudáveis quanto afetados por
doenças.

b) Do repositório Mendeley Data:
- Tomato Leaf Image Dataset (TLID/PTLID): Um dataset adicional para complementar
as imagens de folhas de tomate, aumentando a variedade de exemplos para as classes
relacionadas.

<img width="609" height="179" alt="image" src="https://github.com/user-attachments/assets/8c479aa7-d935-4901-90f2-01a18793adc4" />

As imagens apresentam resoluções originais distintas. As imagens de cacau possuem
resolução de 1080 × 1080 pixels, enquanto as imagens de tomate apresentam resolução de 256
× 256 pixels.

🧠 Metodologia

O desenvolvimento do projeto foi estruturado em quatro fases principais:

Modelo Base
Implementação inicial de uma CNN para estabelecer métricas de referência em cenários balanceados e desbalanceados.

Otimizações de Treinamento
Aplicação de técnicas como:

Data Augmentation

Ponderação de classes (class_weight)

Expansão para Múltiplas Classes
Adaptação do modelo para a classificação das quatro classes de interesse.

Arquitetura Aprimorada e Seleção de Modelo

CNN customizada

Implementação de um callback personalizado para seleção do modelo

Critério de escolha baseado em precisão e recall por classe, e não apenas na acurácia geral.

📈 Resultados

Acurácia de 95% no conjunto de validação

Todas as classes com precisão e recall superiores a 0.85

Teste externo com imagens inéditas, atingindo 90% de acurácia

Demonstração de boa capacidade de generalização do modelo

Os resultados confirmam que estratégias focadas no equilíbrio das métricas são fundamentais para sistemas de diagnóstico agrícola confiáveis.

<img width="801" height="707" alt="image" src="https://github.com/user-attachments/assets/d3c080e9-9a36-4fe2-b0a0-f60d0fee7dad" />

🛠️ Tecnologias Utilizadas

Python

TensorFlow / Keras

NumPy

Pandas

Scikit-learn

Matplotlib / Seaborn
```text
📁 Estrutura do Repositório (exemplo)
├── dataset/
│   ├── treino/
│   ├── validacao/
│   └── teste/
├── models/
├── notebooks/
├── src/
│   ├── treinamento.py
│   ├── avaliacao.py
│   └── callbacks.py
├── README.md
└── requirements.txt


(A estrutura pode variar conforme a organização final do projeto)

⚠️ Aviso Importante

Este projeto possui finalidade exclusivamente acadêmica e educacional.
Os resultados obtidos não garantem desempenho estatístico absoluto em ambientes reais de produção agrícola.

👨‍🎓 Autor

Igor Alex Farias
Trabalho de Conclusão de Curso – Graduação
Área: Inteligência Artificial / Visão Computacional / Agricultura 4.0 / Redes Neurais Convolucionais / Desbalanceamento de Classes /  Diagnóstico Agrícola. 
