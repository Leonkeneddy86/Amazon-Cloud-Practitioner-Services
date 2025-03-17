---
title: "Cloud Database Migration - Características de AWS Database Migration Service (AWS DMS) - AWS"
source: "https://aws.amazon.com/es/dms/features/"
author:
  - "[[Amazon Web Services]]"
  - "[[Inc.]]"
published:
created: 2025-03-17
description: "AWS Database Migration Service (AWS DMS) le permite migrar las bases de datos a AWS de manera rápida y segura. AWS DMS le ofrece la capacidad de planificar, evaluar, convertir y migrar las bases de datos y los sistemas de análisis a escala bajo un servicio central, ahorrando tiempo, recursos y costos."
tags:
  - "clippings"
---
## Características de AWS Database Migration Service

## Información general

[AWS Database Migration Service](https://aws.amazon.com/dms/) (AWS DMS) le ayuda a migrar de forma rápida y segura [las bases de datos](https://aws.amazon.com/products/databases/migrations/) y [los almacenes de datos](https://aws.amazon.com/redshift/) a AWS con un tiempo de inactividad mínimo y sin pérdida de datos. AWS DMS le ofrece la capacidad de planificar, evaluar, convertir y migrar las bases de datos y los sistemas de análisis a escala bajo un servicio central, ahorrando tiempo, recursos y costes. La [base de datos de origen](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Introduction.Sources.html) permanece totalmente operativa durante la migración, minimizando así el tiempo de inactividad de las aplicaciones que dependen de ella. AWS DMS puede gestionar incluso las migraciones más complejas, incluida la migración simultánea de decenas o incluso cientos de cargas de trabajo.

AWS DMS puede migrar datos hacia y desde la mayoría de las [bases de datos de código abierto](https://aws.amazon.com/products/databases/open-source-databases/) y comerciales de uso general. La base de datos de origen puede estar ubicada en sus propias instalaciones fuera de AWS, en una base de datos autogestionada que se ejecute en una instancia de Amazon Elastic Compute Cloud (Amazon EC2), en una base de datos de Amazon totalmente gestionada o en un servicio de base de datos de terceros. La base de datos de destino puede ser una base de datos autogestionada que se ejecute en una instancia de Amazon EC2 o una base de datos de Amazon totalmente gestionada. Consulte la lista de motores de [origen](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Introduction.Sources.html) y [destino](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Introduction.Targets.html) compatibles en la Guía del usuario de AWS DMS.

Además de las migraciones, AWS DMS admite la replicación continua para muchos casos de uso, incluida la distribución y el desarrollo de bases de datos geográficas y la sincronización de entornos de prueba. Una tarea de replicación continua aplicará los cambios de la base de datos de origen a la base de datos de destino con una latencia mínima. Puede reproducir datos de una sola base de datos en una o más bases de datos de destino; o consolidar y reproducir los datos de varias bases de datos en una o más bases de datos de destino. Todas las características de AWS DMS, como la validación y las transformaciones de datos, están disponibles para una tarea de reproducción.

![ilustración de bases de datos](https://d1.awsstatic.com/rusmadei/dms-features-overview-1.a6f57b0c008ae7447b720c79813933eaef353935.jpeg)

## Page Topics

[Facilidad de uso](https://aws.amazon.com/es/dms/features/#product-features#dms-features-2#simple-to-use) [Amplitud de opciones](https://aws.amazon.com/es/dms/features/#product-features#dms-features-2#breadth-of-choices) [Tiempo de inactividad mínimo](https://aws.amazon.com/es/dms/features/#product-features#dms-features-2#minimal-downtime) [Rentabilidad](https://aws.amazon.com/es/dms/features/#product-features#dms-features-2#cost-effective) [Fiable](https://aws.amazon.com/es/dms/features/#product-features#dms-features-2#reliable) [Productividad para los desarrolladores](https://aws.amazon.com/es/dms/features/#product-features#dms-features-2#developer-productivity) [Preguntas frecuentes](https://aws.amazon.com/es/dms/features/#product-features#dms-features-2#faqs)

## Facilidad de uso

[Open all](https://aws.amazon.com/es/dms/features/#)

### No se requiere configuración

AWS DMS es fácil de usar. No es necesario instalar ningún controlador o aplicación y, en la mayoría de los casos, no es necesario realizar cambios en la [base de datos de origen](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Introduction.Sources.html). Puede iniciar la migración de una base de datos en tan solo unos pasos en la [consola de administración de AWS.](https://aws.amazon.com/console/)

### Planificación automatizada de la migración

[AWS DMS Fleet Advisor](https://aws.amazon.com/dms/fleet-advisor/) es una función gratuita y totalmente gestionada que automatiza la planificación de la migración mediante el inventario y la evaluación de la flota de almacén de datos y bases de datos operativas locales y la identificación de posibles rutas de migración. Mediante el uso de patrones históricos de rendimiento y uso recopilados de bases de datos autoadministradas, AWS DMS Fleet Advisor puede [recomendar motores de bases de datos de destino](https://docs.aws.amazon.com/dms/latest/userguide/fa-recommendations.html) y opciones de instancias, así como estimar los costos.

AWS DMS Fleet Advisor obtiene resultados en algunas horas, en lugar de en semanas o meses, sin usar herramientas de terceros y sin contratar a expertos en migración. Puede comenzar a [planificar la migración con AWS DMS Fleet Advisor](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_DMSStudio.FleetAdvisor.html) en unos pocos pasos en la consola de AWS DMS.  

## Amplitud de opciones

[Open all](https://aws.amazon.com/es/dms/features/#)

### Amplitud de opciones

Con AWS DMS, puede realizar una migración de bases de datos homogénea mediante la migración de bases de datos iguales o modernizarse con una migración de bases de datos heterogénea mediante la migración entre diferentes bases de datos. AWS DMS admite más de 20 bases de datos y almacenes de datos como puntos de enlace de origen y destino.

### Migraciones de base de datos homogénea

Para las migraciones homogéneas, la estructura del esquema, los tipos de datos y el código de la base de datos ya son compatibles entre las bases de datos de origen y destino. Algunos ejemplos de migraciones homogéneas son: [de Oracle a Amazon RDS para Oracle](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/migrate-an-on-premises-oracle-database-to-amazon-rds-for-oracle.html), [de MySQL a Amazon Aurora MySQL](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/AuroraMySQL.Migrating.RDSMySQL.html), [de MySQL a Amazon RDS para MySQL](https://docs.aws.amazon.com/dms/latest/sbs/chap-manageddatabases.mysql2rds.html) o [de Microsoft SQL Server a Amazon RDS para SQL Server.](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/migrate-an-on-premises-microsoft-sql-server-database-to-amazon-rds-for-sql-server.html) Usted crea una tarea de migración con conexiones a las bases de datos de origen y destino y, a continuación, inicia la migración en un solo paso. AWS DMS se ocupa del resto.

AWS DMS ofrece varias opciones para realizar migraciones homogéneas. La primera opción consiste en usar las [herramientas de base de datos nativas integradas](https://docs.aws.amazon.com/dms/latest/userguide/data-migrations.html) para migrar de forma automática a la base de datos de destino sin tener que administrar las instancias de replicación. Es mejor usarlo para migrar todos los tipos de datos y objetos secundarios para las migraciones de MySQL y PostgreSQL a Aurora y Amazon RDS como motores de destino. Hay opciones alternativas, como el uso de instancias de replicación de [AWS DMS Serverless](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Serverless.html) o [AWS DMS](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_ReplicationInstance.html), disponibles para todos los demás motores.

### Migraciones de bases de datos heterogéneas

En el caso de las migraciones heterogéneas, los motores de bases de datos de origen y de destino son diferentes, como en el caso de las migraciones de [Oracle a Aurora](https://aws.amazon.com/getting-started/hands-on/migrate-oracle-to-amazon-aurora/), de [Oracle a PostgreSQL](https://docs.aws.amazon.com/dms/latest/sbs/chap-rdsoracle2postgresql.html) o de [Microsoft SQL Server a MySQL](https://aws.amazon.com/blogs/database/migrating-a-sql-server-database-to-a-mysql-compatible-database-engine/). El proceso de las migraciones heterogéneas cuenta con dos pasos. Como la estructura del esquema, los tipos de datos y el código de la base de datos de las bases de datos de origen y destino pueden ser muy diferentes, el primer paso es convertir el esquema y el código de origen para que coincidan con los de la base de datos de destino. El segundo paso consiste en migrar los datos de la base de datos de origen a la base de datos de destino con AWS DMS. Puede elegir entre instancias de replicación de AWS DMS o AWS DMS Serverless, que automatizan las arduas tareas de aprovisionamiento, monitoreo y escalado de los recursos de migración. Todos los tipos de datos necesarios se convertirán de forma automática durante la migración. 

Para la conversión de esquemas, AWS DMS ofrece dos soluciones de conversión de esquemas que pueden ahorrar semanas o meses de esfuerzo. Puede optar por iniciar sesión en la consola de AWS DMS para iniciar el flujo de trabajo (AWS DMS SC) [AWS DMS Schema Conversion](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_SchemaConversion.html) y disfrutar de una experiencia totalmente administrada o descargar el software de [Herramienta de conversión de esquemas de AWS (AWS SCT)](https://docs.aws.amazon.com/SchemaConversionTool/latest/userguide/CHAP_Welcome.html) para realizar una evaluación y conversión similares en su sistema local.

Ambas opciones evaluarán y convertirán automáticamente el esquema de la base de datos de origen y la mayoría de los objetos de código de la base de datos, incluidas las vistas, los procedimientos almacenados y las funciones, a un formato compatible con la base de datos de destino. Con unos pocos pasos, puede generar un informe de evaluación que muestre la complejidad de la conversión de esquemas. Este informe proporciona recomendaciones sobre cómo resolver las incompatibilidades entre los motores de base de datos de origen y de destino. Cualquier objeto que no se pueda convertir automáticamente se marca con claridad como elemento de una acción con instrucciones prescriptivas sobre cómo llevar a cabo la conversión, para que se pueda convertir manualmente y así completar la migración. Una vez finalizada la conversión del esquema, AWS DMS puede migrar los datos del origen al destino.

AWS DMS SC usa IA generativa en combinación con un enfoque tradicional basado en reglas para reducir aún más la cantidad de objetos de bases de datos que requieren conversión manual. Con las recomendaciones de IA generativa, puede simplificar y acelerar sus proyectos de migración de bases de datos, especialmente al convertir objetos de código complejos, como procedimientos, funciones o activadores almacenados. La conversión de esquemas de AWS DMS con IA generativa acelera la migración al proporcionar recomendaciones de código revisables, lo que reduce el tiempo y el esfuerzo de las conversiones complejas y permite migraciones de bases de datos más rápidas y confiables. La característica está disponible para las conversiones de esquemas de motores comerciales, como Microsoft SQL Server, a la edición compatible con PostgreSQL de Amazon Aurora y Amazon Relational Database Service (Amazon RDS) para PostgreSQL. Para más información sobre AWS DMS SC, consulte la [documentación](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_SchemaConversion.html) y la [guía de introducción](https://docs.aws.amazon.com/dms/latest/userguide/getting-started.html). Consulte la documentación sobre las [conversiones de bases de datos compatibles con AWS DMS SC](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_SchemaConversion.html#schema-conversion-data-providers) y las [conversiones de AWS SCT](https://docs.aws.amazon.com/SchemaConversionTool/latest/userguide/CHAP_Welcome.html).

Para convertir sentencias SQL incrustadas en su aplicación, [Amazon Q Developer](https://aws.amazon.com/q/developer/) puede escanear el código de origen de la aplicación Java y convertir el código de Oracle a Amazon Aurora PostgreSQL o Amazon RDS para PostgreSQL.

## Tiempo de inactividad mínimo

[Open all](https://aws.amazon.com/es/dms/features/#)

### Tiempo de inactividad mínimo

AWS DMS le ayuda a migrar sus bases de datos a AWS prácticamente sin tiempo de inactividad. Todos los cambios de datos a la base de datos de origen que se producen durante la migración se reproducen de forma continua en el destino, lo que permite que la base de datos de origen esté completamente operativa durante el proceso de migración. Una vez finalizada la migración de la base de datos, la [base de datos de destino](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Introduction.Targets.html) permanecerá sincronizada con la de origen durante el tiempo que elija, lo que le permitirá cambiar a la base de datos de destino en el momento que desee.

## Rentabilidad

[Open all](https://aws.amazon.com/es/dms/features/#)

### Rentable

[Las instancias bajo demanda de AWS DMS](https://aws.amazon.com/dms/pricing/) le permiten pagar la capacidad de migración de bases de datos por hora sin compromisos a largo plazo. De este modo, puede olvidarse de los costos y las complejidades de planificar, comprar y mantener equipos, lo que permite que todo el proceso resulte más rápido y económico. Por lo tanto, la migración de una base de datos del tamaño de un terabyte se puede realizar de forma rentable.

### Capacidad de automatización

AWS DMS Serverless facilita aún más la migración de datos y la hace más rentable sin necesidad de aprovisionar instancias de replicación o supervisar el uso y ajustar la capacidad de forma manual. Aprovisiona, monitorea y escala automáticamente los recursos de migración a la capacidad óptima necesaria para satisfacer la demanda, eliminando las tareas de administración de instancias como la estimación de la capacidad, el aprovisionamiento, la optimización de costos y la administración de las versiones y parches del motor de replicación. Ya no necesita aprovisionar recursos en exceso para los picos de demanda y solo paga por la capacidad de migración de datos que utiliza. AWS DMS Serverless admite varios casos de uso, como la replicación continua de datos, la consolidación de bases de datos y las migraciones heterogéneas y homogéneas. Para obtener más información, consulte la documentación de [AWS DMS Serverless](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Serverless.html).

### Consolidación de bases de datos

Puede usar AWS DMS para optimizar aún más sus costos mediante la consolidación de las bases de datos, lo que reduce la cantidad de instancias de bases de datos y, por lo tanto, los costos de infraestructura. Al combinar varias bases de datos en un único sistema optimizado, las organizaciones pueden eliminar el almacenamiento redundante, reducir las tarifas de licencia y reducir los costos operativos. La consolidación de bases de datos se puede realizar para migraciones homogéneas y heterogéneas.

## Fiable

[Open all](https://aws.amazon.com/es/dms/features/#)

### Fiabilidad

AWS DMS es altamente resiliente y se autorrepara. Monitorea constantemente las bases de datos de origen y destino, la conectividad de red y las instancias de replicación. En caso de interrupción, reinicia automáticamente el proceso y continúa la migración desde donde se detuvo. La [opción Multi-AZ](https://docs.aws.amazon.com/dms/latest/userguide/disaster-recovery-resiliency.html) de AWS DMS ofrece alta disponibilidad para la migración de bases de datos y la replicación continua de datos con instancias de replicación redundantes.

## Productividad para los desarrolladores

[Open all](https://aws.amazon.com/es/dms/features/#)

### Productividad para los desarrolladores

AWS DMS se puede utilizar para migrar datos dentro y fuera de la nube con fines de desarrollo. Existen dos situaciones comunes. La primera consiste en implementar sistemas de desarrollo, de pruebas o de ensayo en AWS para aprovechar la escalabilidad y el rápido aprovisionamiento que ofrece la nube. Esto permite que los desarrolladores y los evaluadores puedan usar copias de datos de producción reales y copiar las actualizaciones de vuelta en el sistema de producción local.  
  
La segunda situación sucede cuando los sistemas de desarrollo se encuentran localmente (con frecuencia, en computadoras portátiles personales) y se migra una copia actual de una base de datos de producción de AWS a estos sistemas locales, ya sea por única vez o de manera continua. Se puede evitar interrumpir los procesos de DevOps existentes y, a su vez, garantizar la representación actualizada de su sistema de producción.

## Preguntas frecuentes

[Open all](https://aws.amazon.com/es/dms/features/#)

### ¿Para qué se utiliza AWS DMS?

AWS DMS se utiliza para migraciones de bases de datos y almacén de datos hacia y desde AWS, además de para la replicación continua de datos y la consolidación de bases de datos. Con AWS DMS, puede migrar a una base de datos de AWS totalmente gestionada. Al trasladar sus bases de datos comerciales y de código abierto autogestionadas a servicios de bases de datos de AWS totalmente gestionados, obtiene agilidad, acelera el tiempo de comercialización y mejora la disponibilidad, al tiempo que reduce los gastos operativos.

Como alternativa, puede optar por modernizar sus bases de datos mediante migraciones heterogéneas a bases de datos personalizadas de AWS. Con AWS, puede elegir las bases de datos adecuadas y optimizar la relación precio-rendimiento a cualquier escala.

### ¿Qué características de AWS DMS son gratuitas?

AWS DMS ofrece hasta 750 horas al mes para una instancia dms.t2.micro Single-AZ como parte del [nivel gratuito de AWS](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=*all&awsf.Free%20Tier%20Categories=categories%23databases). Dependiendo de la función, existe un costo basado en el uso. En el caso de AWS DMS Fleet Advisor y AWS DMS SC, solo paga por el almacenamiento que utiliza. En el caso de las opciones de migración de AWS DMS, tanto si utiliza instancias de replicación como opciones sin servidor, paga por hora por la capacidad que utiliza. Consulte los [precios de AWS DMS](https://aws.amazon.com/dms/pricing/) para obtener más información.

## Pasos siguientes

[

Pricing

## Visite la página de precios

](https://aws.amazon.com/dms/pricing/?nc=nsb&pg=faq)

[

Free Tier

](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html)