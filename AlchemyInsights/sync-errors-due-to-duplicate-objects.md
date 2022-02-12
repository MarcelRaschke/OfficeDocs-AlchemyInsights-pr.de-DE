---
title: 902 (Synchronisierungsfehler aufgrund doppelter Objekte)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 922826d9e438ac1ffc01279c7fa15087a9aad2d2
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62661990"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synchronisierungsfehler aufgrund doppelter Objekte

Möglicherweise wird eine der folgenden Fehlermeldungen angezeigt, wenn die Verzeichnissynchronisierung in Microsoft 365 abgeschlossen ist:

- Dieses Objekt kann in Microsoft Online Services nicht aktualisiert werden, da die folgenden diesem Objekt zugeordneten Attribute Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnis zugeordnet sind.

- In Ihrem Microsoft Online Services-Verzeichnis ist bereits ein synchronisiertes Objekt mit derselben Proxyadresse vorhanden.

- Dieses Objekt kann nicht aktualisiert werden, da die folgenden diesem Objekt zugeordneten Attribute Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Ihren lokalen Verzeichnisdiensten zugeordnet sind: UserPrincipalName.

Laden Sie das [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix) herunter, und führen Sie es aus, um das Problem zu identifizieren und zu beheben.

Weitere Informationen finden Sie unter [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
