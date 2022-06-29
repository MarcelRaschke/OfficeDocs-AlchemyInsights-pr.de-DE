---
title: 902 (Synchronisierungsfehler aufgrund doppelter Objekte)
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 902
ms.date: 04/21/2020
ms.openlocfilehash: 1e3b89a3706fa3ed79a61722e0b4bf28a55bcf96
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66416830"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synchronisierungsfehler aufgrund doppelter Objekte

Möglicherweise wird eine der folgenden Fehlermeldungen angezeigt, wenn die Verzeichnissynchronisierung in Microsoft 365 abgeschlossen ist:

- Dieses Objekt kann in Microsoft Online Services nicht aktualisiert werden, da die folgenden diesem Objekt zugeordneten Attribute Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnis zugeordnet sind.

- Ein synchronisiertes Objekt mit derselben Proxyadresse ist bereits in Ihrem Microsoft Online Services-Verzeichnis vorhanden.

- Dieses Objekt kann nicht aktualisiert werden, da die folgenden diesem Objekt zugeordneten Attribute Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Den lokalen Verzeichnisdiensten zugeordnet sind: UserPrincipalName.

Um das Problem zu identifizieren und zu beheben, laden Sie das [IdFix DirSync-Fehlerbehebungstool](https://github.com/Microsoft/idfix) herunter, und führen Sie es aus.

Weitere Informationen finden Sie [unter KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
