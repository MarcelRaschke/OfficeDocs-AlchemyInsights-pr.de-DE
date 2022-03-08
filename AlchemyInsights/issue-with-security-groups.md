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
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 4e5ad28a229e0fb98b0d8094605ecf1a90b13a9a
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63235527"
---
# <a name="issue-with-security-groups"></a>Problem mit Sicherheitsgruppen

**Wenn Sie Netzwerkfehler des Typs AADDS104 erhalten**

Ungültige Regeln für Netzwerksicherheitsgruppen sind die häufigste Ursache für Netzwerkfehler in Azure Active Directory Domain Services (AD DS). Die Netzwerksicherheitsgruppe für das virtuelle Netzwerk muss den Zugriff auf bestimmte Ports und Protokolle zulassen. Wenn diese Ports blockiert sind, kann die Azure-Plattform die verwaltete Domäne nicht überwachen oder aktualisieren. Die Synchronisierung zwischen Azure AD und Azure AD DS ist ebenfalls betroffen. Stellen Sie sicher, dass die Standardports geöffnet bleiben, um Dienstunterbrechungen zu vermeiden.

Informationen zum Verstehen und Beheben häufiger Warnungen zu Konfigurationsproblemen bei der Netzwerksicherheitsgruppe finden Sie unter [Hinzufügen und Überprüfen von Sicherheitsgruppen](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
