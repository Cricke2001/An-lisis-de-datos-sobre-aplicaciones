# Proyecto de Análisis de Datos con Pandas y Visualización con Matplotlib y Seaborn

URL CSV: https://drive.google.com/file/d/1XX1NKxgOQr4P_92e1YVHeqbvzMpyt6dq/view?usp=sharing

## Descripción

Este proyecto tiene como objetivo realizar un análisis exploratorio de datos (EDA) utilizando Python y varias bibliotecas populares, como Pandas, Matplotlib y Seaborn para obtener información relavente para elaborar una campaña de publicidad en aplicaciones efectiva y personalizada para el público objetivo. Se utiliza Jupyter Notebook como entorno de desarrollo para facilitar la visualización y el análisis interactivo de los datos. El conjunto de datos proviene de una base de datos publicada en Kaggle basada en la Play Store, con más de 400.000 aplicaciones.

## Tecnologías Utilizadas

- **Python**: Lenguaje de programación principal.
- **Pandas**: Biblioteca para la manipulación y análisis de datos.
- **Matplotlib**: Biblioteca para crear visualizaciones estáticas en Python.
- **Seaborn**: Biblioteca para visualización de datos que se basa en Matplotlib y proporciona una interfaz más amigable y atractiva.
- **Jupyter Notebook**: Entorno de desarrollo interactivo que permite la ejecución de código en Python, la visualización de gráficos y la creación de documentos de texto.

## Instalación

1. **Clonar el repositorio**:
   ```bash
   git clone https://github.com/tu_usuario/nombre_del_repositorio.git
   cd nombre_del_repositorio
   ```

2. **Instalar las dependencias**:
   Asegúrate de tener Python y pip instalados. Luego, ejecuta:
   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```

## Uso

1. **Abrir Jupyter Notebook**:
   En la terminal, dentro del directorio del proyecto, ejecuta:
   ```bash
   jupyter notebook
   ```
   Esto abrirá el navegador con la interfaz de Jupyter.

2. **Ejecutar el Notebook**:
   Abre el archivo `analisis_datos.ipynb` y sigue las celdas para ver el análisis paso a paso.

## Contenido del Proyecto

- **`data/`**: Carpeta que contiene los archivos de datos utilizados en el análisis.
- **`analisis_datos.ipynb`**: Notebook de Jupyter que contiene todo el análisis, visualizaciones y comentarios sobre el conjunto de datos.
- **`visualizaciones/`**: Carpeta con gráficos generados durante el análisis, almacenados como imágenes.

## Ejemplo de Análisis

En el Notebook se realizan los siguientes pasos:

1. **Carga de Datos**:
   Se cargan los datos utilizando Pandas, y se realizan inspecciones iniciales para entender la estructura del conjunto de datos.
   ```python
   import pandas as pd
   df = pd.read_csv('data/dataset.csv')
   print(df.head())
   ```

2. **Limpieza de Datos**:
   Se identifican y manejan valores nulos, tipos de datos y se eliminan duplicados.
   ```python
   df.dropna(inplace=True)
   df = df.drop_duplicates()
   ```

3. **Análisis Exploratorio**:
   Se generan estadísticas descriptivas y se visualizan relaciones entre variables utilizando Seaborn y Matplotlib.
   ```python
   import seaborn as sns
   import matplotlib.pyplot as plt
   
   sns.pairplot(df)
   plt.show()
   ```

4. **Visualización**:
   Se crean gráficos para ilustrar los hallazgos clave del análisis, como histogramas, diagramas de dispersión y gráficos de barras.
   ```python
   plt.figure(figsize=(10, 6))
   sns.barplot(x='categoria', y='ventas', data=df)
   plt.title('Ventas por Categoría')
   plt.show()
   ```

## Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar este proyecto, por favor sigue estos pasos:

1. Haz un fork del proyecto.
2. Crea una nueva rama (`git checkout -b feature/mi-contribucion`).
3. Realiza tus cambios y haz commit (`git commit -m 'Añadir nueva funcionalidad'`).
4. Envía un pull request.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

## Autor

[Carlos Ricke] - [carlosricke.p@protonmail.com] - [@Cricke2001]

---

¡Gracias por tu interés en este proyecto! Espero que encuentres útil este análisis y las visualizaciones generadas.
```
