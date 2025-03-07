
**IAM** es un servicio de Amazon Web Services (AWS) que permite gestionar de forma segura el acceso a los recursos y servicios de AWS. Su función principal es controlar **quién (autenticación)** puede realizar **qué acciones (autorización)** sobre **qué recursos**, asegurando la seguridad de la cuenta de AWS.

---

## **Componentes principales de IAM**

1. **Usuarios**: Representan a personas o aplicaciones que interactúan con AWS. Cada usuario tiene credenciales únicas (como claves de acceso).
    
2. **Grupos**: Colecciones de usuarios a los que se asignan permisos de manera conjunta.
    
3. **Roles**: Identidades con permisos temporales que pueden ser asumidas por usuarios, servicios de AWS (como EC2) o cuentas externas.
    
4. **Políticas**: Documentos en formato **JSON** que definen permisos. Especifican qué acciones están permitidas o denegadas sobre recursos específicos (por ejemplo: "Permitir escritura en un bucket de S3").
    

---

## **Características clave de IAM**

- **Control centralizado**: Gestiona accesos para múltiples servicios y recursos desde un solo lugar.
    
- **Permisos granulares**: Define permisos detallados (por ejemplo, restringir acceso solo a un servidor EC2 específico).
    
- **Integración con servicios de AWS**: Funciona con todos los servicios de AWS (EC2, S3, Lambda, etc.).
    
- **Autenticación multifactor (MFA)**: Añade una capa extra de seguridad para el acceso.
    
- **Federación de identidades**: Permite a usuarios externos (como empleados de una empresa) acceder con credenciales existentes (ej: Microsoft Active Directory, Facebook, Google).
    

---

## **Beneficios de IAM**

- **Seguridad**: Aplica el principio de mínimo privilegio (solo los permisos necesarios).
    
- **Auditoría**: Registra actividades mediante AWS CloudTrail para cumplimiento normativo.
    
- **Sin costo adicional**: **IAM** es gratuito; solo se pagan los recursos utilizados.
    
- **Global**: No está asociado a una región específica de AWS.
    

---

## **Ejemplos de uso de IAM**

1. **Crear usuarios para equipos**: Un usuario para el equipo de desarrollo con acceso a EC2 y S3, y otro para finanzas con acceso solo a informes de costos.
    
2. **Roles para aplicaciones**: Un rol asignado a una instancia EC2 para que acceda a un bucket de S3 sin almacenar claves.
    
3. **Acceso temporal**: Otorgar permisos a un usuario externo por tiempo limitado.
    

---

**IAM** es esencial para garantizar que solo los usuarios y servicios autorizados tengan acceso a los recursos, reduciendo riesgos de seguridad en la nube.

# **Tipos de credenciales de seguridad en AWS**

En Amazon Web Services (AWS), las **credenciales de seguridad** son fundamentales para autenticar y autorizar el acceso a los recursos y servicios. A continuación, te detallo los principales tipos de credenciales de seguridad que ofrece AWS:

---

## **1. Credenciales de acceso (Access Keys)**
- **Descripción**: Compuestas por un **Access Key ID** y un **Secret Access Key**. Se utilizan para acceder a los servicios de AWS mediante programación (API, SDKs, CLI, etc.).
- **Uso común**: Acceso a servicios como S3, EC2, DynamoDB, etc., desde aplicaciones o scripts.
- **Ejemplo**:
  ```plaintext
  Access Key ID: AKIAIOSFODNN7EXAMPLE
  Secret Access Key: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
  ```
- **Importante**: Nunca compartas tu **Secret Access Key**, ya que es equivalente a una contraseña.

---

## **2. Contraseñas de usuario (IAM User Passwords)**
- **Descripción**: Contraseñas asignadas a usuarios de **IAM** para acceder a la consola de administración de AWS.
- **Uso común**: Acceso interactivo a la consola web de AWS.
- **Recomendación**: Activar la autenticación multifactor (MFA) para mayor seguridad.

---

## **3. Tokens de autenticación multifactor (MFA Tokens)**
- **Descripción**: Credenciales temporales generadas por dispositivos MFA (como Google Authenticator, Authy o dispositivos físicos como YubiKey).
- **Uso común**: Añadir una capa adicional de seguridad al iniciar sesión en la consola de AWS o realizar operaciones críticas.
- **Ejemplo**: Un código de 6 dígitos que cambia cada 30 segundos.

---

## **4. Tokens de seguridad temporales (Temporary Security Credentials)**
- **Descripción**: Credenciales de corta duración generadas mediante **AWS STS (Security Token Service)**. Incluyen un **Access Key ID**, un **Secret Access Key** y un **Token de seguridad**.
- **Uso común**: Acceso temporal a recursos para usuarios federados, roles de IAM o aplicaciones externas.
- **Ejemplo**: Usar roles de IAM para otorgar permisos temporales a una aplicación en EC2.

---

## **5. Certificados de clave pública (SSH Key Pairs)**
- **Descripción**: Par de claves (pública y privada) utilizadas para autenticarse en instancias de **Amazon EC2** mediante SSH.
- **Uso común**: Acceso seguro a servidores virtuales en la nube.
- **Ejemplo**: Conectar a una instancia EC2 Linux usando SSH con una clave privada.

---

## **6. Certificados SSL/TLS**
- **Descripción**: Certificados digitales utilizados para cifrar la comunicación entre clientes y servicios de AWS, como **CloudFront** o **Elastic Load Balancer (ELB)**.
- **Uso común**: Habilitar HTTPS en aplicaciones web o APIs.
- **Ejemplo**: Usar AWS Certificate Manager (ACM) para gestionar certificados SSL/TLS.

---

## **7. Credenciales de federación (Federated Credentials)**
- **Descripción**: Permiten a usuarios externos (por ejemplo, empleados de una empresa) acceder a AWS usando credenciales de sistemas de identidad externos (como Microsoft Active Directory, Google, Facebook, etc.).
- **Uso común**: Integración con proveedores de identidad (IdP) mediante **SAML** o **OpenID Connect**.
- **Ejemplo**: Usar AWS Single Sign-On (SSO) para acceder a múltiples cuentas de AWS.

---

## **8. Claves de API (API Keys)**
- **Descripción**: Credenciales utilizadas para acceder a servicios específicos como **Amazon API Gateway**.
- **Uso común**: Autenticar y controlar el acceso a APIs personalizadas.
- **Ejemplo**: Usar una clave de API para limitar el acceso a una API REST.

---

## **9. Credenciales de servicio (Service-Specific Credentials)**
- **Descripción**: Credenciales específicas para ciertos servicios de AWS, como **AWS CodeCommit** (repositorios Git).
- **Uso común**: Acceso a servicios que requieren autenticación específica.
- **Ejemplo**: Usar credenciales de Git para clonar un repositorio en CodeCommit.

---

## **10. Credenciales de root (Root User Credentials)**
- **Descripción**: Credenciales asociadas a la cuenta raíz de AWS (la primera cuenta creada al registrarse en AWS). Tienen acceso completo a todos los recursos y servicios.
- **Uso común**: Solo para tareas administrativas críticas (como gestionar la facturación o crear usuarios de IAM).
- **Recomendación**: No usar estas credenciales para operaciones diarias; en su lugar, crear usuarios de IAM con permisos limitados.

---

## **Resumen de credenciales clave**

| **Tipo de credencial**               | **Uso principal**                          |
|--------------------------------------|--------------------------------------------|
| Access Keys                          | Acceso programático a AWS                 |
| IAM User Passwords                   | Acceso a la consola de AWS                |
| MFA Tokens                           | Autenticación multifactor                 |
| Temporary Security Credentials       | Acceso temporal a recursos               |
| SSH Key Pairs                        | Conexión segura a instancias EC2          |
| SSL/TLS Certificates                 | Cifrado de comunicaciones HTTPS           |
| Federated Credentials                | Acceso mediante proveedores de identidad  |
| API Keys                             | Acceso a APIs personalizadas              |
| Service-Specific Credentials         | Acceso a servicios específicos            |
| Root User Credentials                | Tareas administrativas críticas           |

---

Estas credenciales son esenciales para garantizar la seguridad y el control de acceso en AWS. Siempre sigue las mejores prácticas, como rotar credenciales, usar MFA y aplicar el principio de mínimo privilegio.