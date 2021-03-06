---
author: tfitzmac
ms.service: azure-resource-manager
ms.topic: include
ms.date: 02/24/2020
ms.author: tomfitz
ms.openlocfilehash: 33a63280f6973d2c5e29db29f7a6f3fc68c57c77
ms.sourcegitcommit: 877491bd46921c11dd478bd25fc718ceee2dcc08
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/02/2020
ms.locfileid: "84424770"
---
| Recurso | Límite |
| --- | --- |
| Recursos por [grupo de recursos](../articles/azure-resource-manager/management/overview.md#resource-groups) | Los recursos no están limitados por el grupo de recursos. En su lugar, están limitados por el tipo de recurso de un grupo de recursos. Consulte la fila siguiente. |
| Recursos por grupo de recursos, por tipo de recurso |800: algunos tipos de recursos pueden superar el límite de 800. Consulte [Resources not limited to 800 instances per resource group](../articles/azure-resource-manager/management/resources-without-resource-group-limit.md) (Recursos no limitados a 800 instancias por grupo de recursos). |
| Implementaciones por grupo de recursos en el historial de implementaciones |800<sup>1</sup> |
| Recursos por implementación |800 |
| Bloqueos de administración por ámbito único |20 |
| Número de etiquetas por recurso o grupo de recursos |50 |
| Longitud de la clave de etiqueta |512 |
| Longitud del valor de la etiqueta |256 |

<sup>1</sup>A partir de junio 2020, las implementaciones se eliminarán automáticamente del historial cuando se aproxime al límite. Eliminar una entrada del historial de implementaciones no afecta a los recursos implementados. Para obtener más información, consulte [Eliminaciones automáticas del historial de implementaciones](../articles/azure-resource-manager/templates/deployment-history-deletions.md).

#### <a name="template-limits"></a>Límites de plantilla

| Value | Límite |
| --- | --- |
| Parámetros |256 |
| variables |256 |
| Recursos (incluido el recuento de copia) |800 |
| Salidas |64 |
| Expresión de plantilla |24 576 caracteres |
| Recursos de plantillas exportadas |200 |
| Tamaño de la plantilla |4 MB |
| Tamaño del archivo de parámetros |64 KB |

Puede superar algunos límites de plantilla utilizando una plantilla anidada. Para más información, consulte [Uso de plantillas vinculadas al implementar recursos de Azure](../articles/azure-resource-manager/templates/linked-templates.md). Para reducir el número de parámetros, variables o salidas, puede combinar varios valores en un objeto. Para más información, consulte [Objetos como parámetros](../articles/azure-resource-manager/resource-manager-objects-as-parameters.md).
