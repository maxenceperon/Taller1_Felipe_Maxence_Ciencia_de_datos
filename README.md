# Taller 1

## Integrantes  
- Diego Felipe Tolosa Gamez
- Maxence Péron

## Objetivo y alcance  
El objetivo de este proyecto es analizar el comportamiento de las reservas hoteleras con el fin de identificar los factores que influyen en las cancelaciones y en la ocupación de los hoteles. A partir de un dataset de reservas, se busca extraer información útil que permita proponer estrategias para reducir la tasa de cancelación y mejorar la gestión de la demanda.  

El alcance incluye:  
- Procesamiento y limpieza de datos.  
- Análisis exploratorio de datos (EDA).  
- Identificación de patrones de comportamiento en las reservas.  
- Elaboración de reportes y recomendaciones estratégicas para cadenas hoteleras.  

## Estructura del proyecto  
El repositorio se organiza de la siguiente manera:  

- **documents/**  
  - `Taller_1.pdf`: enunciado del taller.  
  - `Hotel Bookings Demand Data Dictionary.xlsx`: diccionario de datos que explica cada atributo de la base de datos.  
  - `Reporte de Entendimiento.pdf`: documento con el entendimiento inicial del dataset y el análisis univariado de los atributos más relevantes.  
  - `Informe Ejecutivo de Recomendaciones Estratégicas.pdf`: informe final que presenta los insights obtenidos y recomendaciones prácticas para la gestión hotelera.  

- **data/**  
  - `hotel_bookings_modified.csv`: base de datos original en bruto.  
  - `hotel_bookings_clean.csv`: base de datos limpia generada a partir del notebook de limpieza.  

- **cleaning.ipynb**: notebook que procesa y limpia los datos, generando el archivo `hotel_bookings_clean.csv`.  
- **eda.ipynb**: notebook que realiza el análisis exploratorio de datos sobre la versión limpia.  
- **requirements.txt**: archivo con los paquetes necesarios para ejecutar el proyecto.  
- **README.md**: este archivo, que explica el proyecto.  

## Ejecución  
1. Instalar los requerimientos del archivo `requirements.txt`:  
   ```bash
   pip install -r requirements.txt
   ```
2. Ejecutar el notebook `cleaning.ipynb`. Esto generará el archivo `hotel_bookings_clean.csv` dentro de la carpeta `data/`.
> Nota: este archivo no existe inicialmente y debe ser creado en este paso.
3. Ejecutar el notebook `eda.ipynb` para realizar el análisis exploratorio de datos y obtener los insights.

## Principales insights
Del análisis realizado en `eda.ipynb` y documentado en los reportes, se destacan los siguientes hallazgos:
- Aproximadamente el 41% de las reservas terminan cancelándose, lo que representa un reto importante para la ocupación hotelera.
- Las reservas hechas con mucha antelación (más de 69 días) presentan más cancelaciones que aquellas realizadas con menos tiempo de anticipación (menos de 26 días).
- El segmento de grupos y las agencias en línea muestran las tasas de cancelación más altas, mientras que el segmento corporativo es el más estable.
- Los *city hotels* presentan una tasa de cancelación mucho mayor (69%) en comparación con los *resort hotels* (28%).
- Pesé a que los *city  hotels* representan el 32% de las reservas también representan el 54.5% de las cancelaciones.
- Las reservas con tarifas más altas tienden a cancelarse con más frecuencia, lo que sugiere que los precios influyen en la decisión final del cliente.

Estos resultados fueron utilizados para elaborar el `Informe Ejecutivo de Recomendaciones Estratégicas.pdf`, donde se presentan conclusiones y propuestas prácticas orientadas a la reducción de cancelaciones y a la optimización de la ocupación en las cadenas hoteleras.