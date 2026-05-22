# especializacionbigdata
## Pipelines de Orquestación
### Azure Datafactory
El pipeline presentado corresponde a un flujo de procesamiento de datos bajo una arquitectura tipo Medallion en Databricks, compuesto por cuatro notebooks encadenados secuencialmente. El proceso inicia con NB-INGEST-DATA, encargado de la ingesta y carga de datos desde las fuentes origen hacia la capa inicial del ecosistema. Posteriormente, NB-SILVER-DATA realiza procesos de depuración, validación, normalización y transformación de los datos para garantizar calidad y consistencia. Luego, NB-GOLD-DATA consolida y estructura la información de negocio mediante agregaciones y modelos analíticos optimizados para consumo corporativo. Finalmente, NB-GOLD-MODEL ejecuta la generación de modelos, métricas o artefactos analíticos avanzados sobre la información refinada de la capa Gold.

<img width="1181" height="269" alt="image" src="https://github.com/user-attachments/assets/37929356-ea1a-46b7-9a18-be582f9288db" />

### Job DBW
El job presentado implementa un flujo de procesamiento de datos especializado bajo una arquitectura medallion en Databricks, orquestado mediante tareas secuenciales con dependencias controladas. La etapa Bronce ejecuta el notebook NB-BRONZE-INGEST-DATA, responsable de la ingesta inicial y almacenamiento de datos crudos provenientes de las fuentes transaccionales (Kaggle). Posteriormente, la capa Silver ejecuta NB-SILVER-PROCESS-DATA, donde se aplican procesos de limpieza, homologación, validaciones de calidad y transformaciones de negocio para estructurar la información analítica.

La siguiente etapa, Gold, ejecuta NB-GOLD-LOAD-DATA, encargado de consolidar y disponibilizar datasets curados y optimizados para consumo analítico y modelos avanzados. Finalmente, el proceso MODEL_PREDICT_RATING ejecuta el notebook NB-MODEL-PREDICT, donde se realiza la inferencia o ejecución del modelo predictivo sobre la información refinada de la capa Gold, permitiendo generar resultados analíticos y predicciones requeridas.

<img width="1060" height="150" alt="image" src="https://github.com/user-attachments/assets/7289409a-2e1b-41f8-8c06-7e741ce3f1fc" />


## Pruebas
### Azure Datafactory
<img width="1275" height="737" alt="image" src="https://github.com/user-attachments/assets/87bcbb1e-dde9-43f8-af18-158b9606d1e1" />

### Job DBW
<img width="1304" height="459" alt="image" src="https://github.com/user-attachments/assets/c83cd3ad-b6e0-48a3-b1f4-7a1d1e2387eb" />


## Tablero Power BI.
https://unaulaedu.sharepoint.com/:u:/s/BigData/IQCdNtpqS1GbRJR1cCFuU2LzAcGw32uAsx4M65CRiJCcs7w?e=F7dEwv
