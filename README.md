# Detector de Tumor Cerebral
## Projeto  
Este projeto utiliza uma rede convolucional do Google (MobileNetV2) com 2.5 Milhões de parametros já treinados pelo google. Esta rede convolucional foi conectada à uma rede neural com um neorônio de saida que dirá a probabilidade da imagem ter um tumor ou não. Tal tecnica é conhecida como transfer learning, por analogia podemos pensar no transfer learning como treinar uma parte do cérebro para aprender uma tarefe nova, por exemplo usar a parte do cérebro responsável pelo paladar para detectar imagens por meio de impulsos nervosos.

## Base de Dados e Processamento de Imagens
Os dados usados para re-treinar a rede neural foram obtidos de um dataset do [Kaggle](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection) onde foi utilizado 155 tumografias sem tumores e 98 tumografias com tumores. Para almentar o conjuto de treino foi ultilizado o método conhecido como data augmentation que é fazer novas imagens a partir de rotações e ampliações nas imagens originais, tal método torna a rede neural mais robusta para detectar tumores.

![](https://media.springernature.com/lw685/springer-static/image/art%3A10.1007%2Fs40998-021-00426-9/MediaObjects/40998_2021_426_Fig10_HTML.png)

## Resultados
A precisão alcançada foi de 89% para o conjunto de teste, o que não é algo baixo uma vez que o conjunto de traino é razoavelmente pequeno. **dessa forma para tornar-mos esse modelo mais preciso e robusto devemos obter mais imagens de tumografias, de preferencia imagens provenientes de fontes diversas pois isso torna o modelo mais robusto à outliers** 
