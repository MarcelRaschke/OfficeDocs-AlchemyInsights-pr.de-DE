---
title: Kalendersymbol wird im Teams-Client nicht angezeigt
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989590"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalendersymbol wird im Teams-Client nicht angezeigt

Die Registerkarte „Kalender“ in Teams muss über Exchange-Webdienste auf ein Exchange-Postfach zugreifen können. Das Exchange-Postfach kann online oder lokal sein. Vergewissern Sie sich für Onlinebenutzer, für die die Registerkarte „Kalender“ nicht angezeigt wird, dass [ sie für ein Exchange Online-Postfach lizenziert sind und das Postfach aktiviert](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) ist.

Wenn der Benutzer über ein gültiges Postfach in Exchange Online verfügt, die Registerkarte „Kalender“ aber immer noch nicht angezeigt wird, tritt möglicherweise ein Netzwerkproblem auf. Verwenden Sie die [Microsoft-Remoteverbindungsuntersuchung](https://testconnectivity.microsoft.com/), und führen Sie die **Verbindungstests für Microsoft Exchange-Webdienste** für den betroffenen Benutzer durch.

Überprüfen Sie schließlich die [Teams-Apps –-App-Setup-Richtlinien](https://admin.teams.microsoft.com/policies/app-setup), um sicherzustellen, dass die Kalender-App nicht aus der auf den Benutzer angewendeten Richtlinie entfernt wurde (höchstwahrscheinlich die globale Richtlinie (organisationsweiter Standard).

Wenn Ihre Benutzer lokal sind, müssen Sie bestätigen, dass Ihre Hybridkonfiguration fehlerfrei ist. Verwenden Sie zur Problembehandlung den [Assistenten für die Hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Beachten Sie, dass für [Teams Exchange 2016 CU3 oder höher erforderlich ist](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
