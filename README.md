# CapsNet-Comparative-Performance
CapsNet performance 

Este repositorio tiene como objetivo medir el desempeño de CapsNet vs Mobilenet V2.0. Se presenta en la carpeta `CNN notebooks` los jupyter notebooks para poder correr los modelos, así como el `trained_model.h5` que contiene los pesos por si se desea solo correr los test sets. `CapsNet`  contiene tres subcarpetas `Cifar10`, `Fashionmnist` y `MNIST` en las cuales se tienen los modelos así como los pesos correspondientes.

Para el casO de `MNIST` al final de los notebook se tienen los comandos necesarios para correr la prueba con una nueva base de datos `affNIST`. El objetivo es medir que tan preparado esta un modelo entrenado por CapsNet vs CNN

## Corriendo los notebooks

Para poder correr los jupyter notebooks es necesario tomar en cuenta las siguientes consideraciones:

	1. Los modelos de CNN fueron entrenado en la versión beta de tensorflow2.0, para poder correrlos,
	se recomienda primero crear un ambiente local como se menciona abajo.

	2. CapsNet fue entrenada con una versión distinta de tensorflow

### Ambiente local
Para instalar el ambiente completo en tu computadora, se sugiere usar [Anaconda](https://www.anaconda.com/) con el archivo `environment_cpu.yml` de la siguiente manera: 

```
conda env create -n cursoap -f environment_cpu.yml
```

Si tu computadora cuenta con GPU NVIDIA y deseas aprovecharlo, instala los controladores y cambia el archivo `environment_cpu.yml` por `environment_gpu.yml`, es decir

```
conda env create -n cursoap -f environment_gpu.yml
```

Puedes cambiar el nombre del ambiente por el que tu prefieras. Finalmente, debes activar el ambiente cuando desees utilizarlo

```
conda activate cursoap 
```
