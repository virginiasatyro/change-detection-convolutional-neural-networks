# Redes Neurais Convolucionais para Detecção de Mudança em Imagens de Satélite

```
├── main.ipynb
├── dataset-utl.ipynb
```

- main.ipynb: script printipal;
- dataset-utl.ipynb: script relacionado ao dataset;

## TO-DO 

- entendimento do dataset;
- tratamento do dataset;
  - augmentação das imagens;
- treinamento da rede

## Dataset

### [Onera Satellite Change Detection Dataset](https://rcdaudt.github.io/oscd/)

Esse *dataset* tem como objetivo ser útil no problema da detecção de mudanças entre imagens de satélite de diferentes datas.

No total são 24 pares de imagens **multiespectrais** do setélite **Sentinel-2** obtidas entre 2015 e 2018. As imagens são de locais variados como o Brasil, Europa, Estados Unidos, Ásia, etc. Para cada local, existe um par de imagens de satélite de 13 bandas multiespectral obtidos pelo satélite **Sentinel-2**. AS imagens tem resoluções variadas - 10m, 20m e 60m.

**Pixel-level change ground truth** - fornecido para 14 pares de treinamento e 10 pares de treinamento.

As mudanças nesse dataset são focadas em novas **construções** e **estradas**. Pode ser utilizado para treinamento e definição de parametros para algoritmos de CD.

## Por que *Change Detection (CD)*?

CD é um dos maiores problemas associados a àrea de análise e observação da Terra por imagens de satélite. O sistema de CD consiste em assinalar um rótulo binário por pixel baseado em um par de imagens de determinada região em diferentes tempos. O rótulo positivo indica que a àrea correspondente ao pixel foi alterada.

A definição de "mudança" varia de aplicação para aplicação, mas pode se referir a, por exemplo, mudança na vegetação, expansão urbana, derretimento polar, etc. CD é uma ferramenta poderosa na produção de mapas e análise da evolução do uso da terra, cobertura urbana, desmatamento, e outros tipos de análises multi-temporais.

Utilizar CD pode ser uma ferramenta muito útil no estudo e detecção de áreas de desmatamento. As mudanças nas áreas podem ser semânticas (do objeto em análise) ou ruidosas (variações na luminosidade, sombras, entre outras). O desafio no CD é minimizar essas variações ruidosas e enfatizar as mudanças semânticas. Geralmente, o mapa final fornece uma classificação binaria da região modificada.

## Por que *Deep learning*?

Métodos "clássicos" x *Machine Learning (ML)* x *Deep Learning (DL)*
