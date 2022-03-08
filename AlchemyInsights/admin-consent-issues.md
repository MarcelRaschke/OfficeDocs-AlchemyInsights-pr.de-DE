---
title: Probleme mit der Administratorzustimmung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 2e50f2550d5c4f92918a091d30103f5b536cabd4
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63242477"
---
# <a name="admin-consent-issues"></a>Probleme mit der Administratorzustimmung

1. Aktivieren Sie den Workflow für die [Administratorzustimmung](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , damit Benutzer die Administratorgenehmigung direkt über den Zustimmungsbildschirm anfordern können.

1. Wenn ihnen oder den Benutzern Ihrer Anwendung während des Zustimmungsprozesses unerwartete Fehler angezeigt werden, finden Sie in diesem Artikel Schritte zur Problembehandlung: [Unerwarteter Fehler bei der Ausführung der Zustimmung zu einer Anwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Erfahren Sie mehr über [die Administratorzustimmung auf der Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), wie die [Zustimmungsaufforderung](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) funktioniert und wie [Sie eine Anforderung für die mandantenweite Administratorzustimmung auswerten](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Anwendungen, die in Microsoft Identity Platform integriert werden, folgen einem Autorisierungsmodell, das Benutzern und Administratoren die Kontrolle darüber gibt, wie auf Daten zugegriffen werden kann. Die Implementierung des Autorisierungsmodells wurde auf dem Microsoft Identity Platform Endpunkt aktualisiert und ändert, wie eine App mit dem Microsoft Identity Platform interagieren muss. Eine Übersicht über dieses Autorisierungsmodell, einschließlich Bereichen, Berechtigungen und Zustimmung, finden Sie [unter "Berechtigungen und Zustimmung" im Microsoft Identity Platform-Endpunkt](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).