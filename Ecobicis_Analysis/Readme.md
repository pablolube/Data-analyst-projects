# Análisis de Datos: EcoBicis CABA

![EcoBici Banner](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ8Ad17Ry6HR-vjCbOoEjJZRp6_QJ-l5bXZaw&s)

## Descripción del Proyecto
Este proyecto analiza datos del sistema de bicicletas públicas **EcoBici** de la Ciudad de Buenos Aires. EcoBici es un sistema de bicicletas compartidas que funciona en la ciudad, permitiendo a los usuarios realizar viajes gratuitos tras un registro previo.
``
El objetivo del proyecto es explorar, limpiar y analizar los datos proporcionados por el [Portal de Datos Abiertos del Gobierno de la Ciudad de Buenos Aires](https://data.buenosaires.gob.ar/dataset/bicicletas-publicas) para obtener insights sobre los patrones de uso del sistema, como la duración de los viajes, el género de los usuarios y las estaciones más populares.

---

## Sistema EcoBici
- **Inicio del Sistema:** Operado por Tembici desde 2019.
- **Capacidad:** 200 estaciones y 1.200 bicicletas.
- **Usuarios Activos (2019):** Más de 600.000 usuarios realizaron 8 millones de viajes.
- **Restricciones:** En 2020, el sistema fue limitado a 30 minutos de uso por viaje debido a la pandemia.
- **Cobertura:** Presente en 30 de los 48 barrios de la ciudad.

---

## Estructura del Dataset
El dataset contiene la siguiente información:

| Columna                      | Tipo de Dato | Descripción                                          |
|------------------------------|--------------|------------------------------------------------------|
| `Unnamed: 0`                | int64        | Índice del registro.                                |
| `Id_recorrido`              | object       | Identificador del recorrido.                        |
| `duracion_recorrido`        | object       | Duración del recorrido (HH:MM:SS).                  |
| `fecha_origen_recorrido`    | object       | Fecha y hora de inicio del recorrido.               |
| `id_estacion_origen`        | object       | ID de la estación de origen.                        |
| `nombre_estacion_origen`    | object       | Nombre de la estación de origen.                    |
| `direccion_estacion_origen` | object       | Dirección de la estación de origen.                 |
| `long_estacion_origen`      | float64      | Longitud de la estación de origen.                  |
| `lat_estacion_origen`       | float64      | Latitud de la estación de origen.                   |
| `fecha_destino_recorrido`   | object       | Fecha y hora de fin del recorrido.                  |
| `id_estacion_destino`       | object       | ID de la estación de destino.                       |
| `nombre_estacion_destino`   | object       | Nombre de la estación de destino.                   |
| `direccion_estacion_destino`| object       | Dirección de la estación de destino.                |
| `long_estacion_destino`     | float64      | Longitud de la estación de destino.                 |
| `lat_estacion_destino`      | float64      | Latitud de la estación de destino.                  |
| `id_usuario`                | object       | ID del usuario.                                      |
| `modelo_bicicleta`          | object       | Modelo de la bicicleta utilizada.                   |
| `género`                   | object       | Género del usuario.                                  |

---

## Objetivos del Proyecto
1. **Limpieza de Datos:**
   - Identificar y manejar datos faltantes, duplicados o inconsistentes.
   - Transformar columnas como `duracion_recorrido` para un análisis cuantitativo.

2. **Análisis Exploratorio (EDA):**
   - Determinar patrones de uso como horarios pico y duración promedio de viajes.
   - Analizar la popularidad de las estaciones de origen y destino.
   - Explorar diferencias en el uso del sistema según género.

3. **Visualizaciones:**
   - Crear gráficos para representar los patrones de uso.
   - Mapas interactivos de estaciones más utilizadas.

4. **Modelos Predictivos (opcional):**
   - Predecir la demanda futura en estaciones específicas usando Machine Learning.


## Herramientas Utilizadas
- **Lenguajes:** Python.
- **Librerías:**
  - Manipulación y Análisis: `pandas`, `numpy`.
  - Visualización: `matplotlib`, `seaborn`, `folium` (mapas).
  - Procesamiento de Fechas: `datetime`.

---

## Referencias
- [Portal de Datos Abiertos de la Ciudad de Buenos Aires](https://data.buenosaires.gob.ar/dataset/bicicletas-publicas)
- [EcoBici](https://www.buenosaires.gob.ar/ecobici)

