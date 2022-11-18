---
title: 2419-Überwachung kann nicht aktiviert werden
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 2419
ms.date: 04/21/2020
ms.openlocfilehash: 04abbe0a1c2492f6a4122aaa61dc16f4b3b1d63d
ms.sourcegitcommit: 5058f004f549ba7ac2b4843429b385287456a9c7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061991"
---
# <a name="unable-to-enable-unified-auditing"></a>Die einheitliche Überwachung kann nicht aktiviert werden.

Wenn Sie versuchen, die einheitliche Überwachung für Ihre Organisation zu aktivieren, wird möglicherweise eine Fehlermeldung wie die folgende angezeigt:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:

1. [Verbinden, um PowerShell zu Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

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
