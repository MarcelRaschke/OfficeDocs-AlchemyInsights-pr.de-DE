---
title: SCIM-Bereitstellungsprobleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: 78cc48ac4c2c15f16ee818226f7288d47bf5334e
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62693888"
---
# <a name="scim-provisioning-issue"></a>SCIM-Bereitstellungsprobleme

Bei der automatischen Bereitstellung werden Benutzeridentitäten und Rollen in Cloud-Anwendungen erstellt, auf die Benutzer Zugriff erhalten müssen. Zusätzlich zu der Erstellung von Benutzeridentitäten schließt die automatische Bereitstellung auch die Wartung und Entfernung von Benutzeridentitäten ein, wenn sich deren Status oder Rolle ändert. Vor der Bereitstellung können Sie sich [So funktioniert die Bereitstellung](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) durchlesen, um zu erfahren, wie die Bereitstellung in Azure Active Directory (AD) funktioniert, und um Empfehlungen für die Konfiguration zu erhalten.

Als Anwendungsentwickler können Sie die System for Cross-Domain Identity Management (SCIM)-API für die Benutzerverwaltung verwenden, um die automatische Bereitstellung von Benutzern und Gruppen zwischen Ihrer Anwendung und Azure AD zu aktivieren. In dem Artikel [Erstellen eines SCIM-Endpunkts und Konfigurieren der Benutzerbereitstellung mit Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) wird beschrieben, wie ein SCIM-Endpunkt erstellt und mit dem Bereitstellungsdienst in Azure Ad integriert wird.



