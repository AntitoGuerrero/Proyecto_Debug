# 📊 Evaluación de Impacto — Programa “Pasate a Led” (GCBA)

## 📍 Descripción general
Este repositorio contiene el tablero de Power BI y los insumos utilizados para analizar el impacto del programa [***“Pasate a Led”***](https://buenosaires.gob.ar/sites/default/files/2025-03/_Gui%CC%81a%20pra%CC%81ctica_Pasate%20a%20LED.pdf), implementado por el Gobierno de la Ciudad de Buenos Aires (GCBA) entre 2017 y 2019. 
El análisis buscará identificar:
- patrones de participación ciudadana
- ahorro energético
- distribución territorial de los beneficios. 

## 📍 Metodología: fuentes de datos y modelado

Se utilizó un [***dataset***](http://data.buenosaires.gob.ar/dataset/programa-pasate-a-led) provisto por el GCBA, posteriormente procesado y modelado en **Power BI**.

 **El modelo relacional se compone de tres tablas:**

   <img width="404" height="356" alt="image" src="https://github.com/user-attachments/assets/e5528096-2188-4af8-91f7-28a9898990bf" />

1. **Tabla de Actividad**: Registra la cantidad de lámparas LED entregadas por punto verde y período, junto con hogares beneficiados y ahorro energético estimado.
   
2. **Tabla Calendario**: Permite el análisis temporal (día, mes, año, trimestre, semestre).
   
3. **Tabla Puntos Verdes**: Contiene la ubicación, horarios y atributos geográficos de cada punto verde.

➡️ *Las relaciones entre tablas fueron identificadas automáticamente por Power BI*, ***sin necesidad de crear tablas puente***.
    
## 📍 Visualizaciones principales del tablero

 ### 🧩 Índice y navegación principal
 <img width="333" height="149" alt="image" src="https://github.com/user-attachments/assets/58694126-d27e-4a2f-b093-6a492f6d1f16" />

➡️*Esta visualización presenta la información disponible en el tablero y su propósito: “Evaluar para tomar decisiones”*

 ### 🧩 El programa en números
 <img width="320" height="154" alt="image" src="https://github.com/user-attachments/assets/8d420151-148a-4ece-813c-31772132aeab" />

 ➡️*Esta visualización arroja información sobre*: 
   - Ahorro promedio por punto verde 
   - Cantidad de hogares participantes por comuna 
   - Promedio de lámparas intercambiadas por año 
   - Filtros: punto verde, zona, comuna, año, semestre

 ### 🧩 Mapa del ahorro
 <img width="250" height="150" alt="image" src="https://github.com/user-attachments/assets/2b9b8a0a-bb97-4d1b-9e7b-c5c3dc5f5699" />
 
➡️ *Esta visualización refleja la distribución geográfica del ahorro energético por zonas y puntos verdes.* 
*El tamaño y color de los círculos indican el desempeño relativo de cada punto verde respecto al promedio*

 ### 🧩 Análisis de impacto
 <img width="316" height="161" alt="image" src="https://github.com/user-attachments/assets/b53f700d-9aef-4934-99e9-5b0dcb79e13f" />
 
➡️*En esta visualización se puede encontrar un gráfico de dispersión, donde*
  - Eje X: representa ahorro energético
  - Eje Y: refleja la cantidad de lámparas intercambiadas
  - Tamaño de burbuja: indica la cantidad de hogares participantes
  - Línea de tendencia: para visualizar correlación positiva entre variables

## 📍Potencial del tablero
- Permite identificar *zonas y comunas* con ***mayor participación y ahorro***. 
- Facilita la ***comparación temporal y territorial*** de los resultados.
- Ofrece una base para la ***toma de decisiones*** y el diseño de futuras políticas públicas de eficiencia energética.
- Es ***replicable y adaptable*** para otros programas de recambio tecnológico o intervenciones ambientales.
  
## 📍 Límites del tablero
- **Ausencia de parámetros de referencia**: No se dispone de un objetivo cuantitativo de ahorro energético.
- **Evolución de precios**: No se cuenta con información detallada sobre la evolución del precio de las lámparas LED.
- **Datos socioeconómicos**: Ausencia de datos sobre ingresos por comuna/zonas.
- **Enfoque descriptivo**: El tablero es principalmente descriptivo y su mayor valor es simbólico.

## Reflexiones finales
El tablero permite visualizar el alcance y el ahorro energético generado por el programa, pero también evidencia la 
🚨**importancia** 🚨 de contar con ***datos de referencia y variables socioeconómicas***  para una evaluación integral. 

🤓 **El diseño y la evaluación de políticas públicas deben estar en diálogo permanente para maximizar el impacto y la equidad de las intervenciones.**


