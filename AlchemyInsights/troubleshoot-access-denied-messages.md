---
title: Problembehandlung bei Nachrichten mit verweigertem Zugriff
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: da8fbc58ec8d0dd2b65e531da18e639269541c84
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65591850"
---
# <a name="troubleshoot-access-denied-messages"></a>Problembehandlung bei Nachrichten mit verweigertem Zugriff

Wenn jemand eine Meldung "Zugriff verweigert" für einen freigegebenen Ordner in SharePoint erhalten hat, hat der Websitesammlungsadministrator möglicherweise "Sperrmodus für Benutzerberechtigungen mit eingeschränktem Zugriff" aktiviert. So deaktivieren Sie dies: 
  
1. Navigieren Sie zur Website, klicken Sie auf das Symbol Einstellungen, und klicken Sie dann auf **"Website Einstellungen**".
    
2. Klicken Sie unter **Websitesammlungsverwaltung** auf **Websitesammlungsfeatures**.
    
3. Klicken Sie neben dem **Sperrmodus für Benutzerberechtigungen mit eingeschränktem Zugriff** auf **"Deaktivieren**".
    
Eine Meldung "Zugriff verweigert" kann auch für freigegebene Ordner auftreten, wenn es sich bei der Website um eine Veröffentlichungswebsite handelt. Weitere Informationen finden Sie unter [Zugriff verweigert beim Zugriff auf einen freigegebenen Ordner](https://answers.microsoft.com/en-us/windows/forum/all/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).
  
Wenn eine Person beim Versuch, Zugriffsanforderungen anzuzeigen, die Meldung "Zugriff verweigert" erhalten hat, muss der Benutzer entweder als Websitesammlungsadministrator oder als Mitglied der Gruppe "Besitzer" für die Website hinzugefügt werden. Weitere Informationen finden Sie in der [Liste "Zugriffsanforderungen verweigert](https://go.microsoft.com/fwlink/?linkid=2004220)".
  
Wenn ein Benutzer die Meldung "Zugriff verweigert" erhalten hat, nachdem er lokal aus Active Directory entfernt und dann wieder hinzugefügt wurde, lesen Sie ["Zugriff verweigert", wenn ein Benutzerkonto mit Microsoft 365 synchronisiert wird](https://go.microsoft.com/fwlink/?linkid=2004318).
  

