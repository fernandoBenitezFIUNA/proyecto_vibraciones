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
| Random Forest | 84.7% |
| SVM | 45.6% |

*Nota: Se actualizó el Accuracy CV de Random Forest en base al promedio de las iteraciones detalladas a continuación.*

### Detalle de Validación Cruzada (Random Forest)

Para proporcionar más detalle sobre el desempeño del modelo final (Random Forest), a continuación se presentan los resultados individuales por *fold* y las matrices de confusión correspondientes:

**Tabla de Accuracy por Iteración:**

| Fold | Accuracy |
|------|----------|
| 1    | 0.928571 |
| 2    | 0.821429 |
| 3    | 0.857143 |
| 4    | 0.888889 |
| 5    | 0.740741 |

**Resumen de Cross Validation:**
- **Accuracy promedio:** 0.8474
- **Accuracy máximo:** 0.9286
- **Accuracy mínimo:** 0.7407
- **Desviación estándar:** 0.0640

---

**Matrices de Confusión Detalladas por Fold:**

A continuación se presentan las matrices de confusión generadas para cada una de las iteraciones de la validación cruzada. Note que estas matrices detalladas muestran el desempeño individual en diferentes subconjuntos de datos.

**Iteración 1 (cv_fold1):**
![Matrix Fold 1](images/cv_fold1.png)

**Iteración 2 (cv_fold2):**
![Matrix Fold 2](images/cv_fold2.png)

**Iteración 3 (cv_fold3):**
![Matrix Fold 3](images/cv_fold3.png)

**Iteración 4 (cv_fold4):**
![Matrix Fold 4](images/cv_fold4.png)

**Iteración 5 (cv_fold5):**
![Matrix Fold 5](images/cv_fold5.png)

---

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
