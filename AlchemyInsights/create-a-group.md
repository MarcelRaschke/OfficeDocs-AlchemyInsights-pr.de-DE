---
title: Erstellen einer Gruppe
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 227ee85cb88cf71d8255995326d6660e37786720
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66508578"
---
# <a name="create-a-group"></a>Erstellen einer Gruppe

In diesem Thema wird die Gruppenerstellung beschrieben.

**Berechtigung zum Erstellen einer Gruppe**

Stellen Sie sicher, dass Sie berechtigt sind, eine neue Gruppe zu erstellen. Globale Administratoren können die Gruppenerstellung im Microsoft Azure-Portal oder im Access Panel deaktivieren. Möglicherweise benötigen Sie einen Administrator, um die neue Gruppe für Sie zu erstellen oder Ihnen die entsprechenden Berechtigungen zu erteilen.

**Verwalten von Gruppenerstellungsberechtigungen**

1. Globale Administratoren können Gruppenerstellungsberechtigungen (aus sicherheitsrelevanten Gründen) oder Office 365 Gruppen verwalten, die im Azure-Portal oder Zugriffsbereich erstellt wurden, indem sie in "Benutzer können Sicherheitsgruppen in Azure-Portalen erstellen" oder "Benutzer können Office 365 Gruppen in Azure-Portalen erstellen" in **"Alle Gruppen** > **allgemein( Einstellungen) aus**.
2. Sie können auch die Gruppenerstellung einschränken, um eine Gruppe von Benutzern auszuwählen, wenn Sie über eine Azure Active Directory P1 Premium-Lizenz verfügen.

**Deaktivieren der Willkommensbenachrichtigung für neue Office 365 Gruppenmitglieder**

Die willkommene Benachrichtigung, die an Benutzer gesendet wird, die Office 365 Gruppen hinzugefügt werden, kann deaktiviert werden, indem **UnifiedGroupWelcomeMessageEnabled** in Powershell auf "False" festgelegt wird. Erfahren Sie [hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true) mehr über diese Einstellung.

