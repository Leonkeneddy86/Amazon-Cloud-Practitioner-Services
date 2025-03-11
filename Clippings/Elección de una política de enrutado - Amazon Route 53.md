---
title: "Elección de una política de enrutado - Amazon Route 53"
source: "https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy.html"
author:
published:
created: 2025-03-11
description: "Elija una política de direccionamiento antes de crear registros en Amazon Route 53."
tags:
  - "clippings"
---
[PDF](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/route53-dg.pdf#routing-policy)

[RSS](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/amazon-route-53-release-notes.rss)

Modo de enfoque

Elección de una política de enrutado - Amazon Route 53

Al crear un registro, puede seleccionar una política de direccionamiento, que determina cómo Amazon Route 53 responde a las consultas:

- **Política de direccionamiento simple**: se utiliza para un único recurso que realiza una función determinada para su dominio; por ejemplo, un servidor web que ofrece contenido para el sitio web example.com. Puede usar el enrutamiento simple para crear registros en una zona alojada privada.
- **Política de direccionamiento de conmutación por error**: se utiliza si desea configurar la conmutación por error activa-pasiva. Puede usar el enrutamiento de conmutación por error para crear registros en una zona alojada privada.
- **Política de direccionamiento de geolocalización**: se utiliza si desea dirigir el tráfico en función de la ubicación de los usuarios. Puede usar el enrutamiento por geolocalización para crear registros en una zona alojada privada.
- **Política de enrutamiento de geoproximidad**: se utiliza si desea dirigir el tráfico en función de la ubicación de los recursos y, opcionalmente, desviar el tráfico desde los recursos de una ubicación a los de otra. Puede usar el enrutamiento por geoproximidad para crear registros en una zona alojada privada.
- **Política de enrutamiento de latencia**: utilícela cuando tenga varios recursos Regiones de AWS y desee enrutar el tráfico a la región que proporciona la mejor latencia. Puede usar el enrutamiento de latencia para crear registros en una zona alojada privada.
- **Política de direccionamiento basada en IP**: se usa cuando se quiere enrutar el tráfico en función de la ubicación de los usuarios, y tener las direcciones IP de las que se origina el tráfico.
- **Política de direccionamiento de respuesta con varios valores**: se utiliza si desea que Route 53 responda a consultas de DNS con hasta ocho registros de estado seleccionados al azar. Puede usar el enrutamiento de respuesta multivalor para crear registros en una zona alojada privada.
- **Política de direccionamiento ponderada**: se utiliza para dirigir el tráfico a varios recursos en las proporciones que especifique. Puede usar el enrutamiento ponderado para crear registros en una zona alojada privada.

###### Temas

- [Direccionamiento simple](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-simple.html)
- [Enrutado de conmutación por error](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-failover.html)
- [Enrutado de geolocalización](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-geo.html)
- [Enrutamiento por geoproximidad](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-geoproximity.html)
- [Enrutado basado en latencia](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-latency.html)
- [Direccionamiento basado en IP](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-ipbased.html)
- [Direccionamiento de respuesta con varios valores](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-multivalue.html)
- [Direccionamiento ponderado](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-weighted.html)
- [Cómo Amazon Route 53 utiliza EDNS0 para calcular la ubicación de un usuario](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-edns0.html)

[Enviar comentarios](https://docs.aws.amazon.com/forms/aws-doc-feedback?hidden_service_name=Route53&topic_url=https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy.html)

#### Tema siguiente:

[Direccionamiento simple](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/routing-policy-simple.html)

#### Tema anterior:

[Uso de registros](https://docs.aws.amazon.com/es_es/Route53/latest/DeveloperGuide/rrsets-working-with.html)

#### ¿Necesita ayuda?

- [Probar AWS re:Post](https://repost.aws/es/tags/TAceSYwryvTxuK8Uw1UKOTVA)
- [Contacte con un experto de AWS IQ](https://iq.aws.amazon.com/get-started/?utm=docs&service=Amazon%20Route%C2%A053)