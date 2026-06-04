# everpeak-analysis
## Resumen Ejecutivo
                    
# Contexto y Objetivo:
En este análisis nos interesa saber que relación existe entre la movilidad urbana y la productividad económica, en el 2024, en ciudades latinoamericanas. Para esto se utilizarán dos fuentes (Datasets):

- Movilidad Urbana
- Economía Urbana
- Cobertura de datos:
- Se analizan únicamente los resultados del año 2024, de 15 ciudades en 7 paises latinoameericanos.

# Metodología:
Para limpiar nuestros datos y prepararlos para el análisis, comenzamos estandarizando los nombres de las columnas (poniendo texto en minúsulas y separando con _ las palabras). Corregimos los formatos de las columnas de nuestras tablas, dejando las fechas en formato datetime, de esta manera podremos extraér y filtrar únicamente el año que vamos a analisar. En las columnas con datos numéricos, dejamos los números sin símbolos y reemplasando separadores de miles (,) por punto para posteriormente convertir a formato float para conservar los decimales. Se creó una copia de los datasets para no modificar los originales. Posteriormente agrupamos por Ciudad, País y Año en ambos para unirlos (usando las columnas relevantes de cada uno), mediante Inner, de este modo podemos mantener las ciudades y años presentes en ambos datasets. Como validación visual creamos las siguientes gráficas:

1.- Boxplot
Para ver la distribución de los minutos de retraso con un promedio de 629.52

2.- Histograma
De esta forma podemos observar la distribución del PIB per Cápita en las Ciudades, generando la consentración alrededor de los 10,000.

3.- Gráficos de Barras
Para estos gráficos unimos ambos indicadores de los gráficos anteriores para compararlos a la par.

a)
Comparamos el retraso por congestión con el PIB per Cápita, al tener parámetros muy distintos no es complicado observar con claridad la comparación que buscamos. Es por eso que creamos una gráfica (b).

b)
Normalizamos las columnas para tener unos valores que sean más fáciles de comparar en la gráfica sin perder la perspectiva, de esta forma nuestra gráfica de barras visualmente es más clara.

Hallazgos iniciales:
Haciendo un análisis de comparación entre el PIB per cápita de cada ciudad en el 2024 y los minutos de retraso de congestionamiento viál, se observa lo siguiente: No necesariamente existe una relación entre PIB y la congestión. En ciudades como México, Bogotá y Sao Paulo, pareciera que van de la mano. Sin embargo, en el resto de los paises no se ve clara una relación entre PIB y la congestión.

¿Qué ciudades de América Latina presentan alta congestión y baja productividad económica?

En Santiago podemos observar la alta congestión en comparación de la productividad económica, seguido por México, sin embargo la productividad en México si tiene mayor relación con la alta congestión que en Santiago.

¿Cuáles muestran los mejores indicadores combinados (movilidad eficiente y economía fuerte)?

En Brasilia, Belo horizonte, Fortaleza, Montevideo, Buenos Aires, Curitiba, Porto Alegre, Recife, Río de Janeiro y Salvador, definitivamente su productividad es fuerte y presentan indicadores de baja congestión, lo que nos indica una eficiente movilidad.

¿Qué variables parecen tener una relación más fuerte con el desarrollo urbano?

Me pare qeu las variable que tienen una relación más fuerte con el desarrollo urbano serían, la población y los índices de contaminación.

# Recomendaciones
Valdría la pena agregar al análisis: la población y el índice de contaminación de cada Ciudad, de esta forma tendríamos una información más clara para determinar si efectivamente la fuerza de su economía está ligada o no a la movilidad. 
Estudiaría más a fondo el caso de Montevideo que aparentemente tiene una excelente movilidad con una productividad impactante. Y a su ves consideraría países como México y Sao Paulo como Ciudades candidatas para invertir en infraestructura de transporte.  
