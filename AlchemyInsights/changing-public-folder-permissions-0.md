---
title: Ändern von Berechtigungen für öffentliche Ordner
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3500007"
- "633"
ms.date: 01/21/2022
ms.openlocfilehash: 21cfa84519182cbf10913a790ed5897b81aab847
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66519564"
---
# <a name="changing-public-folder-permissions"></a>Ändern von Berechtigungen für öffentliche Ordner

Berechtigungen für öffentliche Ordner können von Benutzern und Administratoren in Outlook geändert werden. Administratoren können berechtigungen auch über das Exchange Admin Center (EAC) steuern, indem sie folgendermaßen vorgehen:
  
1. Wechseln Sie in der Microsoft 365 Admin Center zu **Admin Center** \> [**Exchange**](https://admin.exchange.microsoft.com/#/homepage).
2. Wählen Sie **öffentliche Ordner aus**.
3. Von dort aus können Sie Berechtigungen für einzelne öffentliche Ordner ändern, indem Sie Berechtigungen Sicherheitsgruppen zuweisen. Damit ein Endbenutzer Berechtigungen für öffentliche Ordner ändern kann, muss der Benutzer über Besitzerberechtigungen für den Ordner verfügen.

Führen Sie das unter "So wird's gemacht" beschriebene Verfahren aus, [um Probleme mit öffentlichen Ordnerberechtigungen zu diagnostizieren und zu beheben](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) .

**Hinweis**: Es gibt mehrere bekannte Probleme, die auftreten können, wenn Sie versuchen, Berechtigungen für öffentliche Ordner zu ändern. Weitere Informationen finden Sie in den folgenden Artikeln.

- [Berechtigungen und Einstellungen für öffentliche Ordner werden im EAC nicht weitergegeben](https://aka.ms/pfeac)
- [Fehler "Das Postfach wurde in der lokalen Gesamtstruktur nicht gefunden", wenn Sie auf öffentliche Ordner zugreifen](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
