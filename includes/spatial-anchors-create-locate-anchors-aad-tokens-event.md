---
ms.openlocfilehash: 7219a457a2631f9ff6beee06eff34bce0ff5a23f
ms.sourcegitcommit: 0947111b263015136bca0e6ec5a8c570b3f700ff
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "67186017"
---
Al igual que sucede con los tokens de acceso, si no se ha establecido un token de Azure AD, debe controlar el evento TokenRequired o implementar el método tokenRequired en el protocolo de delegado.

Puede controlar el evento de forma sincrónica mediante el establecimiento de la propiedad en los argumentos del evento.
