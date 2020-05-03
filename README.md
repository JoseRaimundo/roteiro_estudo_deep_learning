
### Descrição do repositório


Este repositório funciona como uma base de consulta sobre tópicos relacionados a deep learning. O objetivo deste repositório é catalogar conteúdos e informações importantes sobre deep learning que foram úteis ou interessantes durante minhas experiências.

#### Linguagem de Programação

#### Python
Atualmente Python é uma das principais linguagens de programação para quem deseja trabalhar com Machine Learning. Esta linguagem oferece uma abstração mais clara e fácil de usar, possibilitando uma curva de aprendizado maior. As melhores bibliotecas  de ML mais  oferecem interface de aplicação para que você possa programar em Python e, ao executar o código, elas utilizam funções em C/C++ por baixo dos panos, devido à velocidade destas linguagens. 

| Titulo | Tipo | Nível | Qualidade | Link | Descrição
|--|--|--|--|--|--|
| Pycubator | Curso | Iniciante | 4 | [Link](http://df.python.org.br/pycubator/index.html)| Curso rápido bem completo
|Python para Zumbis|Curso|4|Iniciante| [Link](https://www.pycursos.com/python-para-zumbis/)| Curso básico



#### Manipulação de dados

**Obtenção**: O acesso aos dados pode ser realizado de diversas maneiras, seja por um arquivo no seu computador ou por um serviço API online ( como uma requisição HTTP GET). Normalmente, a forma mais comum de obter dados, é por meio de um arquivo **.csv**.

Exemplo de acesso a dados em arquivo csv. Mais detalhes ([link](https://www.linkedin.com/pulse/lendo-arquivos-csv-com-pandas-rog%C3%A9rio-guimar%C3%A3es-de-campos-j%C3%BAnior/))

    import pandas as pd
    dataframe  =  pl.read_csv('local_do_meu_arquivo/arquivo.csv)
    print(dataframe.head())


**Manipulação de dados** : Há diversas bibliotecas para manipular dados no seu código, porém as mais utilizadas em data-science são 



| Titulo | Tipo | Nível | Qualidade | Link | Descrição
|--|--|--|--|--|--|
| 28 comandos rápidos | Tutorial | Intermediário | 4 | [Link](https://paulovasconcellos.com.br/28-comandos-%C3%BAteis-de-pandas-que-talvez-voc%C3%AA-n%C3%A3o-conhe%C3%A7a-6ab64beefa93)| Conteúdo para acesso rápido - bom
|Introdução ao Pandas | Tutorial | Intermediário| 4 | [Link](https://medium.com/data-hackers/uma-introdu%C3%A7%C3%A3o-simples-ao-pandas-1e15eea37fa1)| Muito bom para estudar
|A Complete Introduction| Tutorial| Intermediário| 3 | [Link](https://www.learndatasci.com/tutorials/python-pandas-tutorial-complete-introduction-for-beginners/)| Só use se quiser se aprofundar

**Salvando dados**: As vezes é necessário salvar o dataframe pandas ou até mesmo outros dados que você quer manter registrado em arquivo, veja o exemplo para salvar em csv (Mais detalhes [link](https://medium.com/data-hackers/uma-introdu%C3%A7%C3%A3o-simples-ao-pandas-1e15eea37fa1)).

    df = pd.DataFrame({'Aluno' : ["Wilfred", "Abbie", "Harry", "Julia", "Carrie"],  
                   'Faltas' : [3,4,2,1,4],  
                   'Prova' : [2,7,5,10,6],  
                   'Seminário': [8.5,7.5,9.0,7.5,8.0]})  
	df.to_csv("aulas.csv")
	pd.read_csv("aulas.csv")

Resultado:

![enter image description here](https://miro.medium.com/max/668/1*KqH6anQf3HhAtDnq-6uBdg.png)


#### Data mining

Limpeza de dados
Padronização de dados
Tipos de dados
Features selections
Features eliminations

#### Conceitos de Machine Learning

| Titulo | Tipo | Nível | Qualidade | Link | Descrição
|--|--|--|--|--|--|
| An introduction to machine learning with scikit-learn | Tutorial | Avançado | 5 | [Link](https://scikit-learn.org/stable/tutorial/basic/tutorial.html) | Muito bom
**Tipos de aprendizado**: Há três principais tipos de aprendizados, supervisionado, não supervisionado e por reforço. O mais comum é o aprendizado supervisionado, porém é sempre bom conhecer os outros, pois vai depender muito da abordagem do seu problema e da disponibilização dos dados.

| Titulo | Tipo | Nível | Qualidade | Link | Descrição
|--|--|--|--|--|--|
| Os Três Tipos de ML | Tutorial | Iniciante | 4 | [Link](https://lamfo-unb.github.io/2017/07/27/tres-tipos-am/)| Bom para aprender
| Tipos de aprendizagem | Tutorial | Iniciante | 4 | [Link](https://medium.com/brasil-ai/tipos-de-aprendizagem-1c1339f73bdf) | Bom para aprender



#### Métricas

Mais a frente eu explico resumidamente as métricas utilizando o poster apresentado por Paulo Vasconcelos [link](https://paulovasconcellos.com.br/como-saber-se-seu-modelo-de-machine-learning-est%C3%A1-funcionando-mesmo-a5892f6468b). Porém estes links na tabela são ótimos, recomendo a leitura.


| Titulo | Tipo | Nível | Qualidade | Link | Descrição
|--|--|--|--|--|--|
| Avaliando o modelo de ML | Tutorial | Intermediário | 5 | [Link](https://paulovasconcellos.com.br/como-saber-se-seu-modelo-de-machine-learning-est%C3%A1-funcionando-mesmo-a5892f6468b) | Muito bom
| Matriz de Confusão e AUC ROC | Tutorial | Intermediário | 5 | [Link](https://medium.com/data-hackers/matriz-de-confus%C3%A3o-e-auc-roc-f7e446dca107) | Bem completo
|As Métricas Mais Populares| Tutorial | Intermediário | 4| [Link](https://www.mariofilho.com/as-metricas-mais-populares-para-avaliar-modelos-de-machine-learning/)| Explicação mais direta
|As Métricas Mais Comuns de ML| Tutorial | Intermediário | 5| [Link](https://medium.com/as-m%C3%A1quinas-que-pensam/m%C3%A9tricas-comuns-em-machine-learning-como-analisar-a-qualidade-de-chat-bots-inteligentes-introdu-57ff30424192)| Leia todos os 4 postes


#### Matriz de confusão

A Matriz de confusão, nos mostras as taxas de acertos e erros do nosso modelo. 

Exemplo: Imagine que seu modelo tem que classificar se uma foto é de um gato ou não. Em seu dataset há 50 fotos de gatos e 50 fotos que não são de gatos. Após treinar o modelo, você roda a matriz de confusão e descobre que das 50 fotos de gatos, seu modelo classificou 25 corretamente, enquanto das 50 fotos de não gato, ele classificou 40. A matriz ficaria mais ou menos assim:

![enter image description here](https://miro.medium.com/max/1346/1*s0aMRNsHq7A3bCA9gX_qXQ.png)


Dessa imagem podemos extrair: 

 - **Verdadeiro Positivo**: Quando de casos que o modelo previu como gato e que de fato é gato (acertou).
 - **Verdadeiro negativo**: Quantidade de casos que o modelo previu como não gato, e que de fato não são gatos. (acertou).
 - **Falso positivo**: Quantidade de casos não gatos que ele previu como gato (errou).
 - **Falso negativo**: Quantidade de casos de imagem de não gato que o modelo  previu como gato (errou).

#### Métricas Básicos

Para saber como seu modelo está funcionando, é necessário fazer algum tipo de medição, para isso temos as métricas. Utilizando a matriz apresentada anteriormente, temos:

**Acurácia (Accuracy)**: a proporção de casos que foram corretamente previstos, sejam eles verdadeiro positivo ou verdadeiro negativo. Em nosso exemplo:  **65/100 = 0,65**

**Sensibilidade (Sensibility):** a proporção de  **casos positivos**  que foram identificados corretamente. No nosso caso, o cálculo é feito da seguinte forma:  **25/50 = 0,5**  (25 imagens de gatos foram previstas corretamente em um total de 50 imagens);

**Especificidade (Specificity):**  a proporção de  **casos negativos**  que foram identificados corretamente. De forma semelhante a sensibilidade, calculamos a especificidade assim:  **40/50 = 0,8**;

#### Curva ROC e AUC

A Receiver Operating Characteristics (ROC), é ilustrada pela plotagem da  **sensibilidade**  — a taxa de Verdadeiro Positivo —  e a **especificidade**  — a taxa de Falso Positivo. **Quanto mais alto e mais distante da linha diagonal a sua curva estiver, melhor.** 

![enter image description here](https://miro.medium.com/max/976/0*ETMky-ZSiAevQfYG.png)

Area Under the ROC Curve (AUC) é um número de 0 a 1 que mostra como seu modelo está performando ao utilizar como base para o cálculo a Taxa de Falso Positivo e a Taxa de Verdadeiro Positivo. interpretá-lo é fácil:  **quanto mais próximo de 1 esse número estiver, melhor**. 

Estes métricas dão a ideia de quão bem as classes estão separadas como explica o Marcos Silva no [link](https://medium.com/data-hackers/matriz-de-confus%C3%A3o-e-auc-roc-f7e446dca107)

![enter image description here](https://miro.medium.com/max/1312/0*OsG9Go7PzMWu5DNP)

#### Cross Validation

Cross-Validation é uma das melhores técnicas para saber se o seu modelo generaliza bem. Quando você executa seu modelo várias vezes, pode receber valores diferentes devido a vários fatores (dataset, quantidade de épocas, modelo ruim e etc).  **Esse é um tipo de problema que você pode resolver com o Cross-Validation**.  Essa técnica que visa entender como seu modelo generaliza, ou seja, como ele se comporta quando vai prever um dado que nunca viu. 

Cross-Validation serve para criar diferentes conjuntos de treino e teste, treinar o modelo e ter certeza de que ele está performando bem. Nesse caso, **ao invés de usarmos apenas um conjunto de teste para validar nosso modelo, utilizaremos N outros a partir dos mesmos dados**.

Existem vários métodos de Cross-Validation, aqui vamos ver apenas o K-Fold, esse método consiste em dividir seu dataset K vezes.


![enter image description here](https://miro.medium.com/max/1400/0*P--gozwUfJ0TKtEp.png)

No exemplo acima, o dataset foi dividido em 5 partes, para cada uma dessas partes, o modelo irá usar 4 partes (K-1) para treinar, enquanto usará 1 parte para validar. Ao final do processo, quando o modelo iterar/treinar 5 vezes, você terá um verdadeiro score de como seu modelo está generalizando, geralmente ao tirar a média e desvio padrão de todos os treinos realizados. Esse processo faz com que o treino demore um pouco mais, mas é crucial para ter certeza de que seus dados estão generalizando bem.

#### Teoria Redes Neurais Artificiais

| Titulo | Tipo | Nível | Qualidade | Link | Descrição
|--|--|--|--|--|--|
| Deep-learning book | Curso | Ini - Avançado | 5 | [Link](http://deeplearningbook.com.br/deep-learning-a-tempestade-perfeita/) | Se você tiver tempo, lei todos os capítulos

Neurônio artificial
Funções de ativações
Propagation
Topologias de redes
Rede MLP


#### Deep Learning





Rede Neural Profunda

 - [Teoria - médio - bom para referência em artigos](https://www.nature.com/articles/nature14539)

Rede Neural Convolucional
 - [Teoria - muito bom - bom para aprender](https://towardsdatascience.com/a-comprehensive-guide-to-convolutional-neural-networks-the-eli5-way-3bd2b1164a53)

#### Bibliotecas

Manipulação de dados
 - Pandas 
 - Numpy
 
Visualização:
 - Plotly 
 - Pyplot
 
Machine learning:
 - Sklearn

Deep learning::
 - Tensorflow
 - Pytorch



#### Práticas


#### Extra

 -  [Repositório que reúne vários conteúdos de data science](https://github.com/PizzaDeDados/datascience-pizza)
 - [Repositório que reúne vários conteúdos de machine learning](https://github.com/PizzaDeDados/datascience-pizza/blob/master/topicos/aprendizado-de-maquina.md)
