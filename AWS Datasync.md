
**AWS DataSync**  
*Transferencia de datos rápica, segura y sencilla*  

---

### **¿Qué es AWS DataSync?**  
Servicio **administrado** de AWS diseñado para:  
- **Transferir datos** a gran escala entre **entornos locales** y **AWS**.  
- **Sincronizar datos** entre almacenamientos en la nube (Amazon S3, EFS, FSx).  
- **Automatizar y acelerar** migraciones, copias de seguridad y flujos de trabajo híbridos.  

---  

### **Características clave**  
✅ **Rápido**: Usa protocolos optimizados y paralelización para transferencias **10x más rápidas** que herramientas estándar.  
✅ **Seguro**: Cifrado en tránsito (TLS) y en reposo, integración con IAM y AWS KMS.  
✅ **Sencillo**: Configuración con pocos clics, sin necesidad de scripts personalizados.  
✅ **Monitoreo**: Integración con Amazon CloudWatch para seguimiento de tareas.  

---  

### **Casos de uso comunes**  
1. **Migración a la nube**: Mover petabytes de datos desde NAS/SAN locales a Amazon S3 o EFS.  
2. **Copia de seguridad**: Replicar datos críticos en AWS para recuperación ante desastres (DR).  
3. **Procesamiento de datos**: Sincronizar datos con AWS para análisis con servicios como Athena o EMR.  

---  

### **¿Cómo funciona?**  
1. **Despliega el agente** (en servidores locales o EC2).  
2. **Crea tareas de transferencia** (origen → destino).  
3. **Ejecuta y monitorea** desde la consola de AWS.  

---  

### **Beneficios vs. alternativas**  
🆚 **Vs. Rsync/SCP**: Más rápido, automatizado y con manejo de errores.  
🆚 **Vs. Snowball**: Ideal para transferencias recurrentes o menores a 10TB.  

---  

**📌 Conclusión**: DataSync simplifica la transferencia de datos hacia/mientras AWS, reduciendo tiempo, costos y complejidad operacional.  
