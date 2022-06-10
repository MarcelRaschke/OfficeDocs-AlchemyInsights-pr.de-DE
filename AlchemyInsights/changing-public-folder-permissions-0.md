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
ms.openlocfilehash: 85fde7a478776fb95fbb460a2175a6d39fe62837
ms.sourcegitcommit: 5afc3c4a1270409ed3691c90ba139878d845e7a3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/10/2022
ms.locfileid: "66002888"
---
# <a name="changing-public-folder-permissions"></a>Ändern von Berechtigungen für öffentliche Ordner

Berechtigungen für öffentliche Ordner können von Benutzern und Administratoren in Outlook geändert werden. Administratoren können berechtigungen auch über das Exchange Admin Center (EAC) steuern, indem sie folgendermaßen vorgehen:
  
1. Wechseln Sie im Microsoft 365 Admin Center zu **admin center** \> [**Exchange**](https://admin.exchange.microsoft.com/#/homepage).
2. Wählen Sie **öffentliche Ordner aus**.
3. Von dort aus können Sie Berechtigungen für einzelne öffentliche Ordner ändern, indem Sie Berechtigungen Sicherheitsgruppen zuweisen. Damit ein Endbenutzer Berechtigungen für öffentliche Ordner ändern kann, muss der Benutzer über Besitzerberechtigungen für den Ordner verfügen.

Führen Sie das unter "So wird's gemacht" beschriebene Verfahren aus, [um Probleme mit öffentlichen Ordnerberechtigungen zu diagnostizieren und zu beheben](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) .

**Hinweis**: Es gibt mehrere bekannte Probleme, die auftreten können, wenn Sie versuchen, Berechtigungen für öffentliche Ordner zu ändern. Weitere Informationen finden Sie in den folgenden Artikeln.

- [Berechtigungen und Einstellungen für öffentliche Ordner werden im EAC nicht weitergegeben](https://aka.ms/pfeac)
- [Fehler "Das Postfach wurde in der lokalen Gesamtstruktur nicht gefunden", wenn Sie auf öffentliche Ordner zugreifen](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
