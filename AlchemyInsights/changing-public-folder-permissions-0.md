---
title: Ändern von Berechtigungen für öffentliche Ordner
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: b8dc168526494d0c83aec170ef5f46ad29612dd7
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61963999"
---
# <a name="changing-public-folder-permissions"></a>Ändern von Berechtigungen für öffentliche Ordner

Berechtigungen für öffentliche Ordner können von Benutzern und Administratoren in Outlook geändert werden. Administratoren können berechtigungen auch über das Exchange Admin Center (EAC) steuern, indem sie folgendermaßen vorgehen:
  
1. Wechseln Sie im Microsoft 365 Admin Center zu **Admin Center** \> **Exchange**.

2. Wählen Sie **öffentliche Ordner aus.**

3. Von dort aus können Sie Berechtigungen für einzelne öffentliche Ordner ändern, indem Sie Sicherheitsgruppen Berechtigungen zuweisen. Damit ein Endbenutzer Berechtigungen für öffentliche Ordner ändern kann, muss der Benutzer über Besitzerrechte für den Ordner verfügen.

Befolgen Sie das unter ["Diagnostizieren und Beheben von Berechtigungsproblemen bei öffentlichen Ordnern"](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) beschriebene Verfahren, um Probleme mit berechtigungen für öffentliche Ordner zu beheben.

**Hinweis:** Es gibt mehrere bekannte Probleme, die auftreten können, wenn Sie versuchen, Berechtigungen für öffentliche Ordner zu ändern. Weitere Informationen finden Sie in den folgenden Artikeln.

- [Berechtigungen können nicht auf Unterordner für öffentliche Ordner in EAC angewendet werden](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [Fehler "Das Postfach wird in der lokalen Gesamtstruktur nicht gefunden" beim Zugriff auf öffentliche Ordner](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
