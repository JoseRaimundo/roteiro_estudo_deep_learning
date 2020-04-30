
### Descrição do repositório


Este repositório funciona como uma base de consulta sobre tópicos relacionados a deep learning. O objetivo deste repositório é catalogar conteúdos e informações importantes sobre deep learning que foram úteis ou interessantes durante minhas experiências.

#### Redes Neurais Artificiais

Com  o aumento dos recursos computacionais e disponibilidade de dados, cada vez mais é possível explorar técnicas de IA, que antes eram inviável devido a alta demanda de recursos mencionados. Redes Neurais Artificias são uma tentativa de imitar o funcionamento do cérebro humano,  no qual várias camadas de neurônios são conectados por meio  de conexões sinápticas que se ajustam a medida que aprendem, possibilitando a abstração de dados de entrada e identificando padrões que são obtidos na saída [[1]](https://github.com/JoseRaimundo/deep_learning_review#refer%C3%AAncias).

#### Configuração da uma Rede Neural

A escolha dos parâmetros para configurar uma rede neural pode variar  de acordo com o problema abordado, logo **não há um valor padrão ou uma regra absoluta**, uma das melhores abordagens é a partir do método empírico (usar sua experiência e ajudar a partir de uma abordagem tentativa-erro). Porém, aqui será apresentado alguns dicas para auxiliar na escolha inicial dos parâmetros.

##### Profundidade e largura

O conceito de profundida e largura diz respeito respectivamente a quantidade de camadas e de neurônios por camada. 

##### Épocas do treinamento

A quantidade de épocas diz respeito a quantidades que vezes que o conjunto de dados é apresentado a rede [[2]](https://github.com/JoseRaimundo/deep_learning_review#refer%C3%AAncias). 

 - Limite estático: Comece a quantidade de épocas com um valor estático,  um valor pequeno inicialmente como 100 pode ajudar na etapa de testes de desenvolvimento (quando você só quer ver se o código está funcionando). Porém, para ver o funcionamento real da rede, use valores entre **1000** e **10000**. 
 - Limiar de erro: Utilize a taxa de erro médio quadrático para definir a parada do seu treino, a cada época (época agora assume um valor muito grande ou infinito), avalie a taxa de erro, defina uma limiar para caso seja atingida, use limiar como **0.01** para acionar a parada do loop de treino. É importante lembrar que um erro médio quadrático muito pequeno não implica necessariamente numa boa generalização.
 - Combinação dos Mé todos Anteriores.




### Referências


[1] [Deep learning](https://www.nature.com/articles/nature14539)

[2] [DICAS PARA A CONFIGURAÇ ÃO DE REDES NEURAIS](http://www.nce.ufrj.br/labic/downloads/dicas_cfg_rna.pdf)

[3] [A Comprehensive Guide to Convolutional Neural Networks — the ELI5 way](https://towardsdatascience.com/a-comprehensive-guide-to-convolutional-neural-networks-the-eli5-way-3bd2b1164a53)