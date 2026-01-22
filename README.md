Proyecto de Análisis de Clientes – ConnectaTel
🎯 Objetivo del proyecto

El objetivo de este proyecto es analizar el comportamiento de uso de los clientes de ConnectaTel para identificar patrones relevantes, segmentar a los usuarios y generar insights accionables para el negocio. A partir del análisis, se busca entender:

Cómo utilizan los clientes los servicios de mensajes y llamadas.

Qué diferencias existen entre planes (Básico vs Premium).

Qué segmentos de clientes son más valiosos.

Qué oportunidades existen para mejorar o crear nuevos planes comerciales.

🗂️ Datasets utilizados

El análisis se realizó utilizando los siguientes datasets:

1️⃣ users

Contiene información demográfica y de suscripción de los usuarios:

user_id: identificador único del usuario

plan: tipo de plan contratado (Básico / Premium)

age: edad del usuario

city: ciudad del usuario

2️⃣ usage

Registra el historial de uso de los servicios:

user_id: identificador del usuario

type: tipo de interacción (call o text)

duration: duración de la llamada (solo para call)

length: longitud del mensaje (solo para text)

🔍 Etapas del análisis realizadas

Exploración inicial de datos

Revisión de estructura, tipos de variables y valores faltantes.

Tratamiento de valores nulos

Identificación de nulos estructurales en duration y length.

Clasificación de estos nulos como MAR (Missing At Random).

Construcción de métricas de uso por usuario

Total de mensajes enviados.

Total de llamadas realizadas.

Total de minutos de llamadas.

Unificación de datasets

Merge de métricas de uso con información de usuarios.

Análisis estadístico y visualización

Histogramas y boxplots para entender distribuciones y detectar outliers.

Análisis comparativo por tipo de plan.

Identificación de outliers

Uso del método IQR.

Decisión de conservar outliers por representar comportamiento real.

Segmentación de clientes

Segmentación por nivel de uso: Bajo, Medio y Alto uso.

Segmentación por edad: Joven, Adulto y Adulto Mayor.

Insight ejecutivo

Traducción de los hallazgos a conclusiones y recomendaciones de negocio.

▶️ Cómo ejecutar el notebook
Opción recomendada: Google Colab

Abre Google Colab: https://colab.research.google.com/

Sube el notebook (.ipynb) del proyecto.

Asegúrate de subir también los archivos de datos (users.csv, usage.csv).

Ejecuta las celdas en orden de arriba hacia abajo.

Ejecución local (opcional)

Instala Python 3.9 o superior.

Instala las dependencias necesarias:

pip install pandas numpy matplotlib seaborn

Abre el notebook con Jupyter Notebook o Jupyter Lab.

🔁 Guía breve de reproducción

Para reproducir el análisis desde cero:

Cargar los datasets users y usage.

Ejecutar las celdas de limpieza y tratamiento de nulos.

Construir las métricas agregadas de uso por usuario.

Realizar el merge con la información de usuarios.

Generar las visualizaciones y análisis estadísticos.

Ejecutar la segmentación por uso y edad.

Revisar el análisis ejecutivo final.

📌 Resultado final

El proyecto entrega una visión clara del comportamiento de los clientes, identificando segmentos clave y oportunidades comerciales que pueden apoyar la toma de decisiones estratégicas en ConnectaTel.

📈 Este análisis puede ampliarse incorporando métricas de ingresos, churn o evolución temporal del uso.
