---
title: Problem mit Sicherheitsgruppen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: d8a3c011a3a7cba6c0b1cd00ac0eb587b75bbb5b06d96ef9fd75313734e74fd0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925740"
---
# <a name="issue-with-security-groups"></a>Problem mit Sicherheitsgruppen

**Wenn Sie Netzwerkfehler des Typs AADDS104 erhalten**

Ungültige Regeln für Netzwerksicherheitsgruppen sind die häufigste Ursache für Netzwerkfehler in Azure Active Directory Domain Services (AD DS). Die Netzwerksicherheitsgruppe für das virtuelle Netzwerk muss den Zugriff auf bestimmte Ports und Protokolle zulassen. Wenn diese Ports blockiert sind, kann die Azure-Plattform die verwaltete Domäne nicht überwachen oder aktualisieren. Die Synchronisierung zwischen Azure AD und Azure AD DS ist ebenfalls betroffen. Stellen Sie sicher, dass die Standardports geöffnet bleiben, um Dienstunterbrechungen zu vermeiden.

Informationen zum Verstehen und Beheben häufiger Warnungen zu Konfigurationsproblemen bei der Netzwerksicherheitsgruppe finden Sie unter [Hinzufügen und Überprüfen von Sicherheitsgruppen](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
