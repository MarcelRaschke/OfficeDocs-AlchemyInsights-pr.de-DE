---
title: Bekannte Probleme mit der gruppenlosen Gruppenrichtlinie
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9010852"
- "18421"
ms.openlocfilehash: f7c01684acd091d0890f5760eef568811df819cd
ms.sourcegitcommit: cb522562d722b5fcc7dd3ae82bb0ae51ffc5ef4b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/23/2022
ms.locfileid: "67992141"
---
# <a name="known-issues-with-ownerless-group-policy"></a>Bekannte Probleme mit der gruppenlosen Gruppenrichtlinie

Es folgen bekannte Probleme mit der Gruppengovernance-Richtlinie für besitzerlose Gruppen:

- **Fehler beim Speichern der besitzerlosen Gruppenkonfiguration**

Möglicherweise wird beim Speichern der Gruppengovernancerichtlinie für besitzerlose Gruppen ein Fehler angezeigt. Die Änderungen, die Sie an der Richtlinie vornehmen, werden unabhängig von der angezeigten Fehlermeldung gespeichert. Der Fix zur Behebung dieses Problems befindet sich im Rollout.

- **Gruppenmitglieder erhalten keine E-Mail-Benachrichtigung**

Dies geschieht, wenn der in der Richtlinie konfigurierte Absender **kein** Benutzerpostfach oder Gruppenpostfach ist. Benutzerpostfach oder Gruppenpostfach sind die einzigen unterstützten Absender.

- **Die Interaktiven Schaltflächen (Ja,Nein) fehlen in der Benachrichtigungs-E-Mail**

Stellen Sie sicher, dass die primäre E-Mail-Adresse und der UPN des Absenders identisch sind, oder dass die Interaktiven Schaltflächen in Benachrichtigungs-E-Mails nicht sichtbar sind.