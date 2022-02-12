---
title: Ändern von Berechtigungen für öffentliche Ordner
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.date: 01/21/2022
ms.openlocfilehash: e0ce0685ce675b8a8fb2ddc956518bf6b1b36d8f
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62673115"
---
# <a name="changing-public-folder-permissions"></a>Ändern von Berechtigungen für öffentliche Ordner

Berechtigungen für öffentliche Ordner können von Benutzern und Administratoren in Outlook geändert werden. Administratoren können berechtigungen auch über das Exchange Admin Center (EAC) steuern, indem sie folgendermaßen vorgehen:
  
1. Wechseln Sie im Microsoft 365 Admin Center zu **Admin Center** \> **Exchange**.
2. Wählen Sie **öffentliche Ordner aus**.
3. Von dort aus können Sie Berechtigungen für einzelne öffentliche Ordner ändern, indem Sie Sicherheitsgruppen Berechtigungen zuweisen. Damit ein Endbenutzer Berechtigungen für öffentliche Ordner ändern kann, muss der Benutzer über Besitzerrechte für den Ordner verfügen.

Befolgen Sie das unter ["Diagnostizieren und Beheben von Berechtigungsproblemen bei öffentlichen Ordnern](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) " beschriebene Verfahren, um Probleme mit berechtigungen für öffentliche Ordner zu beheben.

**Hinweis**: Es gibt mehrere bekannte Probleme, die auftreten können, wenn Sie versuchen, Berechtigungen für öffentliche Ordner zu ändern. Weitere Informationen finden Sie in den folgenden Artikeln.

- [Berechtigungen und Einstellungen für öffentliche Ordner werden in EAC nicht verteilt](https://aka.ms/pfeac)
- [Fehler "Das Postfach wird in der lokalen Gesamtstruktur nicht gefunden" beim Zugriff auf öffentliche Ordner](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
