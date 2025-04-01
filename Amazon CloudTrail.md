**Amazon CloudTrail**  
*Monitoriza y Audita la Actividad de tu Cuenta AWS*

---

**Definición**  
- Servicio de **registro de actividad** que rastrea llamadas a la API de AWS.  
- Registra acciones de usuarios, roles, servicios y dispositivos.  

---

**Características Clave**  
- **Registro Continuo**:  
  - Captura eventos de **gestión** (crear, modificar recursos) y **datos** (operaciones en recursos).  
  - Incluye detalles: **quién**, **qué**, **cuándo**, **desde dónde**.  
- **Historial de Eventos**:  
  - Hasta **90 días** de historial gratuito en la consola AWS.  
- **Integración**:  
  - Almacena logs en **Amazon S3** (durable) y envía a **CloudWatch Logs** para alertas.  
  - Compatible con herramientas de SIEM (Ej: Splunk, Sumo Logic).  

---

**Beneficios**  
- **Seguridad**:  
  - Detecta actividad no autorizada o riesgos (Ej: accesos desde IPs sospechosas).  
- **Cumplimiento**:  
  - Facilita auditorías (Ej: PCI-DSS, GDPR).  
- **Operaciones**:  
  - Diagnostica errores (Ej: verifica cambios en configuraciones).  
- **Habilitado por Defecto**:  
  - Activo automáticamente en regiones nuevas.  

---

**Casos de Uso**  
1. **Auditoría**:  
   - Rastrea cambios en IAM, VPC, S3.  
2. **Análisis Forense**:  
   - Investiga incidentes de seguridad paso a paso.  
3. **Automatización**:  
   - Usa logs para activar flujos de trabajo con Lambda.  

---

**Funcionamiento**  
1. **Evento**: Usuario/Rol llama a una API (Ej: `RunInstances`).  
2. **Captura**: CloudTrail registra el evento (JSON).  
3. **Almacenamiento**:  
   - Guarda en S3 (encriptado).  
   - Opcional: CloudWatch para alertas en tiempo real.  

---

**Mejores Prácticas**  
✅ **Habilita en todas las regiones**.  
✅ **Centraliza logs** en un bucket S3 único.  
✅ **Encripta logs** con KMS.  
✅ **Monitorea con CloudWatch** (Ej: alertas por root login).  

---

*CloudTrail = Visibilidad total sobre tu cuenta AWS*  
*Esencial para seguridad, cumplimiento y gobernanza.*