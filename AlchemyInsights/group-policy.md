---
title: Gruppenrichtlinie
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: 2bc750c3262f0ff6c161f6b5849a9e9d4161a259
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62734085"
---
# <a name="group-policy"></a>Gruppenrichtlinie

Einstellungen für Benutzer- und Computerobjekte in Azure Active Directory Domain Services (Azure AD DS) werden häufig mit Gruppenrichtlinienobjekten (GPOs) verwaltet. Azure AD DS enthält integrierte GPOs für die Container "AADDC-Benutzer" und "AADDC-Computer". Sie können diese integrierten Gruppenrichtlinienobjekte anpassen, um Gruppenrichtlinien nach Bedarf für Ihre Umgebung zu konfigurieren. Mitglieder der Gruppe der Azure AD DC-Administratoren verfügen in der Azure AD DS-Domäne über Administratorrechte für Gruppenrichtlinien und können auch benutzerdefinierte Gruppenrichtlinienobjekte und Organisationseinheiten erstellen. Weitere Informationen darüber, was eine Gruppenrichtlinie ist und wie sie funktioniert, finden Sie unter [Gruppenrichtlinienübersicht](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

In einer Hybridumgebung werden in einer lokalen AD DS-Umgebung konfigurierte Gruppenrichtlinien nicht mit Azure AD DS synchronisiert. Um Konfigurationseinstellungen für Benutzer oder Computer in Azure AD DS zu definieren, bearbeiten Sie eines der Standardrichtlinienobjekte, oder erstellen Sie ein benutzerdefiniertes Gruppenrichtlinienobjekt.

In diesem Artikel, [Verwalten von Gruppenrichtlinienrichtlinien](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) wird gezeigt, wie Sie die Tools für die Gruppenrichtlinienverwaltung installieren, die integrierten Gruppenrichtlinienobjekte bearbeiten und wie benutzerdefinierte Gruppenrichtlinienobjekte erstellt werden.



