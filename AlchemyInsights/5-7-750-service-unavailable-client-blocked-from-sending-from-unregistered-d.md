---
title: 1048 5.7.750 Dienst nicht verfügbar. Client, der am Senden von nicht registrierten Domänen gehindert wird
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 4201519d7c5cfa4d7f58ce1d91a14a74ae14dbe1
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62567273"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750 Client darf keine Mails von unregistrierter Domäne senden

Der Fehler tritt auf, wenn eine große Anzahl von Nachrichten von Domänen gesendet wird, die nicht in Ihrem Mandanten bereitgestellt werden (als akzeptierte Domänen hinzugefügt und überprüft).

Um diesen Fehler zu vermeiden, können Sie einen zertifikatbasierten Nachrichtenflussconnector verwenden, bei dem die Domäne des Zertifikats eine bereitgestellte Domäne ist, oder Sie können alle sendenden Domänen bereitstellen.

Weitere Informationen finden Sie unter [Beheben von Problemen mit der Zustellung von E-Mails bei Fehlercode 5.7.700 bis 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).