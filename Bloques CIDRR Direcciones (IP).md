

---

### **¿Qué es CIDR?**
CIDR es una forma de representar rangos de direcciones IP. En AWS, se usa para definir redes y subredes dentro de una VPC (Virtual Private Cloud). Es como decir: "Este es el grupo de direcciones IP que voy a usar en mi red".

---

### **Partes de un bloque CIDR**
Un bloque CIDR tiene dos partes:
1. **Dirección IP base**: Es la primera dirección del rango.
2. **Máscara de subred**: Indica cuántas direcciones IP hay en ese rango.

Se escribe así: `10.0.0.0/16`

- **10.0.0.0**: Es la dirección IP base.
- **/16**: Es la máscara de subred. Indica que los primeros 16 bits de la dirección IP están fijos, y los restantes pueden variar.

---

### **¿Cómo se calcula el tamaño de un bloque CIDR?**
La máscara de subred (`/16`, `/24`, etc.) determina cuántas direcciones IP hay en el bloque. Cuanto más pequeño sea el número después de la "/", más grande será el rango de direcciones IP.

#### Fórmula:
- **Número de direcciones IP** = 2^(32 - máscara de subred).

#### Ejemplos:
1. **10.0.0.0/16**:
   - Máscara: `/16`.
   - Número de direcciones IP: 2^(32 - 16) = 2^16 = **65,536 direcciones IP**.
   - Rango: Desde `10.0.0.0` hasta `10.0.255.255`.

2. **192.168.1.0/24**:
   - Máscara: `/24`.
   - Número de direcciones IP: 2^(32 - 24) = 2^8 = **256 direcciones IP**.
   - Rango: Desde `192.168.1.0` hasta `192.168.1.255`.

3. **172.16.0.0/20**:
   - Máscara: `/20`.
   - Número de direcciones IP: 2^(32 - 20) = 2^12 = **4,096 direcciones IP**.
   - Rango: Desde `172.16.0.0` hasta `172.16.15.255`.

---

### **¿Por qué es importante en AWS?**
En AWS, cuando creas una VPC, debes asignarle un bloque CIDR. Este bloque define el rango de direcciones IP que puedes usar dentro de esa VPC. Luego, puedes dividir ese bloque en subredes más pequeñas (subnets) para organizar tus recursos.

---

### **Ejemplo práctico en AWS**
Imagina que estás creando una VPC para una aplicación web.

1. **Crear una VPC**:
   - Asignas un bloque CIDR: `10.0.0.0/16`.
   - Esto te da un rango de direcciones IP desde `10.0.0.0` hasta `10.0.255.255` (65,536 direcciones IP).

2. **Crear subredes dentro de la VPC**:
   - **Subred pública**: `10.0.1.0/24` (256 direcciones IP, desde `10.0.1.0` hasta `10.0.1.255`).
   - **Subred privada**: `10.0.2.0/24` (256 direcciones IP, desde `10.0.2.0` hasta `10.0.2.255`).

3. **Asignar recursos**:
   - Puedes lanzar una instancia EC2 en la subred pública con la dirección IP `10.0.1.10`.
   - Puedes lanzar una base de datos RDS en la subred privada con la dirección IP `10.0.2.20`.

---

### **Reglas importantes en AWS**
1. **Tamaño mínimo de bloque CIDR para una VPC**: `/28` (16 direcciones IP).
2. **Tamaño máximo de bloque CIDR para una VPC**: `/16` (65,536 direcciones IP).
3. **Los bloques CIDR no pueden superponerse**: Si tienes una VPC con el bloque `10.0.0.0/16`, no puedes crear otra VPC con `10.0.1.0/24` porque se superponen.

---

### **Ejercicio práctico**
1. **Calcula el número de direcciones IP**:
   - Bloque CIDR: `192.168.0.0/26`.
   - Máscara: `/26`.
   - Número de direcciones IP: 2^(32 - 26) = 2^6 = **64 direcciones IP**.
   - Rango: Desde `192.168.0.0` hasta `192.168.0.63`.

2. **Divide un bloque CIDR en subredes**:
   - Bloque CIDR: `10.0.0.0/16`.
   - Quieres crear subredes de tamaño `/24`.
   - Cada subred tendrá 256 direcciones IP.
   - Puedes crear 256 subredes (porque 65,536 / 256 = 256).

---

### **Resumen**
- **CIDR** es una forma de definir rangos de direcciones IP.
- En AWS, se usa para crear VPCs y subredes.
- La máscara de subred (`/16`, `/24`, etc.) determina cuántas direcciones IP hay en el bloque.
- Ejemplo: `10.0.0.0/16` te da un rango grande, mientras que `10.0.0.0/24` te da un rango más pequeño.
