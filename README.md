# Evaluación de Impacto — Programa “Pasate a Led” (GCBA)

## Descripción general
Este repositorio contiene el tablero de Power BI y los insumos utilizados para analizar el impacto del programa “Pasate a Led”, implementado por el Gobierno de la Ciudad de Buenos Aires (GCBA) entre 2017 y 2019. El objetivo principal es ofrecer una herramienta de evaluación para funcionarios, técnicos, analistas y estudiantes interesados en la medición de resultados y la toma de decisiones basada en evidencia.

## Objetivo del proyecto
Analizar el impacto del programa “Pasate a Led”, orientado a reducir los efectos medioambientales del consumo eléctrico mediante el recambio gratuito de lámparas tradicionales por lámparas LED. El análisis busca identificar patrones de participación ciudadana, ahorro energético y distribución territorial de los beneficios.

## Descripción del programa
- ### Implementación:
El programa incentivó el recambio de lámparas en “puntos verdes”, espacios de contacto entre el GCBA y la ciudadanía, localizados en plazas y orientados al reciclaje y la educación ambiental.
- ### Mecánica:
Los vecinos acudían a estos puntos para intercambiar lámparas tradicionales por LED de manera gratuita.

## Metodología y fuentes de datos
Se utilizó una base de datos provista por el GCBA, procesada y modelada en Power BI. El modelo relacional incluye tres tablas principales:
1. **Tabla de Actividad**: Registra la cantidad de lámparas LED entregadas por punto verde y período, junto con hogares beneficiados y ahorro energético estimado.
2. **Tabla Calendario**: Permite el análisis temporal (día, mes, año, trimestre, semestre).
3. **Tabla Puntos Verdes**: Contiene la ubicación, horarios y atributos geográficos de cada punto verde.

*Las relaciones entre tablas fueron identificadas automáticamente por Power BI, sin necesidad de crear tablas puente. Se realizaron transformaciones menores, como el ajuste del tipo de variable para los identificadores.*

Diagrama entidad-relación: assets/diagrama_entidad_relacion.png

## Variables y medidas calculadas
- **Medidas principales**:
  - Ahorro promedio por punto verde (kWh)
  - Cantidad de puntos verdes activos
  - Promedio de lámparas intercambiadas por punto verde
  - Cantidad de lámparas por año y punto verde
  - $$ Invertido por año (ajustado por inflación para años posteriores a 2017)

- **Columnas calculadas**:
  - *Nivel de ahorro*: Categorización de cada actividad en “alto” o “bajo” según el promedio general.
  - *Zonas*: Agrupación de comunas en norte, centro y sur según la segmentación estratégica del GCBA.

- ## Medidas avanzadas:
  - Cálculo de inversión ajustada por inflación (supuesto: evolución de precios igual a inflación general).
  - Análisis de correlación entre ahorro energético, cantidad de lámparas y hogares participantes (limitado por las capacidades de DAX para calcular coeficientes de correlación).
    
## Visualizaciones principales del tablero
1. ### Índice y navegación principal
Esta visualización presenta la información disponible en el tablero y su propósito: “Evaluar para tomar decisiones”.
Imagen: assets/indice_tablero.png

2. ### El programa en números
  - Ahorro promedio por punto verde (gráfico de anillos)
  - Cantidad de hogares participantes por comuna (barras)
  - Promedio de lámparas intercambiadas por año (barras)
  - Filtros: punto verde, zona, comuna, año, semestre
Imagen: assets/programa_en_numeros.png

3. ### Mapa del ahorro
Distribución geográfica del ahorro energético por zonas y puntos verdes. El tamaño y color de los círculos indican el desempeño relativo de cada punto verde respecto al promedio.
Imagen: assets/mapa_ahorro.png

4. ### Análisis de impacto
**Gráfico de dispersión**:
  - Eje X: ahorro energético
  - Eje Y: cantidad de lámparas
  - Tamaño de burbuja: cantidad de hogares participantes
  - Línea de tendencia para visualizar correlación positiva entre variables
Imagen: assets/analisis_impacto.png

## Alcances y potencial del tablero
  - Permite identificar zonas y comunas con mayor participación y ahorro.
  - Facilita la comparación temporal y territorial de los resultados.
-   Ofrece una base para la toma de decisiones y el diseño de futuras políticas públicas de eficiencia energética.
-   Es replicable y adaptable para otros programas de recambio tecnológico o intervenciones ambientales.
  
## Límites y consideraciones
 - **Ausencia de parámetros de referencia**: No se dispone de un objetivo cuantitativo de ahorro energético.
  - **Evolución de precios**: No se cuenta con información detallada sobre la evolución del precio de las lámparas LED.
  - **Datos socioeconómicos**: Ausencia de datos sobre ingresos por comuna/zonas.
  - **Capacidades técnicas**: Algunas métricas avanzadas no pudieron ser implementadas completamente en DAX.
  - **Enfoque descriptivo**: El tablero es principalmente descriptivo y su mayor valor es simbólico.

## Reflexiones finales
El tablero permite visualizar el alcance y el ahorro energético generado por el programa, pero también evidencia la importancia de contar con datos de referencia y variables socioeconómicas para una evaluación integral. El diseño y la evaluación de políticas públicas deben estar en diálogo permanente para maximizar el impacto y la equidad de las intervenciones.


