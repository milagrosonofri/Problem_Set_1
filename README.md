# Problem Set 1 - Machine Learning

Este repositorio contiene los materiales, scripts y resultados del Problem Set 1 de Machine Learning en la Maestría en Economía de la UNLP. El proyecto abarca web scraping, limpieza de datos, análisis exploratorio, modelado predictivo y presentación de resultados. A continuación, se detalla la estructura del repositorio y el flujo de trabajo.

## Estructura del repositorio

```plaintext
Problem_Set_1/
├── document/
│   └── report.pdf         # PDF con la metodología, análisis y resultados
├── scripts/
│   └── PS1.ipynb          # Script con el código para scraping, análisis y modelado
├── stores/
│   └── dataframe.csv      # Conjunto de datos crudos obtenidos del web scraping
├── views/
│   └── *.png              # Gráficos con estadísticas descriptivas, resultados de modelos y errores de predicción
├── README.md
└── requirements.txt
```

## 1. document
Contiene un archivo PDF (report.pdf) que documenta todo el proceso, incluyendo los objetivos, la metodología y los resultados clave.
Consulta este archivo para obtener un resumen completo del proyecto sin necesidad de ejecutar el código.

## 2. scripts
PS1.ipynb: Un notebook de Jupyter que incluye:
- Scraping de datos desde múltiples páginas web utilizando las librerías requests y BeautifulSoup.
- Limpieza y filtrado de datos: Restricción a individuos empleados mayores de 18 años y preparación de variable de interés.
- Análisis exploratorio de datos con estadísticas descriptivas y distribuciones de variables.
- Construcción y evaluación de modelos predictivos, como regresión lineal y polinómica, para predecir el salario horario de los asalariados en Colombia. 
- Comparación de los RSME asociados a cada modelo.
- Generación de gráficos para analizar los errores de predicción de los modelos con menor RSME.
- Leave-One-Out-Cross-Validation (LOOCV) para evaluar la capacidad predictiva de los modelos con mejor RMSE.

## 3. stores
Contiene el conjunto de datos (dataframe.csv), generado tras el scraping.

## 4. views
Almacena visualizaciones generadas durante el análisis, que incluyen:
- Histogramas de las variables clave.
- Scatterplots y matriz de correlación para analizar la relación entre las variables independientes y la dependiente.
- Errores de predicción para diferentes modelos.

## Cómo usar este repositorio
### Instalar Dependencias

Este proyecto utiliza Python y varias bibliotecas. Instala las dependencias necesarias con:

```plaintext
pip install -r requirements.txt
```

### Ejecutar el script

- Abre el archivo PS1.ipynb en Jupyter Notebook, Jupyter Lab o Google Colab.
-  Ejecuta las celdas en orden para reproducir los resultados:
- Realizar el scraping y limpieza de datos.
- Generar estadísticas descriptivas y visualizaciones.
- Entrenar modelos predictivos y evaluar su desempeño.

### Explorar los resultados

- Revisa las visualizaciones en la carpeta views/ para obtener información clave.
- Consulta el archivo report.pdf en la carpeta document/ para un resumen detallado.

### Características principales
Web Scraping: Obtención de datos desde una fuente pública usando Python.
Limpieza de Datos: Filtrado y preprocesamiento de datos para su análisis.
Modelado Predictivo: Incluye regresión simple y polinómica para predecir ingresos.
Visualización: Gráficos informativos para apoyar la interpretación de los datos.

### Requisitos
- Python 3.8 o superior
- Bibliotecas principales:
requests, BeautifulSoup, pandas, numpy
seaborn, matplotlib, scikit-learn
