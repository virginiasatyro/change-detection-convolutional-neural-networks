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