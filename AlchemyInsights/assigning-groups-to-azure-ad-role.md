---
title: Zuweisen von Gruppen zu Azure AD-Rollen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9003230"
- "7898"
ms.date: 01/15/2021
ms.openlocfilehash: 1bb4c7fd0035a45b7fd1a965c34711b4ca9697fd
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66299872"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Zuweisen von Gruppen zu Azure AD-Rollen

Um eine Azure AD-Gruppe mit Autoritätsquelle in Azure AD zu einer Azure AD-Rolle zuzuweisen, führen Sie die folgenden Schritte aus:

1. Erstellen Sie eine neue Gruppe – Um eine neue Gruppe zu erstellen:

    a. Melden Sie sich im Azure AD-Admin Center mit Berechtigungen für einen **Administrator für privilegierte Rollen** oder für einen **globalen Administrator** an.
    b. Wählen Sie **Azure Active Directory > Gruppen > Alle Gruppen > Neue Gruppe** aus.
    c. Erstellen Sie die Gruppe.

2. Weisen Sie der Gruppe die Rolle zu, entweder während der Erstellung der Gruppe oder nachdem die Gruppe erstellt wurde.

    a. Um der Gruppe eine Rolle zum Zeitpunkt der Gruppenerstellung zuzuweisen, aktivieren Sie die Umschaltfläche **Azure AD-Rollen können der Gruppe zugewiesen werden** und erstellen Sie die Gruppe.
    b. Um der Gruppe eine Rolle zuzuweisen, nachdem sie erstellt wurde, navigieren Sie zur Registerkarte **Zugewiesene Rollen** für die neu erstellte Gruppe und weisen Sie der Gruppe die Rolle zu.  

**Verwalten Sie die Mitgliedschaft in einer Gruppe, der eine Azure AD-Rolle** zugewiesen wurde.

Um eine standardmäßige Erhöhung von Rechten zu verhindern, können nur Administratoren für privilegierte Rollen und globale Administratoren die Mitgliedschaft einer Gruppe ändern, der eine Rolle zugewiesen wurde. Sie können jedoch auswählen, ob Sie einen Besitzer für eine solche Gruppe auswählen möchten und diese Aufgabe delegieren.

Weitere Details darüber, wie Cloudgruppen zu Azure AD-Rollen zugewiesen werden, finden Sie unter [Zuweisen von AD-Rollen für Cloudgruppen](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Weitere Details über Problembehandlung von Rollen, die Cloudgruppen zugewiesen werden, finden Sie unter [Problembehandlung von Rollen, die Cloudgruppen zugewiesen wurden](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





