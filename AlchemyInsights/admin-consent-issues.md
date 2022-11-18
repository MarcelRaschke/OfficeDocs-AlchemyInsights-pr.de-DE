---
title: Admin Probleme mit der Zustimmung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004354"
- "7786"
ms.date: 01/18/2021
ms.openlocfilehash: c3b3a8de3a82aedf295004bf7fe4f364e1e54642
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66312699"
---
# <a name="admin-consent-issues"></a>Admin Probleme mit der Zustimmung

1. Aktivieren Sie den Workflow für die [Administratorzustimmung](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , damit Benutzer die Administratorgenehmigung direkt über den Zustimmungsbildschirm anfordern können.

1. Wenn Sie oder die Benutzer Ihrer Anwendung während des Zustimmungsprozesses unerwartete Fehler sehen, finden Sie in diesem Artikel Informationen zur Problembehandlung: [Unerwarteter Fehler beim Ausführen der Zustimmung zu einer Anwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Erfahren Sie mehr über [Admin Zustimmung im Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), wie die [Zustimmungsaufforderung](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) funktioniert und wie [Sie eine Anforderung für die mandantenweite Administratorzustimmung auswerten](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Anwendungen, die in Microsoft Identity Platform integrieren, folgen einem Autorisierungsmodell, das Benutzern und Administratoren die Kontrolle darüber gibt, wie auf Daten zugegriffen werden kann. Die Implementierung des Autorisierungsmodells wurde auf dem Microsoft Identity Platform Endpunkt aktualisiert und ändert, wie eine App mit der Microsoft Identity Platform interagieren muss. Eine Übersicht über dieses Autorisierungsmodell, einschließlich Bereiche, Berechtigungen und Zustimmung, finden Sie [unter Berechtigungen und Zustimmung im Microsoft Identity Platform Endpunkt](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).