---
title: Skripts für öffentliche Ordner schlagen fehl, fehler beim Zugriff verweigert
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
- "17155"
ms.date: 04/12/2022
ms.openlocfilehash: d806846535cca6570020404792990efeb37c5c90
ms.sourcegitcommit: b6ba43b438551e7558ad67d8b94f84b608d26bf9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/13/2022
ms.locfileid: "64826496"
---
# <a name="public-folder-scripts-fail-with-access-denied-error"></a>Skripts für öffentliche Ordner schlagen fehl, fehler beim Zugriff verweigert

Derzeit unterstützen Skripts für öffentliche Ordner, die E-Mail-aktivierte öffentliche Ordner (MEPF) synchronisieren, um Exchange Online nur die Standardauthentifizierung zu unterstützen. Wenn die Standardauthentifizierung für das Remote-PowerShell-Protokoll und das im Skript bereitgestellte Administratorkonto deaktiviert ist, schlägt die Skriptausführung fehl.

Lösung:

1. Diag ausführen [: Aktivieren Sie die Standardauthentifizierung in EXO](https://aka.ms/PillarEXOBasicAuth), um zu überprüfen, ob die Standardauthentifizierung für das Remote-PowerShell-Protokoll deaktiviert ist, und aktivieren Sie die Standardauthentifizierung für das Remote-PowerShell-Protokoll.
2. Wenn Sie die Standardauthentifizierung für das Administratorkonto deaktiviert haben, aktivieren Sie die Standardauthentifizierung für das Administratorkonto, das im Skript verwendet wird, bis die Ausführung des Skripts erforderlich ist.
