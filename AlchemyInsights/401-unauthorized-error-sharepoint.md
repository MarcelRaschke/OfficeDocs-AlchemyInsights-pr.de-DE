---
title: „401 Nicht autorisiert“-Fehler in SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539931"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>„401 Nicht autorisiert“-Fehler in SharePoint

Wenn Sie in SharePoint die Fehlermeldung „(401) Nicht autorisiert“ erhalten, kann dies mit der veralteten TLS-Version 1.0/1.1 zusammenhängen. Weitere Informationen finden Sie unter:

- [Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Authentifizierungsfehler treten auf, wenn der Client keine TLS 1.2-Unterstützung hat](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Wenn Benutzer Windows 7 verwenden, sollten sie unbedingt [TLS-Verschlüsselungssammlungen in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7) überprüfen.