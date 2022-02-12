---
title: Leistungsprobleme SharePoint oder OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 9d882e5819e33a3d2eb028cef33f60eba0457477
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62572599"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint oder OneDrive langsam, nicht zugänglich oder für mehrere Benutzer nicht verfügbar

SharePoint oder OneDrive können aus verschiedenen Gründen langsam, unzugänglich oder nicht verfügbar sein oder Dienstfehler oder 503-Fehler anzeigen:
  
- Wenn Ihre SharePoint oder OneDrive Website für mehrere Benutzer langsam oder verzögert ist, kann es zu einem temporären Dienstproblem kommen, bei dem Benutzer beim Zugriff auf SharePoint Websites oder OneDrive Inhalte zeitweilige Verzögerungen oder Navigationsfehler feststellen. Schauen Sie im [Dienststatus-Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) nach, ob Ihre Organisation davon betroffen ist.
  
- Benutzer erhalten möglicherweise einen *503-Server ist ausgelastet*, wenn sie versuchen, zu SharePoint oder OneDrive Websites zu navigieren. Dieser Fehler kann durch Drosselung innerhalb des SharePoint Diensts verursacht werden. SharePoint Online verwendet Einschränkung, um eine optimale Leistung und Zuverlässigkeit des Diensts SharePoint Online verwalten. Drosselung schränkt die Anzahl von Benutzeraktionen oder gleichzeitige Aufrufe (durch Code oder Skripts), um die Überlastung von Ressourcen zu verhindern. Weitere Informationen zur Drosselung finden Sie unter ["Vermeiden von Einschränkungen oder Sperren in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)".

- Wenn bei einer **klassischen** oder **modernen** SharePoint Website oder Seite eine langsame Leistung auftritt, verwenden Sie das [Seitendiagnosetool](https://aka.ms/perftool), um die Seiten zu analysieren.
  
- Wenn die Leistung weiterhin allgemein langsam ist, lesen Sie die Ressourcen unten in diesem Artikel: [Einführung in die Leistungsoptimierung für SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  