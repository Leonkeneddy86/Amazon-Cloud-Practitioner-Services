
**AWS Snowball**  

**¿Qué es?**  
AWS Snowball es un servicio de transferencia de datos físicos que permite mover grandes volúmenes de información hacia y desde AWS de manera segura y eficiente, sin depender de conexiones de red lentas o costosas.  

**Características principales:**  
- **Dispositivos físicos:** AWS envía un dispositivo Snowball resistente y portátil con alta capacidad de almacenamiento.  
- **Alta capacidad:**  
  - **Snowball:** 50 TB o 80 TB por dispositivo.  
  - **Snowball Edge:** Incluye capacidad de computación (opciones de 100 TB o 100 TB con GPU).  
- **Cifrado seguro:** Todos los datos se protegen con cifrado AES-256 bit.  
- **Rápido:** Mucho más veloz que la transferencia por Internet (hasta 5 veces más rápido).  

**Casos de uso comunes:**  
✅ Migración de grandes volúmenes de datos a la nube.  
✅ Backup y recuperación ante desastres.  
✅ Análisis de datos locales sin conexión.  
✅ Transferencia de datos desde ubicaciones remotas con Internet limitado.  

**Proceso de uso:**  
1. **Solicitar un Snowball** desde la consola de AWS.  
2. **Conectar el dispositivo** a tu red local y copiar los datos.  
3. **Devolverlo a AWS** para que carguen los datos en tu cuenta.  

**Beneficios:**  
✔ **Ahorro de tiempo y ancho de banda.**  
✔ **Seguridad mejorada** (sin riesgos de transferencia en línea).  
✔ **Sin costos de infraestructura adicional.**  

**¿Cuándo usarlo?**  
- Cuando transferir por Internet tomaría **más de una semana**.  
- Cuando hay **limitaciones de red** (ej: conexiones lentas o inestables).  

**Precio:**  
- Basado en el alquiler del dispositivo y la cantidad de datos transferidos.  

**Conclusión:**  
AWS Snowball es la solución ideal para mover **grandes cantidades de datos** de forma **segura, rápida y económica**.  

---  
### **Ejemplos Prácticos de AWS Snowball**  

#### **1. Migración de Datos desde un Data Center Local**  
**Situación:** Una empresa quiere migrar **500 TB** de datos históricos (archivos, bases de datos, backups) a AWS, pero su conexión a Internet es lenta (100 Mbps).  
**Problema:** Transferir 500 TB por Internet tomaría **más de 1 año**.  
**Solución:**  
- Solicitar **varios dispositivos Snowball** (ej: 7 Snowballs de 80 TB cada uno).  
- Copiar los datos en los dispositivos (usando la herramienta AWS Snowball Client).  
- Enviarlos de vuelta a AWS, donde los datos se cargarán automáticamente en **Amazon S3**.  
**Resultado:** Migración completada en **2-3 semanas** en lugar de más de un año.  

---  

#### **2. Backup de Datos Críticos en la Nube**  
**Situación:** Un hospital necesita respaldar **200 TB** de registros médicos (imágenes MRI, historias clínicas) en AWS para cumplir con regulaciones.  
**Problema:**  
- La red del hospital no soporta transferencias masivas sin afectar operaciones diarias.  
- Los datos son sensibles y requieren máxima seguridad.  
**Solución:**  
- Usar **Snowball Edge con cifrado AES-256**.  
- Copiar los datos y enviarlos a AWS para almacenarlos en **Amazon S3 Glacier** (bajo costo).  
**Resultado:** Backup seguro y rápido, sin saturar la red del hospital.  

---  

#### **3. Recolección de Datos en Ubicaciones Remotas**  
**Situación:** Una empresa petrolera genera **50 TB** de datos diarios en plataformas marinas con **Internet satelital limitado**.  
**Problema:** No pueden enviar datos en tiempo real debido al alto costo y baja velocidad.  
**Solución:**  
- Usar **Snowball Edge** (con capacidad de computación) para:  
  - Almacenar datos localmente.  
  - Procesar información preliminar (ej: análisis de sensores).  
- Enviar el dispositivo periódicamente a AWS para cargar los datos procesados.  
**Resultado:** Reducción de costos de transferencia y análisis más rápido.  

---  

#### **4. Distribución de Contenido a Locales sin Conexión**  
**Situación:** Una productora de cine necesita enviar **80 TB** de material audiovisual a estudios de edición en zonas rurales sin banda ancha.  
**Problema:** No pueden usar servicios en la nube para compartir los archivos.  
**Solución:**  
- Cargar el contenido en un **Snowball**.  
- Enviarlo físicamente a los estudios, donde pueden copiar los datos a sus servidores locales.  
**Resultado:** Distribución segura y rápida sin depender de Internet.  

---  

### **¿Por qué Elegir Snowball en Estos Casos?**  
| Escenario | Alternativa (Internet) | Problema | Ventaja de Snowball |
|-----------|-----------------------|----------|---------------------|
| Migración de 500 TB | 1+ año de transferencia | Lento, costoso | **Completado en semanas** |  
| Backup de 200 TB | Congestión de red | Riesgo de interrupciones | **Sin afectar la red local** |  
| Datos en plataformas petroleras | Internet satelital (caro) | Latencia alta | **Procesamiento local + envío físico** |  
| Distribución de contenido | No viable sin Internet | - | **Entrega física segura** |  

---  

**Conclusión:**  
AWS Snowball es ideal cuando:  
- Tienes **más de 10 TB** que transferir.  
- Tu conexión a Internet es **lenta, inestable o cara**.  
- Necesitas **seguridad reforzada** (ej: datos médicos, financieros).  

