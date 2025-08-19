### INFORME DE LABORATORIO #1.
ANÁLISIS ESTADISTICO DE LA SEÑAL
---------------
##### Este repositorio contiene el desarrollo del laboratorio de análisis de señales fisiológicas, incluyendo la importación, generación, análisis estadístico.
### OBJETIVOS
1. Seleccionar e importar una señal fisiologica desde physionet
2. Generar una señal fisiologica (ECG) por medio del uso del generador de señales, capturarla e importarla en python.
3.  Calcular estadísticos descriptivos con dos métodos (manual y funciones de Python).
4. Analizar estadísticamente la señal propia y compararla con la importada
### PARTE A
En la primera parte se trabaja con una señal fisiológica obtenida de bases de datos como Physionet. La señal se importó en Python y graficó usando librerías como matplotlib. Posteriormente, se calculan estadísticos descriptivos de dos maneras: (1) programando las fórmulas desde cero y (2) empleando funciones predefinidas de Python.
Los estadísticos a calcular son: media, desviación estándar, varianza, coeficiente de variación, histogramas, función de probabilidad y curtosis.

### PROCEDIMIENTO
Para el desarrollo de esta parte se utilizó la señal fisiológica proveniente de la base de datos de **Physionet**. La señal se descargó en formato (.hat) y (.hea), se importó a python por medio de la libreria **wfdb**. Ademas para la visualización de la señal se utilizó la libreria **matplotlib** con el alias **plt**. Esta libreria permitió crear el gráfico con ayuda de sus funciones:
1. plt.plot() : Encargada de **dibujar**la señal.
2. plt.xlabel() y plt.ylabel() : Colocan etiquetas en los ejes.
3. plt.axis() :Ajusta los límites de los ejes.
4. plt.grid() :Encargada de activar la cuadrícula para el gráfico.
### CÓDIGO
![LIBRERIA WFDB](https://github.com/TomasCobos-rgb/INFORME-1-LAB-SE-ALES-/blob/main/CARPETA%20IMAGENES/LIBRERIA%20DE%20WFDB%20EXTRACCION%20SE%C3%91AL%20.png?raw=true)

*USO DE LIBRERIA WFDB Y PLT: CÓdigo para generar gráfica*
### GRÁFICA SEÑAL ECG
![ECG](https://github.com/TomasCobos-rgb/INFORME-1-LAB-SE-ALES-/blob/main/CARPETA%20IMAGENES/IMAGEN%20ELECTRO%20FISIONET.png?raw=true)

*SEÑAL ECG: Señal extraida desde Physionet*

Luego de esto se desarrolló el calculo de los **estadísticos descriptivos** de dos formas:
1. Manualmente.
2. Usando funciones predefinidas de librerias.
   
[Ver cálculos descriptivos](https://github.com/TomasCobos-rgb/INFORME-1-LAB-SE-ALES-/blob/3141668ded5c4e1716253ba7c0ca370a28697c74/CARPETA%20PUNTO%20A/%20estad%C3%ADsticos%20descriptivos/.md)

### PARTE B
En esta sección se trabajará con una señal fisiológica generada a través de un generador de señales biológicas. La señal fue adquirida mediante un DAQ (Data Acquisition System) y almacenada en formato .csv. Posteriormente, se importará el archivo en Python para su procesamiento, lo que incluye la visualización de la señal y el cálculo de sus estadísticos descriptivos (media, varianza, desviación estándar, entre otros). Finalmente, los resultados serán comparados con los obtenidos en la Parte A, con el fin de analizar las similitudes y diferencias entre ambas etapas del estudio.

### PROCEDIMIENTO 
Para el desarrollo de esta parte se utilizó una señal *(ecg)* generada en el generador de señales fisiologicas, con el uso de python se pudó analizar e interpretar la señal adquiridad por medio del *DAQ* y almacenada en un archivo *.csv*.
1. Lectura del archivo. Se usa pandas para abrir el .csv, *sep* permite delimitar o separar por medio de la *","*, se nombran las columnas con *time* y *amplitude* y por último se omite la primera fila con *skiprows=1*
2. Visualización de la señal. Con *Matplotlib* se gráfica la amplitud en funcion del tiempo y se añaden título y etiquetas para cada eje.
### CÓDIGO

![CODIGO PARA LECTURA ARCHIVO .CSV](https://github.com/TomasCobos-rgb/INFORME-1-LAB-SE-ALES-/blob/main/CARPETA%20IMAGENES/CODIGO%20ECG%20DAQ.png?raw=true)

### GRÁFICA SEÑAL ECG DAQ

![SEÑAL ECG DAQ](https://github.com/TomasCobos-rgb/INFORME-1-LAB-SE-ALES-/blob/main/CARPETA%20IMAGENES/SE%C3%91AL%20ECG%20DAQ.png?raw=true)

Luego de esto se desarolló el cálculo de los **estadísticos descriptivos**:
[Ver cálculos descriptivos Parte B](https://github.com/TomasCobos-rgb/INFORME-1-LAB-SE-ALES-/blob/495b2cebcea90640615d2b3002b7b9e79da3f7d4/CARPETA%20PUNTO%20B/C%C3%81LCULOS%20DESCRIPTIVOS/.md)
