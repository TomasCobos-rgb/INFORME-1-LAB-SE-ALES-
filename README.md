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
