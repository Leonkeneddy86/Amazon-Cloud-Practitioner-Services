 ### Aprenderá a: 

- Explicar el propósito y la función de los contenedores y los servicios de AWS que admiten el uso de contenedores.
- Describir los contenedores y sus beneficios.
- Describir Docker y examinar una implementación de Docker.
- Comparar y correlacionar diferentes servicios de contenedores en AWS.
- Diferenciar Kubernetes y Amazon Elastic Kubernetes Service (Amazon EKS).
- Identificar los desafíos de la administración de contenedores y AWS Fargate.

## Términos clave:

- Contenedores
- Docker
- Expansión de contenedores
- Contenedores zombis
- Contenedor de Amazon Elastic Container Service (Amazon ECS)
- AWS Fargate
- Clúster
- Kubernetes
- Amazon Elastic Kubernetes Service (Amazon EKS)
- Amazon Elastic Container Registry (Amazon ECR)

## Que es un contenedor?

- Un método de virtualización del sistema operativo (SO)
- Una aplicación y sus dependencias, que se pueden ejecutar en procesos aislados de recursos

---

**¿Qué es Docker?**

- **Definición**: Docker es una plataforma de código abierto que permite desarrollar, desplegar y ejecutar aplicaciones en contenedores.
- **Contenedores**: Los contenedores son unidades ligeras y portátiles que encapsulan una aplicación y todas sus dependencias (bibliotecas, frameworks, configuraciones, etc.).
- **Aislamiento**: Cada contenedor se ejecuta de manera aislada, lo que garantiza que la aplicación funcione de manera consistente en diferentes entornos (desarrollo, pruebas, producción).

---

**Beneficios de Docker**

1. **Portabilidad**: Las aplicaciones empaquetadas en contenedores pueden ejecutarse en cualquier sistema que soporte Docker, sin importar el entorno subyacente.
2. **Eficiencia**: Los contenedores comparten el kernel del sistema operativo, lo que los hace más ligeros y rápidos que las máquinas virtuales (VMs).
3. **Escalabilidad**: Facilita la escalabilidad horizontal, ya que puedes ejecutar múltiples instancias de un contenedor en paralelo.
4. **Consistencia**: Elimina el problema de "funciona en mi máquina" al garantizar que el entorno de ejecución sea el mismo en todas las etapas del ciclo de vida del software.

---

**¿Cómo se relaciona con AWS?**

- **Integración con AWS**: Docker se integra perfectamente con servicios de AWS como:
  - **Amazon ECS (Elastic Container Service)**: Un servicio de orquestación de contenedores totalmente gestionado.
  - **Amazon EKS (Elastic Kubernetes Service)**: Para gestionar aplicaciones en contenedores usando Kubernetes.
  - **AWS Fargate**: Permite ejecutar contenedores sin necesidad de gestionar servidores subyacentes.
- **Despliegue en la nube**: Docker facilita el despliegue de aplicaciones en la infraestructura de AWS, permitiendo una transición fluida entre entornos locales y la nube.

---

**Casos de uso comunes**

1. **Microservicios**: Docker es ideal para arquitecturas basadas en microservicios, donde cada servicio puede ejecutarse en su propio contenedor.
2. **CI/CD (Integración Continua/Despliegue Continuo)**: Facilita la automatización de pipelines de desarrollo y despliegue.
3. **Pruebas y desarrollo**: Permite a los desarrolladores trabajar en entornos aislados y consistentes.

---
**Amazon Elastic Container Registry (Amazon ECR)**  
*Almacenamiento seguro y escalable para imágenes de contenedores*

---

**¿Qué es Amazon ECR?**  
- **Registro de contenedores Docker totalmente administrado** por AWS.  
- Permite **almacenar, gestionar y desplegar imágenes de contenedores** de forma segura.  
- Integrado con servicios AWS como **Amazon ECS, EKS y AWS Fargate**.  

---

**Características clave**  
🔒 **Seguridad**:  
- Cifrado automático de imágenes (**en tránsito y en reposo**).  
- Control de acceso con **AWS IAM** y políticas de repositorio.  

🚀 **Escalabilidad y rendimiento**:  
- Alta disponibilidad y durabilidad con infraestructura global de AWS.  
- Compatible con **Docker CLI** y herramientas estándar.  

🛠 **Integración nativa**:  
- **Amazon ECS/EKS**: Despliega imágenes directamente en clústeres.  
- **AWS CI/CD**: Integración con **AWS CodePipeline, CodeBuild y CodeDeploy**.  

---

**Beneficios principales**  
✅ **Privado y seguro**: Repositorios privados con políticas granulares.  
✅ **Eficiencia**: Almacenamiento en capas para imágenes optimizadas.  
✅ **Escaneo de vulnerabilidades**: Identifica riesgos en imágenes con **Amazon ECR Image Scanning**.  

---

**Casos de uso comunes**  
1. **Microservicios**: Almacena imágenes para arquitecturas modernas.  
2. **CI/CD**: Automatiza despliegues en pipelines de integración continua.  
3. **Colaboración segura**: Comparte imágenes entre equipos o cuentas AWS.  

---

**¿Cómo empezar?**  
1. **Crea un repositorio** en AWS Management Console o CLI.  
2. **Sube imágenes** con `docker push` autenticado mediante AWS IAM.  
3. **Despliega** en ECS, EKS o Fargate con solo referenciar la URI de la imagen.  


---

### **¿Qué es Kubernetes?**  
**Plataforma de orquestación de contenedores**  
(Open Source, diseñado por Google, mantenido por la CNCF)  

---

#### **Problema que resuelve**  
🚨 **Complejidad en entornos modernos:**  
- Escalar aplicaciones en contenedores (Docker, etc.).  
- Gestionar fallos, actualizaciones y recursos en clusters.  
- Balancear tráfico y descubrir servicios automáticamente.  

---

#### **Características clave**  
✅ **Automatización:**  
- **Despliegues:** Rollouts y rollbacks controlados.  
- **Escalado:** Ajusta recursos en tiempo real (Horizontal Pod Autoscaler).  
- **Auto-reparación:** Reinicia contenedores fallidos o reemplaza nodos.  

🔗 **Service Discovery & Load Balancing:**  
- Asigna direcciones IP únicas y balancea carga entre pods.  

📦 **Gestión de almacenamiento:**  
- Monta sistemas de almacenamiento (AWS EBS, S3, etc.).  

---

#### **Arquitectura básica**  
🏗️ **Cluster = Nodos (workers) + Plano de control (control plane)**  
- **Nodos:** Ejecutan los pods (contenedores).  
- **Control Plane:**  
  - **kube-apiserver:** Punto de entrada para gestionar el cluster.  
  - **kube-scheduler:** Asigna pods a nodos.  
  - **kube-controller-manager:** Monitorea el estado del cluster.  
  - **etcd:** Base de datos clave-valor para almacenar estados.  

---

#### **AWS + Kubernetes**  
🛠️ **Amazon EKS (Elastic Kubernetes Service):**  
- Servicio gestionado de Kubernetes en AWS.  
- Integra IAM, VPC, CloudWatch y Load Balancers.  
- Elimina la necesidad de gestionar el plano de control.  

---

#### **Beneficios**  
🚀 **Portabilidad:**  
- Ejecuta la misma app en cualquier nube (híbrida/multicloud).  

📈 **Escalabilidad:**  
- De 1 a miles de nodos con comandos o APIs.  

🛡️ **Resiliencia:**  
- Tolerancia a fallos y alta disponibilidad.  

🔧 **Ecosistema:**  
- Herramientas como Helm, Prometheus, Istio, etc.  

---

#### **Casos de uso comunes**  
1. **Microservicios:** Coordina cientos de servicios en contenedores.  
2. **Machine Learning:** Escala workloads de entrenamiento/inferencia.  
3. **CI/CD:** Actualiza apps sin downtime (blue-green deployments).  

---

**Resumen:** Kubernetes es el estándar para orquestar contenedores, y AWS lo simplifica con EKS.  

---

**Amazon Fargate**  
*Servicio de Computación Serverless para Contenedores*  

---

**¿Qué es Amazon Fargate?**  
- **Motor de computación serverless** para contenedores.  
- Integrado con **Amazon ECS** y **Amazon EKS**.  
- Elimina la necesidad de administrar servidores o clusters.  
- **Enfoque en la aplicación**, no en la infraestructura.  

---

**Comparación: Fargate vs. EC2 tradicional**  
| **Fargate**                          | **EC2 tradicional**                |  
|--------------------------------------|-------------------------------------|  
| Sin gestión de servidores            | Administrar instancias EC2          |  
| Pago por uso (vCPU/memoria)          | Pago por instancias reservadas      |  
| Escalado automático integrado        | Configurar Auto Scaling manualmente |  
| Aislamiento de tareas/containers     | Compartir recursos del servidor     |  

---

**Beneficios Clave**  
✅ **Operaciones simplificadas**  
- Sin aprovisionar, parchear o escalar servidores.  
- Gestión centralizada con ECS/EKS.  

✅ **Seguridad mejorada**  
- Cada tarea/Pod se ejecuta en un entorno aislado.  

✅ **Integración con AWS**  
- Compatible con IAM, VPC, CloudWatch, ALB/NLB.  

✅ **Costos optimizados**  
- Pagas solo por los recursos que consumes.  

---

**Casos de Uso Comunes**  
- **Aplicaciones web/microservicios**: Escalado ágil sin gestión de servidores.  
- **Procesamiento de datos batch**: Ejecución de tareas efímeras.  
- **Entornos CI/CD**: Integración con CodePipeline, GitHub Actions, etc.  
- **Machine Learning**: Despliegue de modelos en contenedores.  

---

**Modelo de Precios**  
- **Por tarea/Pod**:  
  - **vCPU**: Costo por hora según GB asignados.  
  - **Memoria**: Costo por hora según GB usados.  
- **Sin costos adicionales** por clusters o instancias.  

---

**Resumen**  
- **Serverless para contenedores**: Ideal para equipos que priorizan la agilidad.  
- **Reducción de carga operativa**: AWS gestiona la infraestructura.  
- **Pago por uso**: Costos alineados con la demanda real.  

✨ **Enfócate en tu código, no en servidores.** ✨  

--- 
