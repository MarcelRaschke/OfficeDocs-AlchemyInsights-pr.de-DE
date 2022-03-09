---
title: Der Fehler „Die zugrunde liegende Verbindung wurde geschlossen“ in SharePoint
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 65ca6bddd2b7f2f74f55c09541a3cecfcfa6e5a9
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63257741"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Fehler "Die zugrunde liegende Verbindung wurde geschlossen" in SharePoint

Wenn in SharePoint die Fehlermeldung „Die zugrunde liegende Verbindung wurde geschlossen“ angezeigt wird, könnte dies mit dem Ende von TLS 1.0/1.1 zusammenhängen. Weitere Informationen finden Sie in den folgenden Artikeln:

- [Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Authentifizierungsfehler treten auf, wenn der Client keine TLS 1.2-Unterstützung hat](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Wenn Benutzer Windows 7 verwenden, sollten sie unbedingt [TLS-Verschlüsselungssammlungen in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7) überprüfen.