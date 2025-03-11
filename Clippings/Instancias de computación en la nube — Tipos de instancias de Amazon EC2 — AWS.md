---
title: "Instancias de computación en la nube — Tipos de instancias de Amazon EC2 — AWS"
source: "https://aws.amazon.com/es/ec2/instance-types/"
author:
  - "[[Amazon Web Services]]"
  - "[[Inc.]]"
published:
created: 2025-03-11
description: "Los tipos de instancias de Amazon EC2 se componen de distintas combinaciones de CPU, memoria, almacenamiento y capacidad de redes. Esto le otorga la flexibilidad de elegir la instancia que mejor se adapte a sus necesidades."
tags:
  - "clippings"
---
Contenido de la página

[Uso general](https://aws.amazon.com/es/ec2/instance-types/#General_Purpose) [Optimizadas para informática](https://aws.amazon.com/es/ec2/instance-types/#Compute_Optimized) [Optimizadas para memoria](https://aws.amazon.com/es/ec2/instance-types/#Memory_Optimized) [Informática acelerada](https://aws.amazon.com/es/ec2/instance-types/#Accelerated_Computing) [Optimizadas para almacenamiento](https://aws.amazon.com/es/ec2/instance-types/#Storage_Optimized) [Optimizadas para HPC](https://aws.amazon.com/es/ec2/instance-types/#HPC_Optimized) [Características de las instancias](https://aws.amazon.com/es/ec2/instance-types/#Instance_Features) [Medición del rendimiento de las instancias](https://aws.amazon.com/es/ec2/instance-types/#Measuring_Instance_Performance)

## Uso general

Las instancias de uso general brindan una combinación equilibrada de recursos informáticos, de memoria y de red. Además, pueden usarse para distintas cargas de trabajo. Estas instancias son ideales para las aplicaciones que usan estos recursos en partes iguales, como los servidores web y los repositorios de código. 

Todas las vCPU de las instancias de Amazon EC2 basadas en Graviton son un núcleo de procesador de AWS Graviton.  

Todas kas vCPU de las instancias de Amazon EC2 no basadas en Graviton son un subproceso de un procesador basado en x86, excepto en instancias M7a, instancias T2 y m3.medium.

† AVX, AVX2 y las redes mejoradas solo están disponibles en las instancias lanzadas con AMI HVM.

\* Número predeterminado y máximo de CPU virtuales disponible para este tipo de instancia. Puede especificar un número personalizado de vCPUs al lanzar este tipo de instancia. Si desea obtener más detalles acerca de los totales válidos de CPU virtuales y cómo empezar a usar esta característica, consulte la página de documentación relacionada con este tema [aquí](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-optimize-cpu.html).

\*\* Estas instancias M4 pueden lanzarse en un procesador Intel Xeon E5-2686 v4 (Broadwell).  

\*\*\*Las instancias con la indicación de ancho de banda “Hasta” cuentan con un ancho de banda de base y pueden utilizar un mecanismo de crédito E/S de red para superar el ancho de banda de referencia en función del mejor esfuerzo. Para obtener más información, consulte [Ancho de banda de la red de instancias](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-network-bandwidth.html).  

## Optimizado para computación

Las instancias optimizadas para la computación son ideales para las aplicaciones que dependen de los recursos de computación y se benefician de los procesadores de alto rendimiento. Las instancias que forman parte de esta categoría funcionan bien con las cargas de trabajo de procesamiento por lotes, la transcodificación de archivos multimedia, los servidores web de alto rendimiento, la computación de alto rendimiento (HPC), la creación de modelos científicos, los servidores de videojuegos y los motores de servidor de publicidad dedicados, la inferencia del machine learning, entre otras aplicaciones con uso intensivo de computación.  

Todas las vCPU de las instancias de Amazon EC2 basadas en Graviton son un núcleo de procesador de AWS Graviton.  

Cada vCPU en las instancias de Amazon EC2 no basadas en Graviton es un subproceso de procesador basado en x86, excepto en las instancias C7a.  

† AVX, AVX2 y las redes mejoradas solo están disponibles en las instancias lanzadas con AMI HVM.

\* Número predeterminado y máximo de CPU virtuales disponible para este tipo de instancia. Puede especificar un número personalizado de vCPUs al lanzar este tipo de instancia. Si desea obtener más detalles acerca de los totales válidos de CPU virtuales y cómo empezar a utilizar esta característica, consulte la página de documentación de optimización de CPU [aquí](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-optimize-cpu.html).

\*\*\*Las instancias con la indicación de ancho de banda “Hasta” cuentan con un ancho de banda de base y pueden utilizar un mecanismo de crédito E/S de red para superar el ancho de banda de referencia en función del mejor esfuerzo. Para obtener más información, consulte [Ancho de banda de la red de instancias](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-network-bandwidth.html).  

## Optimizadas para la memoria

Las instancias optimizadas para la memoria se diseñaron con el objetivo de brindar un rendimiento rápido para las cargas de trabajo que procesan grandes conjuntos de datos en la memoria.  

Todas las vCPU de las instancias de Amazon EC2 basadas en Graviton son un núcleo de procesador de AWS Graviton.  

Cada vCPU en las instancias de Amazon EC2 no basadas en Graviton es un subproceso de procesador basado en x86, excepto en las instancias R7a.  

† AVX, AVX2 y las redes mejoradas solo están disponibles en las instancias lanzadas con AMI de HVM.  

\*\*\*Las instancias con la indicación de ancho de banda de la red “Hasta” cuentan con una banda ancha de base y pueden utilizar un mecanismo de crédito E/S de red para superar el banda ancha de referencia en función del mejor esfuerzo. Para obtener más información, consulte [Ancho de banda de la red de instancias](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-network-bandwidth.html).  

## Computación acelerada

En las instancias de computación acelerada, se utilizan aceleradores de hardware, o coprocesadores, para realizar funciones, como el cálculo de números de coma flotante, el procesamiento de gráficos o la búsqueda de coincidencias de patrones de datos, con una eficiencia mayor de la ofrecida en un software que se ejecuta en CPU.  

Cada CPU virtual es un proceso de un núcleo Intel Xeon o AMD EPYC, excepto en el caso de T2 y m3.medium.

† AVX, AVX2, AVX-512 y las redes mejoradas solo están disponibles en las instancias lanzadas con AMI HVM.

\* Número predeterminado y máximo de CPU virtuales disponible para este tipo de instancia. Puede especificar un número personalizado de vCPUs al lanzar este tipo de instancia. Si desea obtener más detalles acerca de los totales válidos de CPU virtuales y cómo empezar a utilizar esta característica, consulte la página de documentación de optimización de CPU [aquí](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-optimize-cpu.html).

\*\*\*Las instancias con la indicación de banda ancha “Hasta” cuentan con un banda ancha de base y pueden utilizar un mecanismo de crédito E/S de red para superar el banda ancha de referencia en función del mejor esfuerzo. Para obtener más información, consulte [Ancho de banda de la red de instancias](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-network-bandwidth.html).  

## Optimizadas para el almacenamiento

Las instancias optimizadas para almacenamiento se diseñaron para las cargas de trabajo que necesitan acceso de escritura y lectura secuencial alto a conjuntos de datos muy grandes en el almacenamiento local. Se optimizan para brindar decenas de miles de operaciones de E/S aleatorias de baja latencia por segundo (IOPS) a las aplicaciones.  

\*\* i3.metal ofrece 72 procesadores lógicos en 36 núcleos físicos

¿Está buscando instancias de la generación anterior que no aparecen aquí? Consulte la página [Instancias de la generación anterior](https://aws.amazon.com/es/ec2/previous-generation/).  

## Optimizadas para HPC

Las instancias de computación de alto rendimiento (HPC) están diseñadas específicamente con el fin de ofrecer el mejor rendimiento de precio para ejecutar cargas de trabajo de HPC a escala en AWS. Las instancias de HPC son ideales para aplicaciones que se benefician de procesadores de alto rendimiento, como simulaciones grandes y complejas y cargas de trabajo de aprendizaje profundo.  

## Características de las instancias

Las instancias de Amazon EC2 proporcionan múltiples características adicionales que le ayudarán a implementar, administrar y escalar sus aplicaciones.  

Instancias de rendimiento ampliable

Amazon EC2 le permite elegir entre las familias de instancias de rendimiento fijo (por ejemplo, M6, C6 y R6) e instancias de rendimiento ampliable (por ejemplo, T3). Las instancias de rendimiento ampliable proporcionan un nivel base de rendimiento de la CPU con capacidad de ampliarse por encima ese nivel.

Las instancias T ilimitadas pueden conservar un rendimiento de CPU alto durante el tiempo que una carga de trabajo lo necesite. Para la mayoría de las cargas de trabajo generales, las instancias T ilimitadas ofrecerán rendimiento amplio sin cargo adicional. El precio por hora de la instancia T cubre automáticamente todos los picos temporales de uso cuando la utilización de CPU promedio de una instancia T es igual o menor al valor base durante un período de 24 horas. Si la instancia requiere un mayor uso de la CPU durante un período prolongado, puede hacerlo con un cargo fijo adicional de 5 centavos de USD por hora de CPU virtual.

El rendimiento base y la capacidad de ampliación de las instancias T se rigen por los créditos de la CPU. Toda instancia T recibe constantemente créditos de la CPU, cuyo porcentaje depende del tamaño de la instancia. Las instancias T acumulan créditos de la CPU cuando están inactivas y utilizan los créditos de la CPU cuando están activas. Un crédito de la CPU proporciona el rendimiento de un núcleo de la CPU completa durante un minuto.

Por ejemplo, una instancia t2.small recibe créditos continuamente con una frecuencia de 12 créditos de CPU por hora. Esta capacidad proporciona un rendimiento base equivalente al 20% del núcleo de una CPU (20% x 60 min = 12 min). Si la instancia no utiliza los créditos que recibe, se almacenan en el saldo de créditos de la CPU hasta un máximo de 288 créditos de CPU. Cuando la instancia t2.small necesita ampliarse hasta más del 20% de un núcleo, extrae esta capacidad del crédito de la CPU para administrar este aumento automáticamente.

Con la instancia T2 ilimitada activada, la instancia t2.small puede ampliarse por encima del valor base, inclusive después de disminuir a cero el saldo de crédito de la CPU. Para la gran mayoría de las cargas de trabajo generales en las que el uso de CPU promedio es igual o menor al rendimiento base, el precio básico por hora de la instancia t2.small cubre todas las ampliaciones de la CPU. Si la instancia se ejecuta con un uso de CPU promedio del 25% (5% por encima del valor base) durante un período de 24 horas después de que el saldo de crédito de CPU haya disminuido a cero, se le cobrará un monto adicional de 6 centavos (5 centavos/hora de CPU virtual x 1 CPU virtual x 5% x 24 horas).

Muchas aplicaciones, como servidores web, entornos para desarrolladores y pequeñas bases de datos, no necesitan de manera constante altos niveles de CPU, pero sí les beneficia considerablemente disponer de acceso completo a CPU muy rápidas cuando las necesitan. Las instancias T se diseñan específicamente para estos casos de uso. Si necesita un rendimiento de la CPU alto de manera consistente para aplicaciones como, por ejemplo, codificación de video, sitios web de alto volumen o aplicaciones HPC, le recomendamos que use instancias de rendimiento fijo. Las instancias T están diseñadas para funcionar como si tuvieran núcleos de procesadores de gran velocidad, dedicados y disponibles cuando la aplicación necesita realmente el rendimiento de la CPU, mientras que lo protege del rendimiento variable o de otros efectos colaterales comunes que podría observar normalmente por suscripciones excesivas en otros entornos.  

Múltiples opciones de almacenamiento

Amazon EC2 le permite elegir entre múltiples opciones de almacenamiento en función de sus necesidades. [Amazon EBS](https://aws.amazon.com/es/ebs/) es un volumen de almacenamiento de nivel de bloque duradero que se puede asociar a una instancia única de Amazon EC2 que ya esté en ejecución. Puede usar Amazon EBS como dispositivo de almacenamiento primario para datos que requieran actualizaciones granulares con frecuencia. Por ejemplo, Amazon EBS es la opción de almacenamiento recomendada si se ejecuta una base de datos en Amazon EC2. Los volúmenes de Amazon EBS persisten con independencia de la vida útil de la instancia de Amazon EC2. Una vez que el volumen se adjunte a una instancia, puede usarlo como cualquier otra unidad física de disco duro. Amazon EBS proporciona tres tipos de volúmenes para satisfacer mejor las necesidades de las cargas de trabajo: uso general (SSD), IOPS provisionadas (SSD) y magnéticos. El uso general (SSD) es el nuevo tipo de volumen de EBS de uso general con respaldo SSD que se recomienda como la opción predeterminada para los clientes. Los volúmenes de uso general (SSD) están indicados para una amplia gama de cargas de trabajo, como bases de datos pequeñas y medianas, entornos de desarrollo y pruebas, y volúmenes de arranque. Los volúmenes de E/S por segundo aprovisionadas (SSD) ofrecen almacenamiento con un rendimiento consistente y de baja latencia y se han diseñado para aplicaciones con requisitos de E/S elevados, como las [bases de datos NoSQL](https://aws.amazon.com/es/nosql/) o relacionales de gran tamaño. Los volúmenes magnéticos proporcionan el costo por gigabyte más bajo de todos los tipos de volúmenes de EBS. Los volúmenes magnéticos son ideales para cargas de trabajo de acceso poco frecuente a los datos y aplicaciones en las que es importante reducir al mínimo el costo de almacenamiento.

Muchas instancias de Amazon EC2 también pueden incluir almacenamiento de dispositivos ubicados dentro de la computadora host lo que se conoce como almacenamiento de instancias. El almacenamiento de instancias proporciona almacenamiento temporal a nivel de bloque para las instancias de Amazon EC2. Los datos del almacenamiento de instancias persisten únicamente durante la vida de la instancia de Amazon EC2 asociada.  

Además del almacenamiento de nivel de bloque mediante Amazon EBS o el almacenamiento de instancias, también puede utilizar Amazon S3 para el almacenamiento de objetos altamente disponible y de larga duración. Para obtener más información sobre las opciones de almacenamiento de Amazon EC2, consulte la [documentación de Amazon EC2](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Storage.html).

Instancias optimizadas para EBS

Para disfrutar de una cuota reducida y adicional por horas, los clientes pueden lanzar tipos de instancias de Amazon EC2 seleccionados como instancias optimizadas para EBS. Las instancias optimizadas para EBS permiten que las instancias de EC2 utilicen plenamente las IOPS aprovisionadas en un volumen de EBS. Las instancias optimizadas para EBS ofrecen un rendimiento específico dedicado entre Amazon EC2 y Amazon EBS, con opciones de entre 500 megabits por segundo (Mbps) y 80 gigabits por segundo (Gbps), en función del tipo de instancia utilizado. El rendimiento específico minimiza los conflictos entre las E/S de Amazon EBS y otro tráfico procedente de la instancia de EC2, lo que proporciona el máximo rendimiento en los volúmenes de EBS. Las instancias optimizadas para EBS están diseñadas para utilizarse con todos los volúmenes de EBS. Cuando se adjuntan a instancias optimizadas para EBS, los volúmenes de IOPS provisionadas pueden conseguir latencias de milisegundos de un solo dígito y están diseñados para ofrecer en torno al 10 % del rendimiento de IOPS aprovisionadas el 99,9 % del tiempo. Recomendamos la utilización de volúmenes de IOPS provisionadas con instancias optimizadas para EBS o instancias soportadas en redes de clústeres para aquellas aplicaciones con unos requisitos de almacenamiento de E/S elevados.

Redes de clústeres

Seleccione las instancias EC2 soportadas en redes de clústeres cuando se lancen en un grupo de ubicación en clúster común. Un grupo de ubicación en clúster ofrece redes de baja latencia entre todas las instancias en el clúster. El ancho de banda que puede utilizar una instancia EC2 depende del tipo de instancia y de la especificación del rendimiento de red. El tráfico entre instancias dentro de la misma región puede utilizar hasta 5 Gbps para el flujo único y hasta 100 Gbps para el tráfico de flujo múltiple en cada dirección (dúplex completo). El tráfico hacia y desde los buckets de S3 en la misma región también puede utilizar todo el ancho de banda adicional de la instancia disponible. Cuando se lanza en un grupo de ubicación, las instancias pueden utilizar hasta 10 Gbps para el tráfico de flujo simple y hasta 100 Gbps para el tráfico de flujo múltiple. El tráfico de redes hacia Internet se limita a 5 Gbps (dúplex completo). Las redes de clústeres son ideales para sistemas de análisis de alto rendimiento y muchas aplicaciones científicas y de ingeniería, especialmente aquellas que usan la biblioteca MPI estándar para la programación paralela.

Características del procesador Intel

![](https://d1.awsstatic.com/logos/xeon-pltnm-m-ww-rgb-60%20(2).e96b4823a7c4d2d8e2a0984fcc440ebbe852ea9d.png)

Las instancias de Amazon EC2 que cuentan con un procesador Intel pueden ofrecer acceso a las siguientes características del procesador:

- **Intel AES New Instructions (AES-NI):** el conjunto de instrucciones de cifrado Intel AES-NI mejora el algoritmo Estándar de cifrado avanzado (AES) original para ofrecer una protección de los datos más rápida y mayor seguridad. Todas las instancias EC2 de la generación actual soportan esta característica del procesador.
- **Extensiones vectoriales avanzadas de Intel (Intel AVX, Intel AVX2 y AVX-512)**: Intel AVX e Intel AVX2 son extensiones de conjuntos de instrucciones de 256 bits, mientras que Intel AVX-512 es una extensión de conjuntos de instrucciones de 512 bits. Están diseñadas para aplicaciones con un uso intensivo de coma flotante (FP). Las instrucciones Intel AVX mejoran el rendimiento de aplicaciones de procesamiento de audio/vídeo e imágenes, simulaciones científicas, análisis financieros, y análisis y modelado en 3D. Estas características solo están disponibles en las instancias ejecutadas con AMI HVM.
- **Intel Turbo Boost Technology:** Intel Turbo Boost Technology ofrece más rendimiento cuando se necesita. El procesador permite ejecutar núcleos automáticamente con mayor rapidez que la frecuencia operativa básica para poder hacer más cosas con mayor rapidez.
- **Intel Deep Learning Boost (Intel DL Boost):** un nuevo conjunto de tecnologías de procesadores integradas que están diseñadas para agilizar los casos de uso de aprendizaje profundo de IA. Los procesadores escalables Intel Xeon de segunda generación amplían las instrucciones Intel AVX-512 con una nueva instrucción de red neuronal vectorial (VNNI/INT8) que aumenta significativamente el rendimiento de la inferencia del aprendizaje profundo en comparación con los procesadores escalables Intel Xeon de la generación anterior (con FP32), para el reconocimiento o la segmentación de imágenes, la detección de objetos, el reconocimiento de voz, la traducción de idiomas, los sistemas de recomendaciones, el aprendizaje mediante refuerzo y otros. VNNI puede no ser compatible con todas las distribuciones Linux. Verifique la documentación antes de usarla.

No todas las características del procesador están disponibles en todos los tipos de instancias. Compruebe la matriz de tipos de instancias para obtener información más detallada sobre qué características están disponibles en cada tipo de instancia.

## Medición del rendimiento de las instancias

¿Por qué debería medir el rendimiento de las instancias?

Amazon EC2 le permite aprovisionar múltiples tipos de instancia que proporcionan diferentes combinaciones de CPU, memoria, disco y redes. Resulta sencillo realizar el lanzamiento de instancias nuevas y la ejecución de pruebas en paralelo, y le recomendamos que mida el rendimiento de las aplicaciones para identificar los tipos de instancia adecuados y validar la arquitectura de su aplicación. También recomendamos pruebas rigurosas de carga/escala para garantizar que sus aplicaciones pueden escalar de acuerdo con sus necesidades.  

Consideraciones para la evaluación del rendimiento de Amazon EC2

Amazon EC2 proporciona una gran variedad de opciones en diez tipos de instancia diferentes, cada uno de ellos con una o varias opciones de tamaño, organizados en familias de instancias diferentes optimizadas para diferentes tipos de aplicación. Le recomendamos que evalúe los requisitos de sus aplicaciones y seleccione la familia de instancias apropiada como punto de partida para la evaluación del rendimiento de su aplicación. Debe comenzar la evaluación del rendimiento del siguiente modo: (a) identifique las necesidades de su aplicación y compárelas con las diferentes familias de instancias (por ejemplo, si está relacionada con los procesos, con la memoria, etc.), y (b) determine su carga de trabajo para identificar el tamaño de instancia adecuado. No hay una alternativa para la medición del rendimiento de toda su aplicación, ya que el rendimiento de la aplicación puede estar supeditado a la infraestructura subyacente o a las limitaciones de arquitectura y software. Le recomendamos que realice pruebas a nivel de aplicación que incluyan el uso de herramientas y servicios de análisis de rendimiento de la aplicación y de evaluación de la carga. Para obtener más información, abra un caso de soporte y solicite especificaciones de rendimiento de red adicionales para el tipo de instancia específico que le interese.