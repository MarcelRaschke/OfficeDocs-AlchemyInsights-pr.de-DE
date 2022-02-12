---
title: Überwachung von 2419 nicht aktivieren
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: c7b4fceeb80aa1751ae6cf2350fea3e2ba70bbd9
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62691620"
---
# <a name="unable-to-enable-unified-auditing"></a>Einheitliche Überwachung kann nicht aktiviert werden

Wenn Sie versuchen, die einheitliche Überwachung für Ihre Organisation zu aktivieren, wird möglicherweise ein Fehler wie der folgende angezeigt:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:

1. [Verbinden zu Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Führen Sie das folgende Cmdlet aus:

   ```
   Enable-OrganizationCustomization
   ```

3. Warten Sie 60 Minuten, bis die vorherige Einstellung wirksam wird.

4. Führen Sie den folgenden Befehl in Exchange Online PowerShell aus:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Weitere Informationen finden Sie in den folgenden Artikeln:

- [Verbinden mit Exchange Online PowerShell per mehrstufiger Authentifizierung](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Aktivieren oder Deaktivieren der Überwachungsprotokollsuche](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
