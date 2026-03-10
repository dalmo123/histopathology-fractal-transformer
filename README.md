# Histopathology Fractal Transformer

Este repositório contém o pipeline experimental desenvolvido no Trabalho de Conclusão de Curso intitulado:

**"Investigação de Modelos Vision Transformers e Representações de Geometria Fractal para Classificação de Lesões Histológicas"**

O objetivo deste trabalho é investigar o uso de **Vision Transformers (ViT)** e **representações baseadas em geometria fractal** para a classificação de imagens histopatológicas do epitélio oral.

---

# Visão Geral

A classificação automática de imagens histopatológicas pode auxiliar no diagnóstico de displasias do epitélio oral. Neste trabalho são avaliadas diferentes representações de imagens com o objetivo de analisar seu impacto no desempenho de modelos de aprendizado profundo.

Os experimentos consideram diferentes tipos de representação da imagem:

- Imagens histopatológicas originais
- Representação Sequencial (SR)
- Representação baseada em Recurrence Plot (RecPlot)

Os modelos são avaliados utilizando métricas clássicas de classificação.

---

# Base de Dados

Os experimentos foram conduzidos utilizando o banco de dados **Oral Epithelium DB**, que contém imagens histopatológicas do epitélio oral classificadas em diferentes graus de displasia.

Classes consideradas:

- Healthy
- Mild
- Moderate
- Severe

Foram avaliados diferentes cenários de classificação binária, incluindo:

- Healthy vs Mild  
- Healthy vs Moderate  
- Healthy vs Severe  
- Mild vs Moderate  
- Mild vs Severe  
- Moderate vs Severe  

---

## Dataset e Representações Geradas

Devido ao tamanho do conjunto de dados, as imagens utilizadas nos experimentos não estão armazenadas diretamente neste repositório.

O dataset completo, incluindo:

- Imagens histopatológicas originais
- Representações sequenciais (SR)
- Representações fractais geradas
- Representações RecPlot

está disponível no Google Drive:

https://drive.google.com/drive/folders/1dmbCKQsBC1WIs54WDj6lukdVmoNNwQan?usp=sharing

# Representações Fractais

A geração das representações fractais utilizadas neste trabalho foi realizada utilizando a implementação disponibilizada por:

**Carvalho, Rafael Henrique de Oliveira**

Repositório:

https://github.com/Carvarafael/Fractal-Reshape-representation

Esse repositório contém a implementação da técnica **Fractal Reshape Representation**, utilizada para gerar as representações fractais aplicadas neste estudo.

---
# Experimentos

Os experimentos realizados neste trabalho incluem:

### Imagens Originais

Classificação utilizando diretamente as imagens histopatológicas originais.

### Representação Sequencial (SR)

Avaliação do desempenho dos modelos utilizando representações sequenciais das imagens.

### Representação RecPlot

Classificação utilizando representações baseadas em **Recurrence Plot**.

### Estudo de Ablação

Avaliação da contribuição de diferentes componentes da arquitetura por meio da desativação seletiva de módulos da rede.

---

# Métricas de Avaliação

O desempenho dos modelos foi avaliado utilizando as seguintes métricas:

- Acurácia
- Precisão
- Recall
- F1-score
- Matriz de Confusão

---

# Resultados

Os resultados experimentais gerados durante os testes estão disponíveis na pasta **Resultados**.

Esses resultados incluem:

- Métricas de classificação
- Matrizes de confusão
- Comparações entre diferentes representações de imagem

# Visualização Interativa dos Resultados

Para facilitar a análise dos resultados obtidos nos experimentos, foi desenvolvida uma interface web que permite visualizar alguns dos gráficos gerados durante a avaliação dos modelos.

A aplicação pode ser acessada no link abaixo:

https://vits-fractal-oral-lesions.lovable.app/

Nessa interface é possível explorar visualmente alguns dos resultados experimentais, incluindo gráficos comparativos entre diferentes representações de imagem e cenários de classificação.
---

# Autor

Dalmo Scalon Inacio  
Universidade Federal de Uberlândia (UFU)

---

# Observação

Este repositório foi desenvolvido para fins **acadêmicos e de pesquisa** no contexto do Trabalho de Conclusão de Curso.
