---
title: "AWS Storage Gateway | Amazon Web Services"
source: "https://aws.amazon.com/es/storagegateway/"
author:
  - "[[Amazon Web Services]]"
  - "[[Inc.]]"
published:
created: 2025-03-25
description:
tags:
  - "clippings"
---
## AWS Storage Gateway

#### Ofrezca a las aplicaciones en las instalaciones acceso a almacenamiento prácticamente ilimitado en la nube

[Introducción a Storage Gateway](https://console.aws.amazon.com/storagegateway/)

## Beneficios

### Proporcione acceso a datos de baja latencia

### Proporcione acceso a las aplicaciones locales

### Ofrezca almacenamiento en la nube prácticamente ilimitado

### Respalde los esfuerzos en materia de conformidad con capacidades clave

## Tipos de Storage Gateway

AWS Storage Gateway ofrece a las aplicaciones un acceso local y en la nube a un almacenamiento en la nube prácticamente ilimitado. Puede desplegar Storage Gateway como una máquina virtual (VM) en el entorno virtual de VMware, Hyper-V o Linux KVM, o como una instancia de [Amazon EC2](https://aws.amazon.com/pm/ec2/?gclid=EAIaIQobChMItt2ik8SGhQMVImBHAR3dcAd0EAAYASAAEgK3AvD_BwE&trk=e9bd424b-2084-4b3a-bb58-3b2eee7e9c7b&sc_channel=ps&ef_id=EAIaIQobChMItt2ik8SGhQMVImBHAR3dcAd0EAAYASAAEgK3AvD_BwE:G:s&s_kwcid=AL!4422!3!651751061172!e!!g!!ec2%20host%20website!19852662368!145019212497) dentro de [Amazon Virtual Private Cloud](https://aws.amazon.com/vpc/) (Amazon VPC).

### Amazon S3 File Gateway

[S3 File Gateway](https://aws.amazon.com/storagegateway/file/s3/)  ofrece un acceso a los datos de [Amazon S3](https://aws.amazon.com/pm/serv-s3/?gclid=EAIaIQobChMImsWe2sSGhQMVh6JaBR0Z4wq-EAAYASAAEgJ1LPD_BwE&trk=20e04791-939c-4db9-8964-ee54c41bc6ad&sc_channel=ps&ef_id=EAIaIQobChMImsWe2sSGhQMVh6JaBR0Z4wq-EAAYASAAEgJ1LPD_BwE:G:s&s_kwcid=AL!4422!3!651751060962!e!!g!!amazon%20s3!19852662362!145019251177) basado en Server Message Block (SMB) o Network File System (NFS).

### Gateway de cinta

[Tape Gateway](https://aws.amazon.com/storagegateway/vtl/?nc=sn&loc=2&dn=3) presenta cintas virtuales para aplicaciones de respaldo que se pueden almacenar en [Amazon S3](https://aws.amazon.com/s3/)  o  [Amazon S3 Glacier](https://aws.amazon.com/pm/s3-glacier/?gclid=EAIaIQobChMIjJXUxMGIhQMVX6BaBR3G4QJvEAAYASAAEgL6tPD_BwE&trk=20e04791-939c-4db9-8964-ee54c41bc6ad&sc_channel=ps&ef_id=EAIaIQobChMIjJXUxMGIhQMVX6BaBR3G4QJvEAAYASAAEgL6tPD_BwE:G:s&s_kwcid=AL!4422!3!674509886391!e!!g!!amazon%20s3%20glacier!19852662362!154273573912).

### Gateway de volumen

[Volume Gateway](https://aws.amazon.com/storagegateway/volume/?nc=sn&loc=2&dn=4) presenta volúmenes de almacenamiento en bloque de iSCSI para las aplicaciones locales que se pueden almacenar en [Amazon S3](https://aws.amazon.com/s3/)  o migrar a  [Amazon EBS](https://aws.amazon.com/ebs/).

## S3 File Gateway ofrece acceso local a los archivos de los datos de Amazon S3

Con [S3 File Gateway](https://aws.amazon.com/storagegateway/file/s3/), puede crear flujos de trabajo de datos para alimentar el lago de datos, archivar datos inactivos, como las imágenes y los videos, y hacer copias de seguridad de bases de datos, como Microsoft SQL, Oracle y SAP; todo en S3.

## Tape Gateway virtualiza los flujos de trabajo de archivado y respaldo de cintas en AWS

[Tape Gateway](https://aws.amazon.com/storagegateway/vtl/) permite reemplazar cintas físicas locales por cintas virtuales en AWS, sin la necesidad de modificar los flujos de trabajo de respaldo existentes. Tape Gateway es compatible con las principales aplicaciones de copias de seguridad y almacena en caché cintas virtuales locales para ofrecer un acceso de baja latencia a los datos.

## Volume Gateway amplía la capacidad de almacenamiento en bloque local

Puede utilizar [Volume Gateway](https://aws.amazon.com/storagegateway/volume/?nc=sn&loc=2&dn=4) junto con servidores de Windows y Linux, de manera local, para proveer el almacenamiento de escala ajustable para las aplicaciones locales con opciones de recuperación en la nube. Con una arquitectura de volumen en caché, accede al beneficio de la protección de los datos y el almacenamiento en la nube de escala ajustable para los conjuntos de datos en crecimiento que necesitan acceso local de baja latencia para los datos que se utilizan con frecuencia.