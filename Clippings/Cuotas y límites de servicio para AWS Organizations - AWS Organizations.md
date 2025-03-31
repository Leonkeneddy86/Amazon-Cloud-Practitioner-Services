---
title: "Cuotas y límites de servicio para AWS Organizations - AWS Organizations"
source: "https://docs.aws.amazon.com/es_es/organizations/latest/userguide/orgs_reference_limits.html"
author:
published:
created: 2025-03-31
description: "AWS Organizations Úselo para crear, organizar y administrar su Cuentas de AWS. Invite a otras cuentas a que se unan a su organización y organice sus cuentas en unidades organizativas acordes con sus modelos de negocio."
tags:
  - "clippings"
---
## Cuotas y límites de servicio para AWS Organizations

[PDF](https://docs.aws.amazon.com/es_es/organizations/latest/userguide/organizations-userguide.pdf#orgs_reference_limits) [RSS](https://docs.aws.amazon.com/es_es/organizations/latest/userguide/aws-organizations-release-notes.rss)  Modo de enfoque Cuotas y límites de servicio para AWS Organizations - AWS Organizations

Las traducciones son generadas a través de traducción automática. En caso de conflicto entre la traducción y la version original de inglés, prevalecerá la version en inglés.

Las traducciones son generadas a través de traducción automática. En caso de conflicto entre la traducción y la version original de inglés, prevalecerá la version en inglés.

En este tema se describen las cuotas y los límites de servicio para AWS Organizations.

## Directrices de nomenclatura

Las siguientes son pautas para los nombres que se crean AWS Organizations, incluidos los nombres de las cuentas, las unidades organizativas (OUs), las raíces y las políticas:

- Los nombres deben estar compuestos por caracteres Unicode.
- La longitud máxima de cadena para los nombres varía según el objeto. Para obtener información sobre el límite real de cada objeto, consulte la [Referencia de la API de AWS Organizations](https://docs.aws.amazon.com/organizations/latest/APIReference/), busque la operación de API que crea el objeto y consulte los detalles del parámetro `Name` de esa operación. Por ejemplo:[Nombre de cuenta](https://docs.aws.amazon.com/organizations/latest/APIReference/API_CreateAccount.html#organizations-CreateAccount-request-AccountName), o bien [Nombre de OU](https://docs.aws.amazon.com/organizations/latest/APIReference/API_CreateOrganizationalUnit.html#organizations-CreateOrganizationalUnit-request-Name).

## Consideraciones

Los códigos de cuota de servicio pueden cambiar con el tiempo debido a las actualizaciones. Esto no afecta a los valores ni a los nombres de las cuotas. Para encontrar el código de cuota de una cuota específica, utilice la [ListServiceQuotas](https://docs.aws.amazon.com/servicequotas/2019-06-24/apireference/API_ListServiceQuotas.html) operación y busque la `QuotaCode` respuesta de la cuota que desee en el resultado.

## Valores mínimos y máximos

Los siguientes son los máximos ***predeterminados*** para las entidades de AWS Organizations.

###### nota

Puede solicitar aumentos de algunos de estos valores mediante la [Consola Service Quotas](https://console.aws.amazon.com/servicequotas/home?region=us-east-1#!/services/organizations/quotas).

Organizations es un servicio global alojado físicamente en la región EE. UU. Este (Norte de Virginia) ( `us-east-1` ). Por lo tanto, debe `us-east-1` utilizarlas para acceder a las cuotas de Organizations cuando utilice la consola Service Quotas AWS CLI, el o un AWS SDK.

### Límites por AWS servicio

La mayoría Servicios de AWS admite el número máximo de cuentas indicado que puede tener en una organización. Sin embargo, algunos servicios establecen límites de cuentas distintos de la cantidad máxima de cuentas permitidas en una organización.

En las siguientes tablas se muestran los servicios con límites de cuentas distintos.

Para obtener más información, consulte [AWS IAM Identity Center quotas](https://docs.aws.amazon.com/singlesignon/latest/userguide/limits.html) en la *Guía del usuario de IAM Identity Center* y [AWS MGN service quota limits](https://docs.aws.amazon.com/mgn/latest/ug/MGN-service-limits.html) en la *Guía del usuario de Application Migration Service*.

## Tiempo de vencimiento de protocolos de enlace (handshakes)

Los siguientes son los tiempos de espera para los apretones de manos. AWS Organizations

## Número de políticas que puede asociar a una entidad

El mínimo y máximo depende del tipo de política y de la entidad a la que asocia la política. En la siguiente tabla se muestra cada tipo de política y el número de entidades a la se puede asociar cada tipo.

###### nota

Estos números solo se aplican a las políticas que están directamente adjuntas a una unidad organizativa o a una cuenta. Las políticas que afectan a una unidad organizativa o a una cuenta por herencia ***no*** cuentan contra estos límites. Los límites de las políticas no se pueden superar.

###### nota

Solo puede tener un nodo raíz en una organización.

## Límites de limitación

En las siguientes tablas se enumeran AWS Organizations APIs las categorías de gestión y se muestran sus respectivas tasas de aceleración a nivel de cuenta y organización.

AWS Organizations utiliza el [algoritmo token bucket](https://en.wikipedia.org/wiki/Token_bucket) para implementar la regulación de las API. Con este algoritmo, su cuenta tiene un *bucket* que contiene un número específico de *tokens*. El número de tokens del bucket representa su cuota de limitación en un segundo determinado.

La *velocidad* es el ritmo fijo al que se añaden los tokens al depósito de fichas por segundo.

La *ráfaga* es la cantidad máxima de fichas que se pueden añadir y la cantidad máxima de fichas que se pueden utilizar por segundo.

Por ejemplo, la `DescribeAccount` API está limitada Cuenta de AWS a 20 solicitudes por segundo como velocidad de referencia y a 30 solicitudes por segundo como velocidad de ráfaga. La velocidad de ráfaga de 30 solicitudes por segundo te permite superar temporalmente la velocidad de referencia de 20 solicitudes por segundo.

Puede realizar 20 solicitudes en el primer segundo, que es la velocidad de referencia. En el segundo siguiente, puedes realizar 30 solicitudes, superando la línea base pero manteniéndote dentro de la velocidad de ráfaga de 30. Sin embargo, en el tercer segundo, si intenta realizar más de 20 solicitudes, se verá limitado, ya que ha superado la velocidad de referencia y se ha utilizado la capacidad de ráfaga.

La velocidad de ráfaga te permite gestionar los picos de tráfico temporales sin que te limites, siempre y cuando el promedio de solicitudes por segundo se mantenga dentro del límite de referencia a lo largo del tiempo.

### Límites de administración de cuentas

En la siguiente tabla se enumeran las correspondientes a la administración AWS Organizations APIs de cuentas.

### Límites de administración del protocolo de enlace

En la siguiente tabla se muestra el apretón AWS Organizations APIs de manos de la cuenta.

### Límites de administración de organizaciones

La siguiente tabla muestra la gestión AWS Organizations APIs de la organización.

### Límites de administración de políticas

En la siguiente tabla se enumeran las políticas AWS Organizations APIs para la gestión.

### Límites de administración de servicios

En la siguiente tabla se muestra la AWS Organizations APIs para la administración de servicios.

### En esta página

[Enviar comentarios](https://docs.aws.amazon.com/forms/aws-doc-feedback?hidden_service_name=Organizations&topic_url=https://docs.aws.amazon.com/es_es/organizations/latest/userguide/orgs_reference_limits.html)

#### Tema siguiente:

[Compatibilidad de regiones](https://docs.aws.amazon.com/es_es/organizations/latest/userguide/region-support.html)

#### Tema anterior:

[Terminología y conceptos](https://docs.aws.amazon.com/es_es/organizations/latest/userguide/orgs_getting-started_concepts.html)

#### ¿Necesita ayuda?

- [Contacte con un experto de AWS IQ](https://iq.aws.amazon.com/get-started/?utm=docs&service=AWS%20Organizations)