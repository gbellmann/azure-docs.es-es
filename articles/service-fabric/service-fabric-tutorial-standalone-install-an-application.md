---
title: Instalación de una aplicación en un clúster independiente
description: En este tutorial aprenderá a instalar una aplicación en el clúster de Service Fabric independiente.
author: dkkapur
ms.topic: tutorial
ms.date: 07/22/2019
ms.author: dekapur
ms.custom: mvc
ms.openlocfilehash: 8dd47d27f928cb33e5a2bbc3ba9a6ab2bc044852
ms.sourcegitcommit: dabd9eb9925308d3c2404c3957e5c921408089da
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/11/2020
ms.locfileid: "86245388"
---
# <a name="tutorial-deploy-an-application-on-your-service-fabric-standalone-cluster"></a>Tutorial: implementación de una aplicación en el clúster de Service Fabric independiente

Los clústeres de Service Fabric independientes ofrecen la opción de elegir un entorno propio y crear un clúster como parte del enfoque "Cualquier sistema operativo, cualquier nube" que toma Service Fabric. En esta serie de tutoriales se crea un clúster independiente hospedado en AWS y se implementa en él una aplicación.

Este tutorial es la tercera parte de una serie.  Los clústeres de Service Fabric independientes ofrecen la opción de elegir un entorno propio y crear un clúster como parte del enfoque "Cualquier sistema operativo, cualquier nube" con Service Fabric. Este tutorial muestra cómo crear la infraestructura de AWS necesaria para hospedar el clúster independiente.

En la tercera parte de la serie, se aprende a:

> [!div class="checklist"]
> * Descargar la aplicación de ejemplo
> * Implementar en el clúster

## <a name="prerequisites"></a>Prerequisites

Antes de empezar este tutorial:

* [Instale Visual Studio 2019](https://www.visualstudio.com/) y las cargas de trabajo de **desarrollo de Azure** y de **desarrollo web y de ASP.NET**.
* [Instale el SDK de Service Fabric](service-fabric-get-started.md)

## <a name="download-the-voting-sample-application"></a>Descarga de la aplicación de ejemplo de votación

En una ventana Comandos, ejecute el comando siguiente para clonar el repositorio de la aplicación de ejemplo en la máquina local.

```
git clone https://github.com/Azure-Samples/service-fabric-dotnet-quickstart
```

### <a name="deploy-the-app-to-the-service-fabric-cluster"></a>Implementación de la aplicación en el clúster de Service Fabric

Una vez descargada la aplicación, puede implementarla en un clúster directamente desde Visual Studio.

1. Abra Visual Studio.

2. Seleccione **Archivo** > **Abrir**

3. Vaya a la carpeta donde clonó el repositorio de git y seleccione Voting.sln

4. Haga clic con el botón derecho en el proyecto de aplicación `Voting` en el Explorador de soluciones y elija **Publicar**

5. Seleccione el **Punto de conexión** en la lista desplegable y escriba el nombre DNS público de uno de los nodos del clúster.  Por ejemplo, `ec2-34-215-183-77.us-west-2.compute.amazonaws.com:19000`. Tenga en cuenta que, en Azure, no se establece un nombre de dominio completo (FQDN) automáticamente, pero [se puede establecer fácilmente en la página Información general de VM](../virtual-machines/linux/portal-create-fqdn.md).

6. Abra su explorador preferido y escriba la dirección del clúster (el punto de conexión, esta aplicación implementa en el puerto 8080, por ejemplo, ec2-34-215-183-77.us-west-2.compute.amazonaws.com:8080).

    ![Respuesta de API desde el clúster](./media/service-fabric-tutorial-standalone-cluster/deployed-app.png)

## <a name="next-steps"></a>Pasos siguientes

En la tercera parte de la serie aprendió a implementar una aplicación en el clúster:

> [!div class="checklist"]
> * Descargar la aplicación de ejemplo
> * Implementar en el clúster

Avance a la cuarta parte para aprender a limpiar el clúster.

> [!div class="nextstepaction"]
> [Limpieza de los recursos](service-fabric-tutorial-standalone-clean-up.md)
