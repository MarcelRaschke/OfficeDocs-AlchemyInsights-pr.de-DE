---
title: Beheben allgemeiner Probleme mit der DKIM-Datensatzformatierung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323989"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Beheben allgemeiner Probleme mit der DKIM-Datensatzformatierung

Die meisten PROBLEME bei der DKIM-Einrichtung beziehen sich auf falsche DNS-Einträge.

Um die PROBLEME bei der DKIM-Einrichtung zu beheben, stellen Sie sicher, dass der DKIM-CNAME-Eintrag **(kein** TXT-Eintrag) korrekt formatiert ist. Weitere Informationen finden Sie unter ["Was Sie tun müssen, um DKIM in Office 365 manuell einzurichten."](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Wenn Sie hilfe bei DNS-Einträgen im Allgemeinen benötigen, finden Sie unter [Erstellen von DNS-Einträgen bei einem beliebigen DNS-Hostinganbieter Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**Hinweis:** Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne erstellt oder aktualisiert haben, müssen Sie warten, bis die DNS-Einträge verteilt werden.
