---
title: 932 Upgrade von AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 2daa1b17180e6ae8df097be7fa2597e6026c3983
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63220281"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade Azure AD Verbinden

Standardmäßig ist das automatische Upgrade für Azure AD Verbinden aktiviert, wodurch sichergestellt wird, dass Sie die neueste Version ausführen. Um die Einstellungen für automatische Upgrades zu überprüfen, verwenden Sie das Cmdlet **"Get-ADSyncAutoUpgrade**" in Azure AD PowerShell. Das Cmdlet gibt einen der folgenden Werte zurück:

- **Aktiviert**: Das automatische Upgrade ist aktiviert.

- **Deaktiviert**: Das automatische Upgrade ist deaktiviert.

- **Angehalten**: Das System ist nicht mehr berechtigt, automatische Upgrades zu erhalten. Sie können diesen Wert nicht konfigurieren. sie wird vom System festgelegt.

Weitere Informationen finden Sie unter ["Automatisches Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)".

Um die neueste Version von Azure AD Verbinden herunterzuladen, wechseln Sie zu [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
