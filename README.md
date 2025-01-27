# CapsNet-Comparative-Performance
CapsNet performance 

Este repositorio tiene como objetivo medir el desempeño de CapsNet vs Mobilenet V2.0. Se presenta en la carpeta `CNN notebooks` los jupyter notebooks para poder correr los modelos, así como el `trained_model.h5` que contiene los pesos por si se desea solo correr los test sets. `CapsNet`  contiene tres subcarpetas `Cifar10`, `Fashionmnist` y `MNIST` en las cuales se tienen los modelos así como los pesos correspondientes.

Para el caso de `MNIST` al final de los notebook se tienen los comandos necesarios para correr la prueba con una nueva base de datos `affNIST`. Aquí el objetivo es medir que tan preparado esta un modelo entrenado por CapsNet vs CNN

## Corriendo los notebooks

Para poder correr los jupyter notebooks es necesario tomar en cuenta las siguientes consideraciones:

	1. Los modelos de CNN fueron entrenados en la versión beta de tensorflow2.0, para poder correrlos,
	se recomienda primero crear un ambiente local como se menciona abajo.

	2. CapsNet fue entrenada con una versión distinta de tensorflow y por tanto se proporciona 
	un archivo distinto para poder crear el ambiente virtual.

### Ambiente local [Ref](https://github.com/gibranfp/CursoAprendizajeProfundo)
Para instalar el ambiente completo en tu computadora, se sugiere usar [Anaconda](https://www.anaconda.com/) con el archivo `archivo.yml` de la siguiente manera: 

```
conda  create -n  archivo.yml
```

Finalmente, debes activar el ambiente cuando desees utilizarlo con el siguiente comando:

```
conda activate nombre_ambiente
```

Elije de la siguiente lista de arvhivos.yml el que corresponda a tu computadora.

* `capsnet_cpu.yml` para correr los jupyter-notebook de `capsnet` usando cpu 
* `capsnet_gpu.yml` para correr los jupyter-notebook de `capsnet` usando gpu
* `environment_cpu.yml` para correr los jupyter-notebook de `CNN` usando cpu 
* `environment_gpu.yml` para correr los jupyter-notebook de `CNN` usando gpu 


## Resultado

En el archivo `CapsNet-Comparative-Performance.pdf` se encuentran los resultados comparativos de los modelos, así como algunas observaciones de interés y referencias utilizadas.
