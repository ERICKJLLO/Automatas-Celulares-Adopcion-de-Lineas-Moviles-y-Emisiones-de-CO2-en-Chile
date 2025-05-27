# Autómatas Celulares para Modelar la Adopción de Líneas Móviles y Emisiones de CO₂ en Chile

Este proyecto explora el uso de **Autómatas Celulares (AC)** como herramienta computacional para modelar fenómenos sociales, específicamente la **adopción de líneas móviles** en Chile y su relación con las **emisiones de dióxido de carbono (CO₂)**. Se propone una simulación basada en reglas locales para observar comportamientos emergentes a nivel nacional.

> Desarrollado como parte del curso de *fundamentos de programacion cientidica* en la *Universidad de Medellín*.

---

## Objetivo del Proyecto

- Simular el comportamiento de adopción de líneas móviles en una población ficticia.
- Evaluar cómo la adopción masiva impacta las emisiones estimadas de CO₂, derivadas del uso de infraestructura tecnológica (torres, dispositivos, energía).
- Demostrar cómo modelos simples (AC) pueden capturar dinámicas complejas del mundo real.

---

## Motivación

El crecimiento acelerado del uso de teléfonos móviles tiene un impacto ambiental no despreciable. En Chile, con una alta tasa de penetración móvil, entender cómo evoluciona este fenómeno es clave para tomar decisiones sostenibles. Este modelo busca:

- Proveer una herramienta exploratoria para investigadores y tomadores de decisiones.
- Concientizar sobre los impactos indirectos del uso tecnológico.
- Integrar informática, sociología y medio ambiente en una simulación accesible.

---

## Metodología

Se usa un autómata celular bidimensional donde:

- Cada celda representa un individuo con o sin línea móvil.
- El estado de cada celda evoluciona en función de sus vecinos (regla de transición).
- Se incorporan factores como presión social, infraestructura disponible y políticas de adopción.
- Se calcula una métrica estimada de emisiones acumuladas según la cantidad de usuarios activos.

---

## Resultados principales

- **Visualizaciones del patrón de adopción**: crecimiento rápido, saturación, zonas de retardo.
- **Gráficas de emisiones acumuladas** de CO₂ por periodo de tiempo.
- Análisis de **escenarios con diferentes parámetros** (influencia social, infraestructura limitada, adopción forzada).
- Observación de **dinámicas emergentes** como clusters, resistencia a la adopción o efecto de red.

---



## Tecnologías y librerías usadas

- **Python 3.10+**
- **Jupyter Notebook**
- **NumPy** – para manejo de la matriz del autómata
- **Matplotlib** – para visualizaciones y animaciones
- **time** – para mediciones de rendimiento


---

## Parámetros configurables

- `prob_adopcion`: probabilidad base de adoptar una línea móvil.
- `vecinos_influyentes`: número mínimo de vecinos con línea para que una celda adopte.
- `capacidad_maxima`: límite de infraestructura (simula saturación de red).
- `coef_emision`: factor que relaciona usuarios activos con emisiones de CO₂.

Estos valores se pueden ajustar fácilmente desde las celdas iniciales del notebook.

## Métricas calculadas

- Número total de usuarios activos por iteración.
- Gráfica de emisiones acumuladas de CO₂.
- Evolución del patrón espacial de adopción.
- Tiempos de convergencia y saturación.

## Posibles mejoras futuras

- Incorporación de datos reales por región (INE, Subtel, etc).
- Validación con datos históricos de adopción en Chile.
- Inclusión de factores económicos o políticas de subsidio.
- Implementación en plataformas interactivas tipo web con Streamlit.


