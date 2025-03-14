---
title: "¿Qué es AWS Lambda? - AWS Lambda"
source: "https://docs.aws.amazon.com/es_es/lambda/latest/dg/welcome.html"
author:
published:
created: 2025-03-14
description: "Lambda es un servicio informático que puede utilizar para crear aplicaciones sin aprovisionar ni administrar servidores."
tags:
  - "clippings"
---
[RSS](https://docs.aws.amazon.com/es_es/lambda/latest/dg/lambda-updates.rss)

Modo de enfoque

¿Qué es AWS Lambda? - AWS Lambda

Puede utilizar AWS Lambda puede ejecutar código sin aprovisionar ni administrar servidores.

Lambda ejecuta el código en una infraestructura de computación de alta disponibilidad y realiza todas las tareas de administración de los recursos de computación, incluido el mantenimiento del servidor y del sistema operativo, el aprovisionamiento de capacidad y el escalado automático, así como las funciones de registro. Con Lambda, lo único que tiene que hacer es suministrar el código en uno de los tiempos de ejecución de lenguaje compatibles con Lambda.

Organice su código en Funciones de Lambda. El servicio de Lambda ejecuta la función solo cuando es necesario y escala automáticamente. Solo pagará por el tiempo informático que consuma; no se aplican cargos cuando el código no se está ejecutando. Para más información, consulte [Precios de AWS Lambda](https://aws.amazon.com/lambda/pricing/).

###### sugerencia

Para obtener información sobre cómo crear **soluciones sin servidor**, consulte la [Guía para desarrolladores sin servidor](https://docs.aws.amazon.com/serverless/latest/devguide/).

## Cuándo debe utilizar Lambda

Lambda es un servicio informático ideal para situaciones de aplicaciones que necesitan escalar verticalmente de forma rápida y reducir verticalmente a cero cuando no hay demanda. Por ejemplo, puede utilizar Lambda para los siguientes procesos:

- **Procesamiento de archivos:** utilice Amazon Simple Storage Service (Amazon S3) para iniciar el procesamiento de datos de Lambda en tiempo real después de la carga.
- **Procesamiento de flujos:** utilice Lambda y Amazon Kinesis para procesar datos de streaming en tiempo real en el seguimiento de la actividad de las aplicaciones, el procesamiento de pedidos de transacciones, el análisis de secuencias de clics, la limpieza de datos, el filtrado de registros, la indexación, el análisis de las redes sociales, la telemetría de datos de dispositivos de Internet de las cosas (IoT) y la medición de valores.
- **Aplicaciones web:** combine Lambda con otros servicios de AWS para crear aplicaciones web potentes que escalen verticalmente de manera automática y se ejecuten en una configuración de alta disponibilidad en varios centros de datos.
- **Backends de IoT:** cree backends sin servidor con Lambda para gestionar las solicitudes de API de Web, dispositivos móviles, IoT y terceros.
- **Backends móviles:** cree backends con Lambda y Amazon API Gateway para autenticar y procesar las solicitudes de API. Utilice AWS Amplify para integrar fácilmente a sus frontends de iOS, Android, Web y React Native.

Cuando se utiliza Lambda, solo es necesario preocuparse por el código. Lambda administra la flota de computación, que ofrece una combinación equilibrada de memoria, CPU, red y otros recursos para ejecutar su código. Como Lambda administra estos recursos, no puede iniciar sesión en instancias de informática ni personalizar el sistema operativo entiempos de ejecución proporcionados. Lambda realiza actividades operacionales y administrativas en su nombre, incluida la administración de la capacidad, la supervisión y el registro de las funciones de Lambda.

## Características principales

Las siguientes características clave lo ayudan a desarrollar aplicaciones escalables de Lambda, seguras y fácilmente extensibles:

**[Variables de entorno](https://docs.aws.amazon.com/es_es/lambda/latest/dg/configuration-envvars.html)**

Utilice variables de entorno para ajustar el comportamiento de la función sin actualizar el código.

**[Versiones](https://docs.aws.amazon.com/es_es/lambda/latest/dg/configuration-versions.html)**

Administre la implementación de las funciones con versiones, de modo que, por ejemplo, una nueva función pueda utilizarse para realizar pruebas beta sin que esto afecte a los usuarios de la versión de producción estable.

**[Imágenes de contenedor](https://docs.aws.amazon.com/es_es/lambda/latest/dg/images-create.html)**

Cree una imagen de contenedor para una función de Lambda mediante una imagen base proporcionada por AWS o una imagen base alternativa, de modo que pueda reutilizar las herramientas de contenedor existentes o implementar cargas de trabajo más grandes basadas en dependencias de tamaño modificable, como el machine learning.

**[Capas de Lambda](https://docs.aws.amazon.com/es_es/lambda/latest/dg/chapter-layers.html)**

Comprima bibliotecas y otras dependencias para reducir el tamaño de los archivos de implementación y acelerar la implementación del código.

**[Extensiones de Lambda](https://docs.aws.amazon.com/es_es/lambda/latest/dg/lambda-extensions.html)**

Aumente las funciones de Lambda con herramientas de supervisión, observabilidad, seguridad y gobernanza.

**[URL de funciones](https://docs.aws.amazon.com/es_es/lambda/latest/dg/urls-configuration.html)**

Agregue un punto de conexión HTTP(S) dedicado a la función de Lambda.

**[Transmisión de respuestas](https://docs.aws.amazon.com/es_es/lambda/latest/dg/configuration-response-streaming.html)**

Configure las URL de su función de Lambda para transmitir las cargas de respuesta a los clientes desde funciones de Node.js, mejorar el rendimiento del tiempo hasta el primer byte (TTFB) o devolver cargas más grandes.

**[Controles de concurrencia y escala](https://docs.aws.amazon.com/es_es/lambda/latest/dg/lambda-concurrency.html)**

Aplique un control detallado sobre el escalado y la capacidad de respuesta de las aplicaciones de producción.

**[Firma de código](https://docs.aws.amazon.com/es_es/lambda/latest/dg/configuration-codesigning.html)**

Compruebe que solo los desarrolladores aprobados publiquen código de confianza e inalterado en sus funciones de Lambda

**[Red privada](https://docs.aws.amazon.com/es_es/lambda/latest/dg/configuration-vpc.html)**

Cree una red privada para recursos como bases de datos, instancias de caché o servicios internos.

**[Sistema de archivos](https://docs.aws.amazon.com/es_es/lambda/latest/dg/configuration-filesystem.html)**

Configure una función para montar Amazon Elastic File System (Amazon EFS) en un directorio local, de modo que el código de función pueda acceder y modificar los recursos compartidos de forma segura y en alta concurrencia.

**[Lambda SnapStart](https://docs.aws.amazon.com/es_es/lambda/latest/dg/snapstart.html)**

Lambda SnapStart puede ofrecer un rendimiento de inicio en menos de un segundo, normalmente sin cambios en el código de la función.

### En esta página

### Related resources

[Referencia de la API de AWS Lambda](https://docs.aws.amazon.com/lambda/latest/api/welcome.html)

[Comandos de la AWS CLI de AWS Lambda](https://docs.aws.amazon.com/cli/latest/reference/lambda/)

[Herramientas y SDK](https://aws.amazon.com/tools/)

[Enviar comentarios](https://docs.aws.amazon.com/forms/aws-doc-feedback?hidden_service_name=Lambda&topic_url=https://docs.aws.amazon.com/es_es/lambda/latest/dg/welcome.html)

### Related resources

[Referencia de la API de AWS Lambda](https://docs.aws.amazon.com/lambda/latest/api/welcome.html)

[Comandos de la AWS CLI de AWS Lambda](https://docs.aws.amazon.com/cli/latest/reference/lambda/)

[Herramientas y SDK](https://aws.amazon.com/tools/)

#### Tema siguiente:

[Creación de su primera función](https://docs.aws.amazon.com/es_es/lambda/latest/dg/getting-started.html)

#### ¿Necesita ayuda?

- [Probar AWS re:Post](https://repost.aws/es/tags/TA5uNafDy2TpGNjidWLMSxDw)
- [Contacte con un experto de AWS IQ](https://iq.aws.amazon.com/get-started/?utm=docs&service=AWS%20Lambda)