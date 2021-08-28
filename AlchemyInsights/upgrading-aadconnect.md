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
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104811"
---
# <a name="upgrade-azure-ad-connect"></a>Aktualisieren von Azure AD-Verbinden

Standardmäßig ist das automatische Upgrade für Azure AD Verbinden aktiviert, wodurch sichergestellt wird, dass Sie die neueste Version ausführen. Verwenden Sie zum Überprüfen der Einstellungen für automatische Upgrades das Cmdlet **"Get-ADSyncAutoUpgrade"** in Azure AD PowerShell. Das Cmdlet gibt einen der folgenden Werte zurück:

- **Aktiviert:** Das automatische Upgrade ist aktiviert.

- **Deaktiviert:** Das automatische Upgrade ist deaktiviert.

- **Angehalten:** Das System ist nicht mehr berechtigt, automatische Upgrades zu erhalten. Sie können diesen Wert nicht konfigurieren. sie wird vom System festgelegt.

Weitere Informationen finden Sie unter ["Automatisches Upgrade".](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Um die neueste Version von Azure AD Verbinden herunterzuladen, wechseln Sie zu [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
