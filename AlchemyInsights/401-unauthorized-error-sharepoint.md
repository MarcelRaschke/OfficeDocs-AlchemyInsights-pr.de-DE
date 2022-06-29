---
title: „401 Nicht autorisiert“-Fehler in SharePoint
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9001435"
- "10935"
ms.date: 04/14/2021
ms.openlocfilehash: 26037b6b87aa91814d29e622e7a185e6154e8e80
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66289774"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>„401 Nicht autorisiert“-Fehler in SharePoint

Wenn Sie in SharePoint die Fehlermeldung „(401) Nicht autorisiert“ erhalten, kann dies mit der veralteten TLS-Version 1.0/1.1 zusammenhängen. Weitere Informationen finden Sie unter:

- [Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Authentifizierungsfehler treten auf, wenn der Client keine TLS 1.2-Unterstützung hat](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Wenn Benutzer Windows 7 verwenden, sollten sie unbedingt [TLS-Verschlüsselungssammlungen in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7) überprüfen.