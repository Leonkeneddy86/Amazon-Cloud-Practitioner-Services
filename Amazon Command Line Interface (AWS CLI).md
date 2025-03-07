# Amazon Command Line Interface (AWS CLI)

Es una herramienta oficial de AWS que permite interactuar con los servicios de AWS **desde la terminal o línea de comandos**, sin necesidad de usar la consola web. Está diseñada para automatizar tareas, gestionar recursos y ejecutar operaciones mediante scripts o comandos manuales.

---

## **¿Qué permite?**

1. **Automatización de tareas**  
   - Ejecutar operaciones repetitivas mediante scripts (Bash, PowerShell, etc.).  
   - Integrarse con herramientas de CI/CD (como Jenkins, GitHub Actions).  

2. **Acceso a todos los servicios de AWS**  
   - Gestionar EC2, S3, Lambda, IAM, DynamoDB y más.  
   - Ejemplo: Crear un bucket de S3:  
     ```bash
     aws s3 mb s3://nombre-bucket
     ```

3. **Multiplataforma**  
   - Funciona en Windows, macOS y Linux.  

4. **Personalización**  
   - Usar perfiles para gestionar múltiples cuentas de AWS.  
   - Configurar regiones, formatos de salida (JSON, texto, tabla).  

5. **Integración con otras herramientas**  
   - Compatible con AWS SAM, Terraform, CloudFormation, etc.  

---

## **Ventajas clave**  
- **Eficiencia**: Más rápido que la consola web para tareas masivas.  
- **Flexibilidad**: Ideal para DevOps y administradores de sistemas.  
- **Escalabilidad**: Gestiona cientos de recursos con pocos comandos.  

---

## **Ejemplo básico**  
Iniciar una instancia EC2:  

```
aws ec2 run-instances \
  --image-id ami-0abcdef1234567890 \
  --instance-type t2.micro \
  --key-name mi-key-pair \
```

## **Instalación y configuración**

### Instalación en Linux:

```
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"  
unzip awscliv2.zip  
sudo ./aws/install
```

### Configurar credenciales:

`aws configure`

- Se solicitará:
    
    - `AWS Access Key ID`
        
    - `AWS Secret Access Key`
        
    - `Region` (ej: `us-east-1`)
        
    - `Formato de salida` (ej: `json`)


	
