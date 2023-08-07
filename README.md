# Inteligencia Artificial - Universidad Francisco Marroquín

Este repositorio contiene el código para la clase de Inteligencia Artificial de la Facultad de Ciencias Económicas de la Universidad Francisco Marroquín.

## Empezando

Pueden correr estos notebooks en plataformas cloud como [Google Colab](https://colab.research.google.com/) o en su máquina local. Noten que la mayoría de notebooks requieren de un GPU para correr en un lapso de tiempo razonable, así que recomiendo que utilicen una de las plataformas cloud ya que vienen preinstaladas con CUDA.

### Utilizando una plataforma cloud

Actualmente, los GPUs en Colab tienden a ser K80s (los cuales tienen memoria limitada), por lo que recomiendo que utilicen [Kaggle](https://www.kaggle.com/docs/notebooks), [Gradient](https://gradient.run/notebooks) o [SageMaker Studio Lab](https://studiolab.sagemaker.aws/). Estas plataformas tienden a proveer GPUs con mejor desempeño como P100s, sin costo.

> Nota: algunas plataformas cloud como Kaggle requieren que reinicien el notebook después de instalar nuevas librerías.

### Corriendo el código en sus maquinas

Para correr los notebooks localmente, primero clonen el repositorio y naveguen a el:

```bash
$ git clone https://github.com/Francososa/UFM-AI-22.git
$ cd UFM-AI-22
```

Luego, corran el siguiente comando para crear un ambiente virtual de `conda` que contiene todas las librerías necesarias para correr los notebooks:

```bash
$ conda env create -f environment.yml
```

> Nota: Necesitaran un GPU que soporte el [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) de NVIDIA para poder build el entorno.

La clase sobre Question Answering tiene un conjunto de dependencias especiales, para correr el codigo de esa clase necesitan un entorno separado:

```bash
$ conda env create -f environment-qa.yml
```

Una vez hayan instalado las dependencias, pueden activar el entorno `conda` y levantar los notebooks de la siguiente manera:

```bash
$ conda activate ufm-ai # o conda activate ufm-ai-qa
$ jupyter notebook
```
