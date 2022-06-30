---
title: GPO-Bereitstellung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004400"
- "8602"
ms.date: 02/24/2021
ms.openlocfilehash: 7722dbd2a93d999e77af8e56fb084be7aa52b80c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66376692"
---
# <a name="gpo-deployment"></a>GPO-Bereitstellung

Einstellungen für Benutzer- und Computerobjekte in Azure Active Directory Domain Services (Azure AD DS) werden häufig mit Gruppenrichtlinienobjekten (GPOs) verwaltet. Azure AD DS enthält integrierte GPOs für die Container "AADDC-Benutzer" und "AADDC-Computer". Sie können diese integrierten Gruppenrichtlinienobjekte anpassen, um Gruppenrichtlinien nach Bedarf für Ihre Umgebung zu konfigurieren. Mitglieder der Gruppe der Azure AD DC-Administratoren verfügen in der Azure AD DS-Domäne über Administratorrechte für Gruppenrichtlinien und können auch benutzerdefinierte Gruppenrichtlinienobjekte und Organisationseinheiten erstellen. Weitere Informationen zur Gruppenrichtlinie und deren Funktionsweise finden Sie [unter Gruppenrichtlinie Übersicht](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

In einer Hybridumgebung werden in einer lokalen AD DS-Umgebung konfigurierte Gruppenrichtlinien nicht mit Azure AD DS synchronisiert. Um Konfigurationseinstellungen für Benutzer oder Computer in Azure AD DS zu definieren, bearbeiten Sie eines der Standardrichtlinienobjekte, oder erstellen Sie ein benutzerdefiniertes Gruppenrichtlinienobjekt.

In diesem Artikel, [Verwalten von Gruppenrichtlinienrichtlinien](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) wird gezeigt, wie Sie die Tools für die Gruppenrichtlinienverwaltung installieren, die integrierten Gruppenrichtlinienobjekte bearbeiten und wie benutzerdefinierte Gruppenrichtlinienobjekte erstellt werden.
