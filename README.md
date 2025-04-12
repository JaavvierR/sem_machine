# README para el Sistema de ML Multi-Módulo

## Descripción
Este proyecto consiste en un sistema de Machine Learning (ML) multi-módulo que permite a los usuarios seleccionar entre diferentes tareas de ML, que incluyen:

1. **Predicción de Series Temporales (Ventas)**: Generación de un conjunto de datos sintético de ventas diarias y un modelo para predecir ventas basado en diferentes factores.
2. **Clasificación de Imágenes (MNIST)**: Entrenamiento de un modelo de red neuronal convolucional (CNN) para clasificar imágenes del conjunto de datos MNIST.
3. **Análisis de Sentimientos**: Evaluación de reseñas de productos para determinar su sentimiento (positivo o negativo) usando redes neuronales.
4. **Generación de Contenido**: Creación de texto simulado y patrones visuales utilizando modelos generativos.

## Requisitos
Este sistema requiere las siguientes bibliotecas de Python:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `tensorflow`

Puedes instalar todas las bibliotecas necesarias utilizando el siguiente comando:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
```

## Estructura del Código

### 1. Importaciones
El código comienza con las importaciones necesarias para el funcionamiento de cada módulo.

### 2. Elegir Módulo
El usuario puede elegir qué módulo ejecutar mediante una función que despliega el menú de opciones y llama a la función correspondiente.

### 3. Funcionalidades de Cada Módulo
- **Predicción de Series Temporales**:
  - Genera un conjunto de datos sintético de ventas.
  - Entrena un modelo de red neuronal para hacer predicciones basadas en este conjunto de datos.
  - Realiza un análisis de sensibilidad para determinar los factores que impactan las ventas.

- **Clasificación de Imágenes (MNIST)**:
  - Carga el conjunto de datos MNIST, lo normaliza y lo visualiza.
  - Construye y entrena un modelo CNN para clasificar imágenes de dígitos.
  - Muestra y guarda las predicciones junto con la matriz de confusión.

- **Análisis de Sentimientos**:
  - Genera un conjunto de datos de reseñas sintéticas con etiquetas de sentimiento.
  - Prepara y entrena un modelo de análisis de sentimientos para clasificar nuevas reseñas.
  - Visualiza la precisión del modelo a lo largo del tiempo.

- **Generación de Contenido**:
  - Implementa un generador de texto simple basado en un modelo LSTM.
  - Crea imágenes usando patrones matemáticos y las guarda.

### 4. Ejecución Principal
El código principal permite al usuario seleccionar el módulo desde la consola y manejar posibles errores durante el ingreso de la opción.

## Ejecución
Para ejecutar el sistema, simplemente corre el archivo principal de Python:

```bash
python nombre_del_archivo.py
```

Asegúrate de tener todos los requisitos instalados y de estar en un entorno adecuado para la ejecución del programa.

## Archivos Generados
Al finalizar cada módulo, se generan archivos con resultados específicos, tales como:

- `ventas_tienda_diarias.csv` - Dataset de ventas.
- `modelo_ventas_tienda.h5` - Modelo de predicción de ventas entrenado.
- `modelo_mnist.h5` - Modelo CNN para clasificación de imágenes.
- `modelo_sentimientos.h5` - Modelo para análisis de sentimientos.
- `modelo_generador_texto.h5` - Modelo generador de texto.
- Varias imágenes generadas y gráficas para visualizaciones.

## Contribuciones
Las contribuciones son bienvenidas. Si tienes mejoras o sugerencias, no dudes en abrir un issue o enviar un pull request.

## Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.