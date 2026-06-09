# Proyecto EDA Python

🧩 Proyecto EDA con Python

Análisis exploratorio de datos utilizando Python a partir de dos ficheros proporcionados:

    - customer-details.xlsx (3 hojas: 2012, 2013, 2014)

    - bank-additional.csv (campañas de marketing)

El objetivo es unir, limpiar y analizar ambos datasets para extraer conclusiones relevantes.


📥 Datos y preparación

    Carga de las tres hojas del Excel y unión en un único DataFrame.

    Carga del CSV y verificación de coincidencia de registros (>99%).

    Unión final por índice en un solo df.


🧹 Limpieza aplicada

    Eliminación de columnas residuales.

    Renombrado de columnas a español.

    Conversión de tipos.

    Relleno de nulos en variables categóricas y numéricas.

    Detección de columnas poco fiables (ingresos, num_hijos).

Análisis descriptivo:

🔹 Distribución de edades

    Edad media: 40 años

    Rango: 17–98

    Se detecta un pico anómalo en los 38 años → dato sintético generado en la transformación.

🔹 Ocupación

    11 categorías.

    Se tradujeron al español.


🔹 Estado civil

    Mayoría casados

    Solteros y divorciados en menor proporción

🔹 Hijos

    Proporciones irreales entre categorías

    Se descarta como variable fiable

🔹 Vía de contacto

    65% móvil

    35% teléfono fijo

    Duración media de llamadas similar entre ambos canales


📊 Principales hallazgos

    Edad media: ~40 años, con un pico anómalo en 38.

    Datos de ingresos con distribuciones poco naturales (datos sintéticos).

    11.3% de éxito en la campaña.

    El cliente que acepta la campaña suele tener 28–36 años, préstamos activos y llamadas más largas.

    La vía de contacto (móvil/fijo) no influye significativamente.


📤 Exportación final

    Se genera clientes_OK.csv con los clientes que aceptaron la campaña y sin la edad anómala de 38.


▶️ Ejecución

   1.- Clonar el repositorio

   2.- Instalar dependencias

   3.- Abrir el notebook

   4.- Ejecutar en orden

