# Projeto Pinniped Species Identification

# Este projeto envolveu o uso de uma Rede Neural Convolucional (RNC) Profunda para criar um aplicativo capaz de classificar imagens de 3 espécies de lobos-marinho com registros para o litoral brasileiro.
# São elas: lobo-marinho-sul-americano (Arctocephalus australis), lobo-marinho-subantártico (A. tropicalis) e lobo-marinho-antártico (A. gazella).
# O modelo RNC foi construído usando 121 imagens das 3 espécies. As imagens foram randomizadas e divididas em média a 70% para treinamento (26 imagens de A. australis 30 de A. tropicalis e 29 de A. gazella) e 30% para teste (12 imagens de cada espécie).Foram utilizados os pesos do modelo VGG16 (Simonyan e Zisserman 2014).
# Após concluído o treinamento, o modelo foi submetido as imagens de teste selecionadas. O modelo atribuiu corretamente 30 das 36 imagens, classificando-as de forma correta de acordo com a espécie previamente informada. Desta forma, a acurácia do modelo foi de 0.8334, ou seja, 83.34% de acerto na classificação das imagens de teste. 
# Das 12 imagens de A. australis (rótulo 0) o modelo atribuiu corretamente 10 e as outras duas ele atribuiu erroneamente, classificou-as como A. gazella.
# Das 12 imagens de A. tropicalis (rótulo 1) o modelo também atribuiu corretamente 10,  enquanto as demais foram classificadas uma como A. australis e outra como A. gazella. 
# Das 12 imagens de A. gazella (rótulo 2) o modelo acertou novamente 10, classificando uma de forma errônea como A. australis e outra como A. tropicalis. 
# O modelo treinado esta sendo implantado em um aplicativo interativo para permitir que os usuários possam compartilhar suas imagens e assim, identificar suas próprias fotos de pinípedes.
# O objetivo final deste projeto é treinar o modelo para classificar corretamente todas as 8 espécies do gênero Arctocephalus (lobos-marinho).
