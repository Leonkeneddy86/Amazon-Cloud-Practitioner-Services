
---

### **¿Qué es una API?**
- **API** significa **Interfaz de Programación de Aplicaciones** (Application Programming Interface).
- Es un conjunto de reglas y protocolos que permite que dos aplicaciones se comuniquen entre sí.
- **Ejemplo**: Imagina que una API es como un "mesero" en un restaurante. Tú (el cliente) pides algo al mesero (la API), y él lleva tu pedido a la cocina (el servidor) y te trae la comida (la respuesta).

---

### **¿Para qué sirven las APIs?**
- **Integración**: Permiten que diferentes sistemas trabajen juntos.
- **Reutilización**: No necesitas reinventar la rueda, puedes usar APIs existentes.
- **Escalabilidad**: Facilita el crecimiento de aplicaciones al separar frontend y backend.
- **Ejemplo**: Cuando usas una app del clima, esta usa una API para obtener datos meteorológicos de un servidor.

---

### **: ¿Qué es REST?**
- **REST** significa **Transferencia de Estado Representacional** (Representational State Transfer).
- Es un estilo de arquitectura para diseñar APIs.
- Se basa en el protocolo **HTTP** (el mismo que usan los navegadores web).
- Usa verbos HTTP como **GET**, **POST**, **PUT**, **DELETE** para realizar acciones.

---

###  Características de REST**
1. **Sin estado (Stateless)**: Cada solicitud es independiente y contiene toda la información necesaria.
2. **Recursos**: Todo se trata de recursos (datos), identificados por URLs.
   - Ejemplo: `https://api.example.com/users`
3. **Formatos comunes**: Los datos se intercambian en formatos como JSON o XML.
4. **Operaciones CRUD**:
   - **GET**: Obtener datos.
   - **POST**: Crear datos.
   - **PUT**: Actualizar datos.
   - **DELETE**: Eliminar datos.

---

###  Ejemplo de una API REST**
- **URL**: `https://api.example.com/users`
- **Operaciones**:
  1. **GET** `/users` → Obtener lista de usuarios.
  2. **POST** `/users` → Crear un nuevo usuario.
  3. **GET** `/users/1` → Obtener detalles del usuario con ID 1.
  4. **PUT** `/users/1` → Actualizar el usuario con ID 1.
  5. **DELETE** `/users/1` → Eliminar el usuario con ID 1.

---

### **Beneficios de REST**
- **Simplicidad**: Fácil de entender y usar.
- **Escalabilidad**: Ideal para aplicaciones web y móviles.
- **Independencia**: Cliente y servidor pueden evolucionar por separado.
- **Compatibilidad**: Funciona con cualquier lenguaje de programación.

---

###  AWS y las APIs**
- **Amazon API Gateway**: Servicio de AWS para crear, publicar y gestionar APIs.
- **Integración**: Se conecta con otros servicios de AWS como Lambda, DynamoDB, etc.
- **Escalabilidad**: Maneja millones de solicitudes sin problemas.
- **Seguridad**: Ofrece autenticación y control de acceso.

---

### **Resumen**
- **API**: Es como un puente entre aplicaciones.
- **REST**: Es una forma popular de diseñar APIs usando HTTP.
- **AWS**: Ofrece herramientas como API Gateway para construir APIs escalables y seguras.

---

