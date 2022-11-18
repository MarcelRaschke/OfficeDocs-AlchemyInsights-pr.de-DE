---
title: 932 Aktualisieren von AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1300025"
- "932"
ms.date: 04/21/2020
ms.openlocfilehash: e5b9c48a082c032e2bb5f58a0cabb3ef5d543dc0
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66510078"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade Azure AD Connect

Standardmäßig ist das automatische Upgrade für Azure AD Connect aktiviert, wodurch sichergestellt wird, dass Sie die neueste Version ausführen. Verwenden Sie zum Überprüfen der Einstellungen für automatische Upgrades das Cmdlet **"Get-ADSyncAutoUpgrade** " in Azure AD PowerShell. Das Cmdlet gibt einen der folgenden Werte zurück:

- **Aktiviert**: Automatisches Upgrade ist aktiviert.

- **Deaktiviert**: Das automatische Upgrade ist deaktiviert.

- **Angehalten**: Das System ist nicht mehr berechtigt, automatische Upgrades zu erhalten. Sie können diesen Wert nicht konfigurieren. sie wird vom System festgelegt.

Weitere Informationen finden Sie unter [Automatisches Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Um die neueste Version von Azure AD Connect herunterzuladen, wechseln Sie zu [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
