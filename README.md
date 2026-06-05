# Clasificación de Condiciones de Desbalance mediante Machine Learning

Proyecto desarrollado en la Facultad de Ingeniería de la Universidad Nacional de Asunción (FIUNA).

Se utilizaron señales de vibración obtenidas de un sistema rotativo para clasificar condiciones de desbalance mediante técnicas de Machine Learning.

![Portada](images/confusion_matrix.png)

## Objetivos
- Adquirir señales de vibración.
- Extraer características estadísticas y espectrales.
- Entrenar modelos de clasificación.
- Comparar desempeño entre algoritmos.

## Dataset

Condiciones evaluadas:

- Normal
- Unbalance 19 g
- Unbalance 23 g
- Unbalance 27 g

## Características extraídas

- RMS
- Peak
- Crest Factor
- Kurtosis
- Desviación estándar
- Frecuencia dominante
- Energía espectral
- Centroide espectral
- Bandwidth espectral

## Tecnologías utilizadas

- Python
- Pandas
- NumPy
- SciPy
- Scikit-Learn
- Matplotlib
- Jupyter Notebook

## Metodología

1. Adquisición de señales de vibración.
2. Segmentación de señales.
3. Extracción de características estadísticas y espectrales.
4. Construcción del dataset.
5. Entrenamiento de modelos de Machine Learning.
6. Evaluación mediante validación cruzada y conjunto de prueba.
   
## Modelos evaluados

- Random Forest
- SVM

## Resultados

| Modelo | Accuracy CV |
|----------|------------|
| Random Forest | 76.8% |
| SVM | 45.6% |

El modelo Random Forest fue seleccionado como modelo final.

Accuracy obtenido en el conjunto de prueba:

**93%**

## Visualizaciones

![FFT](images/FFT.png)

![Confusion Matrix](images/confusion_matrix.png)

## Autores

- Fernando Benitez
- Manuel Arrom

FIUNA - 2026
