---
title: 'Notas de la versión de Live Video Analytics on IoT Edge: Azure'
description: En este tema se proporcionan las notas de la versión sobre las mejoras, las versiones, las correcciones de errores y los problemas conocidos de Live Video Analytics on IoT Edge.
ms.topic: conceptual
ms.date: 04/27/2020
ms.openlocfilehash: 28260728532d9db52b8d36488c2e456bd11803ea
ms.sourcegitcommit: 3d79f737ff34708b48dd2ae45100e2516af9ed78
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/23/2020
ms.locfileid: "87091786"
---
# <a name="live-video-analytics-on-iot-edge-release-notes"></a>Notas de la versión de Live Video Analytics on IoT Edge

>Reciba notificaciones para volver a visitar esta página y obtener actualizaciones; para ello, copie y pegue esta URL (`https://docs.microsoft.com/api/search/rss?search=%22Live+Video+Analytics+on+IoT+Edge+release+notes%22&locale=en-us`) en el lector de fuentes RSS.

En este artículo se proporciona información acerca de lo siguiente:

* Versiones más recientes
* Problemas conocidos
* Corrección de errores
* Funciones obsoletas

## <a name="july-13-2020"></a>13 de julio de 2020

La etiqueta de versión de la actualización de julio de 2020 del módulo es la siguiente:

```
     mcr.microsoft.com/media/live-video-analytics:1.0.2
```

> [!NOTE]
> En los inicios rápido y tutoriales, los manifiestos de implementación usan una etiqueta de 1 (live-video-analytics:1). Por lo tanto, con solo repetir la implementación de tales manifiestos se actualizará el módulo en los dispositivos perimetrales.

### <a name="new-features"></a>Nuevas características
* Ahora puede crear topologías de grafos que tengan un nodo receptor de recursos, así como un nodo receptor de archivos de nivel inferior de un nodo procesador de puerta de señal. Consulte [aquí](https://github.com/Azure/live-video-analytics/tree/master/MediaGraph/topologies/evr-motion-assets-files) para ver un ejemplo.

### <a name="bug-fixes"></a>Corrección de errores
* Mejoras en la validación de las propiedades deseadas

## <a name="june-1-2020"></a>1 de junio de 2020

Esta versión es la primera versión preliminar pública de Live Video Analytics on IoT Edge. La etiqueta de versión es la siguiente:

```
     mcr.microsoft.com/media/live-video-analytics:1.0.0
```

### <a name="supported-functionalities"></a>Funcionalidades admitidas
* Analice secuencias de vídeo en directo con los módulos de inteligencia artificial que prefiera y, de manera opcional, grabe vídeos en su dispositivo perimetral o en la nube.
* Use este módulo en sistemas operativos Linux AMD64 [compatibles](../../iot-edge/support.md) con IoT Edge.
* Implemente y configure el módulo a través de IoT Hub mediante Azure Portal o Visual Studio Code.
* Administre [topologías e instancias de grafos](media-graph-concept.md#media-graph-topologies-and-instances) de forma remota o local mediante la llamada a los siguientes métodos directos:

    *   GraphTopologyGet
    *   GraphTopologySet
    *   GraphTopologyDelete
    *   GraphTopologyList
    *   GraphInstanceGet
    *   GraphInstanceSet
    *   GraphInstanceDelete
    *   GraphInstanceList


## <a name="next-steps"></a>Pasos siguientes

[Información general](overview.md)
