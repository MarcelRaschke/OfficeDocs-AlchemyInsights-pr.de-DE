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
ms.localizationpriority: medium
ms.custom:
- "633"
- "3500007"
ms.date: 01/21/2022
ms.openlocfilehash: 3637f7bcf18f7ad722908c2db438947b370ae724
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63241649"
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
