
**Amazon Athena**  

**¿Qué es?**  
▸ **Servicio de consultas serverless** para analizar datos en S3 usando SQL estándar.  
▸ Sin infraestructura que gestionar.  
▸ Ideal para datos estructurados/semi-estructurados (CSV, JSON, Parquet, etc.).  

**Características clave**  
🔹 **Sin servidores**: Escala automáticamente.  
🔹 **Pago por consulta**: Costo por TB de datos escaneados.  
🔹 **Integrado con AWS Glue**: Catálogo de metadatos centralizado.  
🔹 **Rendimiento rápido**: Optimizado con Apache Spark/Presto.  
🔹 **Formatos compatibles**: CSV, JSON, Avro, ORC, Parquet.  

**Casos de uso comunes**  
✔ **Análisis ad-hoc**: Consultas SQL rápidas en S3.  
✔ **Logs y análisis de datos**: Procesamiento de logs (ej: CloudTrail, ELB).  
✔ **ETL ligero**: Transformación de datos antes de cargar en warehouses.  
✔ **Integración con BI**: Conectores para Tableau, QuickSight, etc.  

**Beneficios principales**  
✅ **Costo-eficiente**: Solo pagas por las consultas ejecutadas.  
✅ **Configuración en minutos**: Define esquemas y consulta directamente desde S3.  
✅ **Compatibilidad**: SQL estándar (ANSI) y herramientas populares.  

**Arquitectura simplificada**  
`S3 (Datos) → Athena (SQL) → Resultados en S3/Consola`  
+ **AWS Glue Data Catalog**: Metadatos y esquemas.  

**Ejemplo de uso**  
```sql  
SELECT * FROM mi_tabla_en_s3 WHERE año = 2023;  
```  

**Icono típico en AWS**: 🐘 (símbolo de consultas ágiles).  

---  
