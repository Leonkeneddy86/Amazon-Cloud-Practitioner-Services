
**Amazon S3 y AWS CLI**  
*Clases de almacenamiento en la nube*  

---

### **¿Qué es Amazon S3?**  
**Amazon Simple Storage Service (S3)** es un servicio de almacenamiento de objetos escalable, duradero y de alta disponibilidad. Permite almacenar y recuperar cualquier cantidad de datos desde cualquier lugar.  

**Características clave:**  
- **Escalabilidad ilimitada**  
- **Durabilidad del 99.999999999% (11 nueves)**  
- **Disponibilidad del 99.99%**  
- **Seguridad integrada** (encriptación, control de acceso)  

---

### **AWS CLI (Command Line Interface)**  
Herramienta oficial de AWS para interactuar con los servicios mediante la terminal.  

**Comandos básicos:**  
```bash
aws s3 ls                          # Listar buckets
aws s3 cp archivo.txt s3://mi-bucket/  # Subir archivo
aws s3 sync carpeta/ s3://mi-bucket/   # Sincronizar directorio
```

---

### **Clases de almacenamiento en S3**  

| **Clase**                | **Caso de uso**                     | **Disponibilidad** | **Durabilidad** | **Costo** |
|--------------------------|-------------------------------------|--------------------|-----------------|-----------|
| **S3 Standard**          | Datos accedidos frecuentemente      | 99.99%             | 99.999999999%   | Alto      |
| **S3 Intelligent-Tiering** | Datos con patrones de acceso variables | 99.9%              | 99.999999999%   | Variable  |
| **S3 Standard-IA**       | Datos accedidos con poca frecuencia | 99.9%              | 99.999999999%   | Medio     |
| **S3 One Zone-IA**       | Datos no críticos, baja frecuencia | 99.5% (1 zona)     | 99.999999999%   | Bajo      |
| **S3 Glacier**           | Archivo a largo plazo (min. 90 días) | Minutos/horas      | 99.999999999%   | Muy bajo  |
| **S3 Glacier Deep Archive** | Backup y compliance (min. 180 días) | Horas              | 99.999999999%   | Más bajo  |

---

### **¿Cuándo usar cada clase?**  
- **Standard**: Aplicaciones web, big data.  
- **Intelligent-Tiering**: Datos con acceso impredecible.  
- **Standard-IA/One Zone-IA**: Copias de seguridad, logs.  
- **Glacier/Deep Archive**: Auditorías, archivos históricos.  

