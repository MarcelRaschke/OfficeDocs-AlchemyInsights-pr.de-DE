---
title: Erstellen einer Gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929304"
---
# <a name="create-a-group"></a>Erstellen einer Gruppe

In diesem Thema wird die Gruppenerstellung beschrieben.

**Berechtigung zum Erstellen einer Gruppe**

Stellen Sie sicher, dass Sie berechtigt sind, eine neue Gruppe zu erstellen. Globale Administratoren können die Gruppenerstellung im Microsoft Azure-Portal oder im Access Panel deaktivieren. Möglicherweise benötigen Sie einen Administrator, um die neue Gruppe für Sie zu erstellen oder Ihnen die entsprechenden Berechtigungen zu erteilen.

**Verwalten von Gruppenerstellungsberechtigungen**

1. Globale Administratoren können Gruppenerstellungsberechtigungen (aus sicherheitsbezogenen Gründen) oder Office 365 Gruppen verwalten, die im Azure-Portal oder im Zugriffsbereich erstellt wurden, indem sie in **"Benutzer** können Sicherheitsgruppen in Azure-Portalen erstellen" oder "Benutzer können Office 365 Gruppen in Azure-Portalen erstellen" in "Alle Gruppen  >  **allgemein (Einstellungen)**" auswählen.
2. Sie können die Gruppenerstellung auch einschränken, um eine Gruppe von Benutzern auszuwählen, wenn Sie über eine Azure Active Directory P1-Premium-Lizenz verfügen.

**Deaktivieren der Willkommensbenachrichtigung für neue Office 365 Gruppenmitglieder**

Die Willkommensbenachrichtigung, die an Benutzer gesendet wird, die Office 365 Gruppen hinzugefügt werden, kann deaktiviert werden, indem **UnifiedGroupWelcomeMessageEnabled** in PowerShell auf "False" festgelegt wird. Erfahren Sie [hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true) mehr über diese Einstellung.

