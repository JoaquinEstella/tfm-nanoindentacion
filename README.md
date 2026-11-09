# Detección automática de anomalías en curvas de ensayos de nanoindentación mediante aprendizaje automático

Cuaderno de análisis del Trabajo Fin de Máster del Máster Universitario en Big Data y Ciencia de Datos (Universidad Internacional de Valencia), de Ricardo Joaquín Estella Vilche, 2026.

El trabajo estudia si un modelo de aprendizaje automático puede reproducir la limpieza que hace un especialista de los ensayos de nanoindentación, y si la forma de la curva fuerza-profundidad aporta información que no está en los valores que calcula el laboratorio.

## Contenido

- `TFM_cuaderno_de_analisis.ipynb`: el cuaderno completo, con sus salidas. Contiene todo el análisis de la memoria, de la comprobación del conjunto de datos a las ilustraciones (celdas 0 a 19).
- `figuras/`: las 17 ilustraciones de la memoria, tal como las guarda la celda 18.

## Datos

Los datos no se incluyen en este repositorio. Son públicos:

Henriksen, A., Zakariya, P., Babuska, T., y Mundt, M. (2025). *A ground truth dataset for anomaly detection on load-displacement nanoindentation curves for NiFe electroplated samples* [Conjunto de datos]. Materials Data Facility. https://doi.org/10.18126/yvgn-w386. Licencia CC BY 4.0.

La descarga se hace desde el Materials Data Facility mediante Globus, con una cuenta gratuita. El fichero comprimido `anomaly_detection_on_nanoindentation.zip` se sube a `/content` antes de ejecutar; la celda 1 lo descomprime en `/content/nanoindent`.

## Cómo ejecutarlo

1. Abrir el cuaderno en Google Colaboratory y subir el fichero de datos a `/content`.
2. Ejecutar la celda 0 y comprobar las versiones. Si alguna no coincide con las de la tabla de abajo, la celda imprime la orden de instalación; después de instalar hay que reiniciar la sesión.
3. Ejecutar todas las celdas en orden y en la misma sesión. La ejecución completa tarda unos minutos.
4. La celda 19 comprime la carpeta de figuras y la descarga (solo en Colab).

Para ejecutarlo fuera de Colab basta con sustituir `/content` por otra carpeta en todo el cuaderno. Los procesos aleatorios usan semillas fijas; con las mismas versiones, la ejecución reproduce las cifras de la memoria.

## Versiones

| Python | NumPy | pandas | SciPy | scikit-learn | Matplotlib | SHAP |
|---|---|---|---|---|---|---|
| 3.13.16 | 2.1.3 | 2.2.3 | 1.16.3 | 1.6.1 | 3.10.0 | 0.52.0 |

Las salidas que acompañan al cuaderno proceden de una ejecución completa con estas versiones.
