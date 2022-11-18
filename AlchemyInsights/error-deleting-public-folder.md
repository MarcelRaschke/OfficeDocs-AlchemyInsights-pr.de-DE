---
title: Fehler beim Löschen des Postfachs für öffentliche Ordner
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3500007"
- "16803"
ms.date: 02/25/2022
ms.openlocfilehash: a40ee4f84722a7d8dd45f544720ae512f9dd799b
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63309261"
---
# <a name="error-when-deleting-public-folder-mailbox"></a>Fehler beim Löschen des Postfachs für öffentliche Ordner

Möglicherweise versuchen Sie, alle Postfächer für öffentliche Ordner zu entfernen und die Fehlermeldung "Das Postfach \<mailboxname\> ist das primäre Postfach für öffentliche Ordner für die Benutzer. Um dieses Postfach zu entfernen, entfernen Sie zuerst alle anderen Postfächer für öffentliche Ordner."  

Dieser Fehler tritt auf, wenn ein Konfliktobjekt (CNF) in Ihrem Mandanten vorhanden ist. Schritte zum Suchen und Entfernen des CNF-Objekts und zum Entfernen der Postfächer für öffentliche Ordner finden Sie [unter Fehler während einer Migration öffentlicher Ordner](https://aka.ms/PFCNF).
