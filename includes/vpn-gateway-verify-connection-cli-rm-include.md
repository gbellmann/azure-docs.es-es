---
title: archivo de inclusión
description: archivo de inclusión
services: vpn-gateway
author: cherylmc
ms.service: vpn-gateway
ms.topic: include
ms.date: 03/21/2018
ms.author: cherylmc
ms.custom: include file
ms.openlocfilehash: 0e009354e66ab13cdb9fbc3cf9e4b37e904bdfd1
ms.sourcegitcommit: 2ec4b3d0bad7dc0071400c2a2264399e4fe34897
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/27/2020
ms.locfileid: "67186145"
---
Puede comprobar que la conexión se realizó correctamente mediante el comando [az network vpn-connection show](/cli/azure/network/vpn-connection). En el ejemplo, " --name" hace referencia al nombre de la conexión que desea probar. Mientras la conexión aún se está estableciendo, su estado de conexión muestra "Conectando". Una vez establecida la conexión, el estado cambia a "Conectado".

```azurecli
az network vpn-connection show --name VNet1toSite2 --resource-group TestRG1
```
