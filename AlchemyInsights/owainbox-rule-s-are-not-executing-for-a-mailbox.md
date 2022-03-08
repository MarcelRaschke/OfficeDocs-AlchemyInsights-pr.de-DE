---
title: 1332 OWA – Posteingangsregel(n) werden für ein Postfach nicht ausgeführt
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
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 5596b1933e393f99a0cdbc87a3428417aab6d9da
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63213909"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Eine Posteingangsregel funktioniert nicht wie erwartet

Überprüfen Sie die folgenden Einstellungen in Outlook im Web:

- Eine Nachricht kann nur einmal basierend auf Posteingangsregeln umgeleitet, weitergeleitet oder beantwortet werden. Eine Umleitungsregel (eine Posteingangsregel oder Nachrichtenflussregel, auch als Transportregel bezeichnet) kann einer Nachricht maximal zehn Weiterleitungsempfänger hinzufügen. Weitere Informationen finden Sie unter [Journal-, Transport- und Posteingangsregellimits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Posteingangsregeln funktionieren nicht für das alternative Journalpostfach. Weitere Informationen zum alternativen Journalpostfach finden Sie unter ["Alternatives Journalpostfach"](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Informationen zum Beheben dieser Probleme finden Sie unter [KB 2829319](https://support.microsoft.com/kb/2829319).

Wenn die vorherigen Probleme nicht zutreffen, führen Sie den Diagnosebericht über posteingangsregel aus, bevor Sie das Problem an den Microsoft-Support eskalieren:

1. Öffnen Sie das Postfach in Outlook im Web, und klicken Sie auf <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
  >  Einstellungen **Ansicht aller Outlook Einstellungen** >  **MailRules** > .

2. Klicken Sie unten auf der Seite auf **"Wenn Ihre Regeln nicht funktionieren", klicken Sie hier, um einen Diagnosebericht zu generieren**.
