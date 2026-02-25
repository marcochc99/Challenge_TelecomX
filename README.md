# Challenge TelecomX

## 1. Generalidades
Este proyecto está orientado al análisis de datos de los clientes de TelecomX con el objetivo de identificar los factores que fomentan la fuga de clientes (churn). El informe final expondrá los factores que más influyen en las decisiones de los clientes en riesgo y ofrecer recomendaciones estratégicas para mejorar su experiencia.

## 2. Librerías Utilizadas
* `pandas`: Manipulación y análisis de datos.
* `numpy`: Soporte para arrays y operaciones numéricas.
* `matplotlib.pyplot` y `seaborn`: Creación de visualizaciones para el análisis exploratorio.

## 3. Metodología
### 3.1. Extracción de Datos
* Los datos se cargaron directamente desde un archivo JSON alojado en un repositorio de GitHub.

### 3.2. Transfornmación de Datos
* **Aplanamiento de la estructura:** Se normalizó la estructura anidada del archivo JSON para crear un DataFrame plano y tabular.
* **Limpieza y transformación:** Se revisó la integridad de los datos para asegurar que no hubiera valores nulos ni duplicados.
* **Ajuste de tipos de datos:** Se corrigieron los tipos de datos en columnas numéricas y se transformaron variables categóricas (como `Partner` y `InternetService`) en un formato binario (1 y 0) para su posterior análisis.

## 4. Análisis
El análisis exploratorio reveló insights cruciales sobre el comportamiento de los clientes:
* **Tasa de Churn General:** TelecomX enfrenta una tasa de churn del **26.5%**.
* **Perfil de Mayor Riesgo:** La combinación de clientes con un **contrato de mes a mes** y servicio de **Fibra Óptica** representa el segmento más propenso a la cancelación.
* **Antigüedad y Costo:**
    * Los clientes que cancelan tienen una antigüedad significativamente menor, con una mediana de **10 meses**, en comparación con la mediana de **40 meses** de los clientes leales.
    * Además, los clientes que abandonan el servicio suelen tener **cargos mensuales más altos**.

## 5. Conclusiones
El churn está fuertemente influenciado por clientes nuevos con planes flexibles y servicios de alto costo, lo que sugiere una posible falta de percepción de valor.

## 6. Recomendaciones
1.  **Focalizar la Retención:** Crear ofertas especiales o descuentos dirigidos a los clientes del segmento de "Fibra Óptica + Contrato Mensual" para incentivarlos a migrar a planes de mayor duración.
2.  **Evaluar la Oferta de Fibra Óptica:** Realizar una revisión de la estructura de precios y la calidad del servicio de fibra para asegurar su competitividad y que cumpla con las expectativas de los clientes que pagan más.
