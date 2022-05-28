---
title: 932 Aktualisieren von AADConnect
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
ms.openlocfilehash: 4ce8b6de8f36e4f3ae1c8c66010400db5accd3b4
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65718189"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD-Verbinden aktualisieren

Standardmäßig ist das automatische Upgrade für Azure AD Verbinden aktiviert, wodurch sichergestellt wird, dass Sie die neueste Version ausführen. Verwenden Sie zum Überprüfen der Einstellungen für automatische Upgrades das Cmdlet **"Get-ADSyncAutoUpgrade** " in Azure AD PowerShell. Das Cmdlet gibt einen der folgenden Werte zurück:

- **Aktiviert**: Automatisches Upgrade ist aktiviert.

- **Deaktiviert**: Das automatische Upgrade ist deaktiviert.

- **Angehalten**: Das System ist nicht mehr berechtigt, automatische Upgrades zu erhalten. Sie können diesen Wert nicht konfigurieren. sie wird vom System festgelegt.

Weitere Informationen finden Sie unter [Automatisches Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Um die neueste Version von Azure AD Verbinden herunterzuladen, wechseln Sie zu [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
