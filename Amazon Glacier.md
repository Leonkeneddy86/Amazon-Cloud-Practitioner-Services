
**Amazon Glacier: Almacenamiento de Archivos de Bajo Costo**  

---

### **¿Qué es Amazon Glacier?**  
- Servicio de almacenamiento **duradero**, **seguro** y **económico** para datos que se acceden con poca frecuencia (*cold storage*).  
- Diseñado para **archivado a largo plazo** y copias de seguridad.  
- **Retrieval time**: Desde minutos hasta horas (dependiendo del tipo de recuperación).  

---

### **¿Para qué sirve?**  
**Casos de uso comunes**:  
- **Backups y recuperación ante desastres**: Respaldos de bases de datos, sistemas empresariales.  
- **Archivado regulatorio**: Datos legales, médicos o financieros (ej. HIPAA, GDPR).  
- **Preservación de datos**: Investigación científica, registros históricos.  
- **Medios y entretenimiento**: Almacenamiento de videos, fotos o música sin acceso frecuente.  

---

### **Beneficios Clave**  
1. **Costo ultra bajo**: Desde **$0.004/GB/mes** (más económico que S3 Standard).  
2. **Durabilidad del 99.999999999%**: Protección contra pérdida de datos.  
3. **Seguridad**: Cifrado AES-256 por defecto y controles de acceso (IAM, VPC Endpoints).  
4. **Escalabilidad**: Sin límites de capacidad; paga solo por lo que usas.  
5. **Integración con AWS**: Uso de **S3 Lifecycle Policies** para mover datos automáticamente a Glacier.  
6. **Cumplimiento normativo**: Certificaciones como ISO, SOC, PCI DSS.  

---

### **Tipos de Almacenamiento en Glacier**  
1. **S3 Glacier**:  
   - Recuperación en **minutos a horas** (Expedited, Standard, Bulk).  
   - Ideal para acceso ocasional (ej. auditorías anuales).  

2. **S3 Glacier Deep Archive**:  
   - Recuperación en **12-48 horas**.  
   - **Costo más bajo** de AWS (ej. datos que rara vez se necesitan).  

---

### **Ejemplos de Retrieval Options**  
| **Tipo**       | **Tiempo de Recuperación** | **Costo**           |  
|----------------|----------------------------|---------------------|  
| **Expedited**  | 1–5 minutos                | Más alto            |  
| **Standard**   | 3–5 horas                  | Medio              |  
| **Bulk**       | 5–12 horas                 | Más económico       |  

---

### **¿Por qué elegir Glacier?**  
- **Alternativa a cintas físicas**: Elimina costos de infraestructura y mantenimiento.  
- **Automatización**: Políticas de ciclo de vida para mover datos de S3 a Glacier sin intervención manual.  
- **Resiliencia**: Datos replicados en múltiples AZs (Availability Zones).  

---
