# Proyecto: Análisis Exploratorio de Clientes y Uso de Servicios de Telecomunicaciones en ConnectaTel

## 📌 Objetivo del Proyecto

El objetivo de este proyecto es identificar patrones de uso, detectar comportamientos atípicos y comprender qué segmentos de clientes muestran necesidades diferenciadas, con el fin de optimizar la oferta comercial y mejorar la experiencia del usuario.

---

## 📂 Datasets Utilizados

El proyecto utiliza tres fuentes de datos principales:

### plans.csv: los planes actuales (precio, minutos incluidos, GB incluidos, costo por extra).

### users_latam.csv: información de clientes: edad, ciudad, fecha de registro, plan contratado.

### usage.csv: el detalle de uso real: llamadas (duración) y mensajes (longitud).

---


## 🔍 Etapas del Análisis

El proyecto siguió un flujo estructurado de análisis exploratorio de datos (EDA), orientado a garantizar la calidad de la información y generar insights accionables para el negocio.

| Paso                                            | Acción                                                                                                    | Resultado para el negocio                                                                         |
| ----------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| **1. Carga y exploración de datos**             | Carga y exploración inicial de los datasets `plans`, `users_latam` y `usage`.                             | Comprensión de la estructura, tipos de datos y contenido de cada fuente de información.           |
| **2. Identificación de problemas de calidad**   | Detección de valores nulos, sentinels, inconsistencias y fechas fuera de rango.                           | Identificación de problemas que podrían afectar la calidad del análisis y la toma de decisiones.  |
| **3. Limpieza y preparación de datos**          | Conversión de fechas, tratamiento de sentinels y manejo de valores ausentes según su contexto de negocio. | Obtención de datos consistentes y preparados para el análisis estadístico.                        |
| **4. Estadística descriptiva**                  | Análisis de variables numéricas y categóricas mediante medidas descriptivas y frecuencias.                | Comprensión del comportamiento típico de los usuarios y detección de valores extremos.            |
| **5. Visualización y detección de outliers**    | Construcción de histogramas y boxplots para analizar distribuciones y valores atípicos.                   | Identificación de patrones de uso, sesgos en las distribuciones y posibles anomalías.             |
| **6. Segmentación de clientes**                 | Creación de grupos de edad y niveles de uso, complementados con visualizaciones mediante countplots.      | Generación de segmentos accionables para diseñar ofertas, campañas y estrategias de fidelización. |
| **7. Generación de insights y recomendaciones** | Elaboración de conclusiones ejecutivas y propuestas de mejora basadas en los hallazgos obtenidos.         | Traducción de los resultados analíticos en recomendaciones concretas para el negocio.             |

### 🔄 Flujo de trabajo

1. Cargar y explorar los datasets.
2. Detectar problemas de calidad de datos.
3. Limpiar y preparar la información.
4. Analizar estadísticas descriptivas.
5. Visualizar distribuciones y evaluar outliers.
6. Crear segmentos de clientes.
7. Elaborar conclusiones y recomendaciones de negocio.


---

## ▶️ Cómo Ejecutar el Proyecto

### Opción 1: Google Colab

1. Descargar el notebook `.ipynb`.
2. Ingresar a Google Colab.
3. Seleccionar **Archivo → Subir notebook**.
4. Cargar el archivo del proyecto.
5. Ejecutar las celdas en orden.

### Opción 2: Jupyter Notebook

1. Instalar Jupyter Notebook.
2. Abrir una terminal en la carpeta del proyecto.
3. Ejecutar:

```bash
jupyter notebook
```

4. Abrir el archivo `.ipynb`.
5. Ejecutar las celdas secuencialmente.

---

## 🔄 Guía de Reproducción

Para reproducir el análisis:

1. Cargar los datasets originales.
2. Ejecutar las etapas de limpieza de datos.
3. Verificar la calidad de las variables y valores faltantes.
4. Generar las variables derivadas:

   * grupo_edad
   * grupo_uso
5. Ejecutar las visualizaciones y análisis exploratorios.
6. Revisar las conclusiones y recomendaciones finales.

---

## 🛠️ Librerías Utilizadas

* pandas
* numpy
* matplotlib
* seaborn

---

## 📈 Principales Hallazgos

* La mayoría de los clientes pertenece al segmento de Uso Medio.
* Los adultos representan el grupo etario predominante.
* Los valores nulos en duration y length son estructurales y dependen del tipo de comunicación.
* Se identificaron outliers estadísticos en variables de uso, pero fueron conservados por representar comportamientos plausibles de negocio.
* Existen oportunidades para diseñar planes específicos para usuarios de bajo y alto consumo.
