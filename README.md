# CNN en Español

Este proyecto contiene una demo sobre la implementación de una Red Neuronal Convolucional,
se muestra el proceso desde la recolección de imagenes, pre-procesamiento de la data,
asi como la construcción y entrenamiento de dicha Red Neuronal.

## Tecnologias
- Python
- Jupyter Notebooks
- Tensorflow
- Keras

## Test con docker
Este proyecto puede ser ejecutado utilizando docker con el siguiente comando
```
docker run --name cnn-espanol -p 8888:8888 -v $(pwd):/home/jovyan/work jupyter/tensorflow-notebook
```

## Recolección de Imagenes.
Para recolectar las imagenes se hizo uso de Google Search y de la extension para chrome [Download All Images](https://chrome.google.com/webstore/detail/download-all-images/ifipmflagepipjokmbdecpmjbibjnakm). El plugin descargara TODAS las imagenes cargadas en la pagina.

Se necesitará una inspección manual de las imagenes descargadas para asegurarse de que dichas imagenes esten directamente relacionadas al problema a tratar y sean una representación valida de las categorias a tratar.

### Imagenes utilizada en este ejemplo: 
- https://lmgtfy.com/?q=charmander&t=i
- https://lmgtfy.com/?q=bulbasaur&t=i
- https://lmgtfy.com/?q=squirtle&t=i

## Pre-procesamiento.
Como media para reducir el computo necesario las imagenes seran transformadas a una version de 32x32 pixeles, los nombres y formatos de las imagenes seran estandarizados para facilitar su manipulación.

Nuevos ejemplos serán creados utilizando [ImageDataGenerator](https://www.tensorflow.org/api_docs/python/tf/keras/preprocessing/image/ImageDataGenerator) con la intención de incrementar la cantidad de imagenes y así mejorar el rendimiento de el algoritmo.

## Construcción de CNN.

## Entrenamiento de CNN.

## Verificación de Predicción.