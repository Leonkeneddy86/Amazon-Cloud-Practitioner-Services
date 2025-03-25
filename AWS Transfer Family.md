
# **AWS Transfer Family**  

### **¿Qué es?**  
AWS Transfer Family es un servicio **completamente administrado** que permite transferir archivos de manera segura hacia y desde Amazon S3 o Amazon EFS utilizando protocolos estándar como:  

- **SFTP** (SSH File Transfer Protocol)  
- **FTPS** (FTP sobre SSL/TLS)  
- **FTP** (File Transfer Protocol)  
- **AS2** (Applicability Statement 2)  

### **Beneficios clave**  
✅ **Sin servidores que administrar**: AWS maneja la infraestructura.  
✅ **Alta disponibilidad**: Diseñado para ser tolerante a fallos.  
✅ **Seguridad integrada**: Integración con IAM, AWS KMS y VPC.  
✅ **Escalable**: Se adapta a las necesidades de carga de trabajo.  
✅ **Pago por uso**: Solo pagas por lo que utilizas.  

### **Casos de uso comunes**  
- Intercambio seguro de archivos con socios y clientes.  
- Migración de sistemas legacy basados en FTP a la nube.  
- Almacenamiento centralizado en S3/EFS con acceso mediante protocolos tradicionales.  

### **¿Cómo funciona?**  
1. **Configuras** un servidor virtual con el protocolo deseado.  
2. **Defines usuarios** (autenticación con IAM, Active Directory o personalizada).  
3. **Conectas** clientes FTP/SFTP/FTPS/AS2 para subir o descargar archivos.  
4. **Los archivos se almacenan** directamente en S3/EFS.  

📌 **Ideal para empresas que necesitan mantener flujos de trabajo tradicionales sin gestionar infraestructura.**  

# **AWS Transfer Family: Configuración y Precios**  

## **🔧 Configuración Básica**  

### **1. Crear un servidor de transferencia**  
- **Paso 1:** Ve a **AWS Transfer Family** en la consola de AWS.  
- **Paso 2:** Elige el protocolo (**SFTP, FTPS, FTP o AS2**).  
- **Paso 3:** Configura la autenticación (**IAM, Active Directory, personalizada**).  
- **Paso 4:** Define el almacenamiento (**Amazon S3 o Amazon EFS**).  
- **Paso 5:** Asigna una VPC y subredes para aislamiento de red.  

### **2. Configurar usuarios y permisos**  
- **Usuarios IAM:** Cada usuario necesita una política que defina acceso a buckets S3 o rutas EFS.  
- **Autenticación externa:** Puedes usar Microsoft AD o LDAP.  

### **3. Conectar clientes**  
- **Ejemplo SFTP:**  
  ```bash
  sftp -i clave_privada.pem usuario@tu-servidor.server.transfer.region.amazonaws.com
  ```  
- **Ejemplo FTP/FTPS:** Usa clientes como FileZilla con credenciales configuradas.  

---

## **💰 Precios (Pago por uso, sin costos iniciales)**  

### **1. Costo por hora del servidor**  
| **Protocolo**  | **Costo por hora (EE.UU. Este - N. Virginia)** |  
|---------------|----------------------------------|  
| SFTP          | $0.30 USD                        |  
| FTPS          | $0.30 USD                        |  
| FTP           | $0.30 USD                        |  
| AS2           | $0.45 USD                        |  

### **2. Costo por transferencia de datos**  
- **$0.04 USD por GB** transferido (entrante y saliente).  

### **3. Almacenamiento (S3/EFS)**  
- **Amazon S3:** Desde $0.023 USD/GB/mes (Standard).  
- **Amazon EFS:** Desde $0.08 USD/GB/mes (Elástico).  

### **4. Ejemplo de costo mensual estimado**  
- **1 servidor SFTP (24/7):** ~$216 USD/mes ($0.30/h × 720h).  
- **100 GB transferidos:** ~$4 USD.  
- **Total aproximado:** **$220 USD/mes** (sin incluir almacenamiento S3/EFS).  

---

## **📌 Recomendaciones para reducir costos**  
✔ **Escalar según demanda:** Apaga servidores si no se usan 24/7.  
✔ **Usar S3 Intelligent-Tiering:** Para optimizar costos de almacenamiento.  
✔ **Monitorear con CloudWatch:** Evitar transferencias innecesarias.  



