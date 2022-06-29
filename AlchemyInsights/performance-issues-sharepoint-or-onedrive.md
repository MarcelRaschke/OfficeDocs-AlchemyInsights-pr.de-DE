---
title: Leistungsprobleme – SharePoint oder OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "5200018"
- "1133"
- "2397"
- "2418"
ms.openlocfilehash: 07d708071f1d4b58985ded72186c3273e84e2372
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66255934"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint oder OneDrive langsam, nicht zugänglich oder für mehrere Benutzer nicht verfügbar

SharePoint oder OneDrive ist möglicherweise langsam, nicht zugänglich oder nicht verfügbar, oder der Dienst ist aus mehreren Gründen nicht verfügbar oder 503 Fehler:
  
- Wenn Ihre SharePoint- oder OneDrive-Website für mehrere Benutzer langsam oder verzögert ist, kann es ein temporäres Dienstproblem geben, bei dem Benutzer beim Zugriff auf SharePoint-Websites oder OneDrive-Inhalte zeitweilig zu Verzögerungen oder Navigationsfehlern kommen. Schauen Sie im [Dienststatus-Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) nach, ob Ihre Organisation davon betroffen ist.
  
- Benutzer erhalten möglicherweise einen *Fehler "503 Server ist ausgelastet* ", wenn sie versuchen, zu SharePoint- oder OneDrive-Websites zu navigieren. Dieser Fehler kann durch Drosselung innerhalb des SharePoint-Diensts verursacht werden. SharePoint Online verwendet Einschränkung, um eine optimale Leistung und Zuverlässigkeit des Diensts SharePoint Online verwalten. Drosselung schränkt die Anzahl von Benutzeraktionen oder gleichzeitige Aufrufe (durch Code oder Skripts), um die Überlastung von Ressourcen zu verhindern. Weitere Informationen zur Drosselung finden Sie unter: [Vermeiden Sie es, in SharePoint Online gedrosselt oder blockiert zu werden](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Wenn Bei einer **klassischen** oder **modernen** SharePoint-Website oder -Seite eine langsame Leistung auftritt, verwenden Sie das [Seitendiagnosetool](https://aka.ms/perftool) , um die Seiten zu analysieren.
  
- Wenn sie immer noch eine allgemeine, langsame Leistung haben, lesen Sie bitte die Ressourcen am Ende dieses Artikels: [Einführung in die Leistungsoptimierung für SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  