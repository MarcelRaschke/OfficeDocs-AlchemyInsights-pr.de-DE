---
title: Beheben häufiger Probleme mit der DKIM-Datensatzformatierung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002531"
- "7375"
ms.date: 02/23/2021
ms.openlocfilehash: 3338105f77d03fb4f32f9d1f3d89064953fd6aaa
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66272764"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Beheben häufiger Probleme mit der DKIM-Datensatzformatierung

Die meisten DKIM-Setupprobleme beziehen sich auf falsche DNS-Einträge.

Um die DKIM-Setupprobleme zu beheben, überprüfen Sie, ob der DKIM CNAME-Eintrag (**kein** TXT-Eintrag) richtig formatiert ist. Weitere Informationen finden Sie unter [Vorgehensweisen zum manuellen Einrichten von DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Wenn Sie im Allgemeinen Hilfe zu DNS-Einträgen benötigen, lesen [Sie "Erstellen von DNS-Einträgen bei einem beliebigen DNS-Hostinganbieter für Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)".

**Hinweis**: Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne erstellt oder aktualisiert haben, müssen Sie warten, bis die DNS-Einträge verteilt werden.
