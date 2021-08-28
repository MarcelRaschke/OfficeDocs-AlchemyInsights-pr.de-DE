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
ms.openlocfilehash: 5bccaedda08e2c948a15c0b32c6f6eeecfc8bd4c4555b25291f294fe5deb3019
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088791"
---
# <a name="group-policy"></a>Gruppenrichtlinie

Einstellungen für Benutzer- und Computerobjekte in Azure Active Directory Domain Services (Azure AD DS) werden häufig mit Gruppenrichtlinienobjekten (GPOs) verwaltet. Azure AD DS enthält integrierte GPOs für die Container "AADDC-Benutzer" und "AADDC-Computer". Sie können diese integrierten Gruppenrichtlinienobjekte anpassen, um Gruppenrichtlinien nach Bedarf für Ihre Umgebung zu konfigurieren. Mitglieder der Gruppe der Azure AD DC-Administratoren verfügen in der Azure AD DS-Domäne über Administratorrechte für Gruppenrichtlinien und können auch benutzerdefinierte Gruppenrichtlinienobjekte und Organisationseinheiten erstellen. Weitere Informationen darüber, was eine Gruppenrichtlinie ist und wie sie funktioniert, finden Sie unter [Gruppenrichtlinienübersicht](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

In einer Hybridumgebung werden in einer lokalen AD DS-Umgebung konfigurierte Gruppenrichtlinien nicht mit Azure AD DS synchronisiert. Um Konfigurationseinstellungen für Benutzer oder Computer in Azure AD DS zu definieren, bearbeiten Sie eines der Standardrichtlinienobjekte, oder erstellen Sie ein benutzerdefiniertes Gruppenrichtlinienobjekt.

In diesem Artikel, [Verwalten von Gruppenrichtlinienrichtlinien](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) wird gezeigt, wie Sie die Tools für die Gruppenrichtlinienverwaltung installieren, die integrierten Gruppenrichtlinienobjekte bearbeiten und wie benutzerdefinierte Gruppenrichtlinienobjekte erstellt werden.



