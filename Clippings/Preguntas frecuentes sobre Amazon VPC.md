---
title: "Preguntas frecuentes sobre Amazon VPC"
source: "https://aws.amazon.com/es/vpc/faqs/"
author:
  - "[[Amazon Web Services]]"
  - "[[Inc.]]"
published:
created: 2025-03-17
description:
tags:
  - "clippings"
---
## Temas de la página

[Preguntas generales

5

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#general-questions)[Facturación

2

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#billing)[Conectividad

9

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#connectivity)[Direccionamiento IP

16

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#ip-addressing)[Bring Your Own IP

10

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#bring-your-own-ip)[IP Address Manager

8

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#ip-address-manager)[Topología

1

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#topology)[Seguridad y filtros

12

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#security-filtering)[Replicación de tráfico de VPC

4

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#vpc-traffic-mirroring)[Amazon VPC y EC2

18

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#amazon-vpc-ec2)[VPC predeterminadas

17

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#default-vpcs)[EC2 Classic

6

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#ec2-classic)[Interfaces de redes elásticas

5

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#elastic-network-interfaces)[Interconexiones

14

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#peering-connections)[ClassicLink

10

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#classiclink)[AWS PrivateLink

4

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#aws-privatelink)[Preguntas adicionales

4

](https://aws.amazon.com/es/vpc/faqs/#product-faqs#vpc-faqs#additional-questions)

## Preguntas generales

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Qué es Amazon Virtual Private Cloud?

### ¿Cuáles son los componentes de Amazon VPC?

### ¿Por qué debería utilizar Amazon VPC?

### ¿Cómo comienzo a utilizar Amazon VPC?

### ¿Cuáles son los diferentes tipos de puntos de conexión de VPC disponibles en Amazon VPC?

## Facturación

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Cómo se cobra y factura el uso de Amazon VPC?

### ¿En qué cargos por uso incurriré si utilizo otros servicios de AWS, como Amazon S3, desde las instancias de Amazon EC2 en mi VPC?

## Conectividad

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Qué opciones de conectividad existen para mi Amazon VPC?

### ¿Cómo puedo conectar mi VPC a Internet?

### ¿Hay limitaciones de ancho de banda para las gateways de Internet? ¿Tengo que preocuparme por la disponibilidad? ¿Puede tratarse de un punto único de error?

### ¿Cómo obtienen acceso a Internet las instancias de una VPC?

### ¿Cuándo se considera una dirección IP como una dirección IP pública?

### ¿Cómo obtienen acceso a Internet las instancias sin direcciones IP públicas?

### ¿Puedo conectarme a mi VPC por medio de una VPN por software?

### ¿El tráfico pasa por Internet cuando dos instancias se comunican mediante direcciones IP públicas, o cuando las instancias se comunican con un punto de conexión del servicio público de AWS?

### ¿Cómo funciona una conexión de AWS Site-to-Site VPN con Amazon VPC?

## Direccionamiento IP

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Qué rangos de direcciones IP puedo utilizar en mi Amazon VPC?

### ¿Cómo puedo asignar rangos de direcciones IP a las Amazon VPC?

### ¿Qué rangos de direcciones IP se asignan a una Amazon VPC predeterminada?

### ¿Puedo usar las direcciones IP en VPC y acceder a ellas a través de Internet?

### ¿Qué tamaño máximo puede tener la VPC creada?

### ¿Puedo modificar el tamaño de una VPC?

### ¿Cuántas subredes puedo crear por VPC?

### ¿Existe un tamaño mínimo o máximo para las subredes?

### ¿Puedo utilizar todas las direcciones IP que asigne a una subred?

### ¿Cómo puedo asignar direcciones IP privadas a instancias de Amazon EC2 en una VPC?

### ¿Puedo cambiar las direcciones IP privadas de una instancia de Amazon EC2 mientras se está ejecutando o cuando se detiene en una VPC?

### Si se detiene una instancia de Amazon EC2 en una VPC, ¿puedo lanzar otra instancia con la misma dirección IP en la misma VPC?

### ¿Puedo asignar direcciones IP para varias instancias de forma simultánea?

### ¿Puedo asignar cualquier dirección IP a una instancia?

### ¿Puedo asignar varias direcciones IP a una instancia?

### ¿Puedo asignar una o varias direcciones IP elásticas (EIP) a instancias de Amazon EC2 basadas en una VPC?

## Bring Your Own IP

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿En qué consiste la característica Bring Your Own IP?

### ¿Por qué debería utilizar BYOIP?

### ¿Qué sucede si lanzo una IP elástica de BYOIP?

### ¿En qué regiones de AWS se encuentra disponible BYOIP?

### ¿Es posible compartir un prefijo de BYOIP con varias VPC en la misma cuenta?

### ¿Cuántos rangos IP puedo incorporar a través de BYOIP?

### ¿Cuál es el prefijo más específico que puedo incorporar a través de BYOIP?

### ¿Qué prefijos de RIR puedo usar para BYOIP?

### ¿Puedo incorporar un prefijo reasignado o redistribuido?

### ¿Puedo mover un prefijo BYOIP de una región de AWS a otra?

## IP Address Manager

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Qué es el Administrador de direcciones IP (IPAM)?

### ¿Por qué debería utilizar IPAM?

### ¿Cuáles son las características clave que ofrece IPAM?

### ¿Cuáles son los componentes clave de IPAM?

### ¿Es IPAM compatible con uso de su propia IP (BYOIP)?

### ¿Amazon proporciona bloques de CIDR contiguos y cómo funcionan con IPAM?

### ¿Se pueden utilizar bloques de CIDR IPv6 contiguos proporcionados por Amazon sin IPAM?

### ¿Puedo compartir mis grupos de IPAM con otras cuentas?

## Topología

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Puedo especificar qué puerta de enlace utilizará cada subred de forma predeterminada?

## Seguridad y filtros

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Cómo puedo proteger las instancias de Amazon EC2 que se ejecutan en mi VPC?

### ¿Qué diferencias existen entre los grupos de seguridad que están en una VPC y las ACL de red de una VPC?

### ¿Qué diferencia existe entre los filtros con estado (stateful) y sin estado (stateless)?

### ¿Pueden las instancias de Amazon EC2 de una VPC comunicarse con las instancias de Amazon EC2 que no están en una VPC?

### ¿Las instancias de Amazon EC2 que están en la VPC de una región pueden comunicarse con las instancias de Amazon EC2 que están en una VPC de otra región?

### ¿Pueden comunicarse con Amazon S3 las instancias de Amazon EC2 dentro de una VPC?

### ¿Puedo supervisar el tráfico de red de mi VPC?

### ¿Qué son los registros de flujo de Amazon VPC?

### ¿Cómo puedo utilizar los registros de flujo de la VPC?

### ¿Los registros de flujo de VPC son compatibles con AWS Transit Gateway?

### El uso de los registros de flujo afecta a la latencia o al rendimiento de mi red?

### ¿Cuánto cuestan los registros de flujo de la VPC?

## Replicación de tráfico de VPC

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Qué es la Creación de reflejo de tráfico de Amazon VPC?

### ¿Qué recursos se pueden supervisar con la Creación de reflejo de tráfico de Amazon VPC?

### ¿Qué tipos de dispositivos se admiten en la Creación de reflejo de tráfico de Amazon VPC?

### ¿Qué diferencias existen entre la Creación de reflejo de tráfico de Amazon VPC y los registros de flujos de Amazon VPC?

## Amazon VPC y EC2

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿En qué regiones de Amazon EC2 está disponible Amazon VPC?

### ¿Una VPC puede abarcar varias zonas de disponibilidad?

### ¿Una subred puede abarcar varias zonas de disponibilidad?

### ¿Cómo puedo especificar en qué zona de disponibilidad se lanzarán las instancias de Amazon EC2?

### ¿Cómo determino en qué zonas de disponibilidad están ubicadas las subredes?

### ¿Se me factura el ancho de banda de la red entre instancias situadas en subredes diferentes?

### Cuando llamo a DescribeInstances(), ¿puedo ver todas las instancias de Amazon EC2, incluidas las instancias EC2-Classic y EC2-VPC?

### Cuando llamo a DescribeVolumes(), ¿puedo ver todos los volúmenes de Amazon EBS, incluidos los volúmenes EC2-Classic y EC2-VPC?

### ¿Cuántas instancias de Amazon EC2 puedo utilizar en una VPC?

### ¿Puedo utilizar mis AMI existentes en Amazon VPC?

### ¿Puedo utilizar mis instantáneas existentes de Amazon EBS?

### ¿Puedo iniciar una instancia de Amazon EC2 desde un volumen de Amazon EBS en Amazon VPC?

### ¿Puedo utilizar Amazon CloudWatch en Amazon VPC?

### ¿Puedo utilizar Auto Scaling en Amazon VPC?

### ¿Puedo lanzar instancias en clúster de Amazon EC2 en una VPC?

### ¿Qué son los nombres de host de las instancias?

### ¿Puedo cambiar el nombre de host de la instancia de Amazon EC2?

### ¿Puedo usar los nombres de host de la instancia como nombres de host DNS?

## VPC predeterminadas

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Qué es una VPC predeterminada?

### ¿Qué beneficios ofrece una VPC predeterminada?

### ¿Qué cuentas admiten una VPC predeterminada?

### ¿Necesito saber algo sobre Amazon VPC para utilizar una VPC predeterminada?

### ¿En qué difieren las instancias lanzadas en EC2-Classic de las instancias lanzadas en EC2-VPC?

### ¿Necesito una conexión de VPN para utilizar una VPC predeterminada?

### Además de la VPC predeterminada, ¿puedo crear otras VPC y utilizarlas?

### ¿Puedo crear subredes adicionales en mi VPC predeterminada, por ejemplo, subredes privadas?

### ¿Cuántas VPC predeterminadas puedo tener?

### ¿Cuántas subredes predeterminadas hay en una VPC predeterminada?

### ¿Puedo especificar qué VPC es mi VPC predeterminada?

### ¿Puedo especificar qué subredes son mis subredes predeterminadas?

### ¿Puedo borrar una VPC predeterminada?

### ¿Puedo borrar una subred predeterminada?

### Tengo una cuenta EC2-Classic. ¿Puedo obtener una VPC predeterminada?

### Deseo disponer de una VPC predeterminada para mi cuenta de EC2. ¿Es posible?

### ¿Cuál es el impacto de la VPC predeterminada en las cuentas de IAM?

## EC2 Classic

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Qué es EC2-Classic?

### ¿Qué va a cambiar?

### ¿Cómo repercute en mi cuenta la retirada de EC2-Classic?

### ¿Cuáles son los beneficios de pasar de EC2-Classic a Amazon VPC?

### ¿Cómo se migra de EC2-Classic a VPC?

### ¿Cuáles son las fechas importantes que debo tener en cuenta?

## Interfaces de redes elásticas

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Puedo conectar o desconectar una o varias interfaces de red a una instancia EC2 mientras esta se encuentra en ejecución?

### ¿Puedo conectar una interfaz de red de una zona de disponibilidad a una instancia ubicada en otra zona de disponibilidad?

### ¿Puedo conectar una interfaz de red de una VPC a una instancia de otra VPC?

### ¿Puedo usar interfaces de redes elásticas como forma de alojar varios sitios web que requieran direcciones IP separadas en una sola instancia?

### ¿Puedo desconectar la interfaz principal (eth0) de mi instancia EC2?

## Interconexiones

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Puedo crear una interconexión con una VPC en una región diferente?

### ¿Puedo interconectar mi VPC con una VPC que pertenezca a otra cuenta de AWS?

### ¿Cuánto cuestan la conexión de emparejamiento de VPC?

### ¿Necesito una puerta de enlace de Internet para utilizar las interconexiones?

### ¿Se cifra el tráfico de las interconexiones de VPC dentro de la región?

### Si elimino mi extremo de una interconexión, ¿el otro extremo aún tendrá acceso a mi VPC?

### Si interconecto la VPC A a la VPC B y, al mismo tiempo, interconecto la VPC B a la VPC C, ¿significa que las VPC A y C están interconectadas?

### ¿Qué sucede si mi interconexión deja de funcionar?

### ¿Hay limitaciones de ancho de banda para las interconexiones?

### ¿El tráfico de la interconexión de VPC entre regiones está cifrado?

### ¿Cómo funcionan las traducciones de DNS con las interconexiones de VPC entre regiones?

### ¿Puedo hacer referencia a grupos de seguridad en una conexión de emparejamiento de VPC entre regiones?

### ¿El emparejamiento de VPC entre regiones es compatible con IPv6?

### ¿La interconexión de VPC entre regiones se puede usar con EC2-Classic Link?

## ClassicLink

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Qué es ClassicLink?

### ¿Cuál es el costo de ClassicLink?

### ¿Cómo se utiliza ClassicLink?

### ¿La instancia EC2-Classic se convierte en miembro de la VPC?

### ¿Puedo utilizar nombres de host de DNS públicos de EC2 desde mis instancias EC2-Classic e instancias EC2-VPC para comunicarse entre sí, a fin de efectuar la comunicación mediante una IP privada?

### ¿Existe alguna VPC para la que no se pueda activar ClassicLink?

### ¿El tráfico proveniente de una instancia EC2-Classic puede recorrer Amazon VPC y salir por la puerta de enlace de Internet, la puerta de enlace privada virtual o hacia VPC interconectadas?

### ¿ClassicLink afecta el control de acceso entre la instancia EC2-Classic y otras instancias que están en la plataforma EC2-Classic?

### ¿Se conservarán los ajustes de ClassicLink en mi instancia EC2-Classic durante los ciclos de parada/inicio?

### ¿ClassicLink permite que las reglas de grupos de seguridad EC2-Classic hagan referencia a grupos de seguridad de VPC, o viceversa?

## AWS PrivateLink

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)

### ¿Qué es AWS PrivateLink?

### ¿Cómo puedo usar AWS PrivateLink?

### ¿Cuáles son los servicios disponibles actualmente en AWS PrivateLink?

### ¿Es posible obtener acceso de manera privada a los servicios con tecnología de AWS PrivateLink a través de AWS Direct Connect?

## Preguntas adicionales

[Abrir todo](https://aws.amazon.com/es/vpc/faqs/#)