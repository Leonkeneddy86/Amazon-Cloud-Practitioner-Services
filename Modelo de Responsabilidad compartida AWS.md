
![[Shared_Responsibility_Model_V2.5.jpg]]

El **Modelo de Responsabilidad Compartida de AWS** divide las obligaciones de seguridad entre AWS y el cliente, permitiendo una gestión eficiente de la infraestructura en la nube. A continuación, se detallan sus aspectos clave:

---

### **Responsabilidades:**
1. **AWS (Seguridad *DE* la nube):**
   - **Infraestructura física:** Centros de datos, hardware, redes, energía y refrigeración.
   - **Global Infrastructure:** Regiones, Zonas de Disponibilidad y Edge Locations.
   - **Servicios básicos:** Seguridad física, redundancia, cumplimiento de certificaciones (ISO, SOC, etc.) y mantenimiento de la disponibilidad.

2. **Cliente (Seguridad *EN* la nube):**
   - **Datos:** Encriptación, integridad, backups y gestión del ciclo de vida.
   - **Aplicaciones:** Configuración segura, parches y gestión de vulnerabilidades.
   - **Acceso:** Identity & Access Management (IAM), autenticación multifactor y políticas de permisos.
   - **Red y sistemas operativos:** Configuración de firewalls, grupos de seguridad, y actualizaciones del SO.
   - **Encriptación:** Claves de encriptación (si el cliente las gestiona) y protección del tráfico de red.

---

### **Beneficios:**
- **Reducción de costos iniciales:** Elimina la inversión en hardware, mantenimiento físico y personal especializado en infraestructura.
- **Escalabilidad:** Ajuste dinámico de recursos según demanda (ej: Auto Scaling, Lambda).
- **Enfoque en el negocio:** El cliente se concentra en desarrollar aplicaciones y servicios, no en infraestructura.
- **Alta disponibilidad:** AWS garantiza redundancia en zonas geográficas y recuperación ante desastres.
- **Cumplimiento normativo:** AWS cumple con estándares globales, facilitando auditorías para el cliente.

---

### **Costos:**
- **Modelo "pay-as-you-go":** Pago por uso de servicios (ej: EC2, S3, RDS). Ideal para empresas con demanda fluctuante.
- **Ahorros a largo plazo:** Opciones como Reserved Instances o Savings Plans reducen costos en cargas de trabajo estables.
- **Costos potenciales a vigilar:**
  - Transferencia de datos salientes (egress).
  - Almacenamiento no optimizado (ej: S3 sin políticas de lifecycle).
  - Recursos huérfanos (ej: instancias EC2 detenidas pero no terminadas).
  - Servicios premium (ej: GuardDuty, Inspector).

---

### **Riesgos y Desafíos:**
- **Configuraciones incorrectas:** Errores en grupos de seguridad o buckets S3 públicos pueden causar brechas.
- **Falta de gestión proactiva:** No aplicar parches o monitorizar accesos incrementa vulnerabilidades.
- **Desconocimiento del modelo:** Algunos clientes asumen que AWS cubre todo, lo que lleva a negligencia en su parte.

---

### **Comparación con Otros Modelos:**
- **On-Premise:** El cliente es 100% responsable (desde el hardware hasta las aplicaciones). Mayor control, pero costos y complejidad elevados.
- **Otros proveedores cloud (Azure, GCP):** Modelos similares, pero con diferencias en servicios específicos y herramientas de gestión.

---

### **Mejores Prácticas para Clientes:**
1. **Automatizar seguridad:** Usar AWS Config, CloudFormation y AWS Backup.
2. **Gestionar acceso:** Implementar IAM con mínimos privilegios y MFA.
3. **Monitorizar:** Utilizar CloudWatch, GuardDuty y CloudTrail.
4. **Encriptar datos:** Usar AWS KMS o claves propias para datos sensibles.
5. **Educar equipos:** Capacitar en Well-Architected Framework y Shared Responsibility Model.

---

### **Ejemplo Práctico:**
- **Caso:** Una startup usa EC2 y RDS.
  - **AWS:** Garantiza la disponibilidad del servidor físico y la red.
  - **Cliente:** Debe configurar grupos de seguridad, aplicar parches al SO, gestionar backups de RDS y encriptar datos sensibles.

---

### **Conclusión:**
El modelo permite a las empresas innovar rápidamente con menor costo inicial, pero exige responsabilidad activa en seguridad y gestión. La clave está en entender qué aspectos controla cada parte y utilizar las herramientas de AWS para mitigar riesgos.