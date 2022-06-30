---
title: Problem mit Sicherheitsgruppen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004397"
- "8252"
ms.date: 02/09/2021
ms.openlocfilehash: 77e9800f12ad785464d70eccc257b1120281bd5c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66405040"
---
# <a name="issue-with-security-groups"></a>Problem mit Sicherheitsgruppen

**Wenn Sie Netzwerkfehler des Typs AADDS104 erhalten**

Ungültige Regeln für Netzwerksicherheitsgruppen sind die häufigste Ursache für Netzwerkfehler in Azure Active Directory Domain Services (AD DS). Die Netzwerksicherheitsgruppe für das virtuelle Netzwerk muss den Zugriff auf bestimmte Ports und Protokolle zulassen. Wenn diese Ports blockiert sind, kann die Azure-Plattform die verwaltete Domäne nicht überwachen oder aktualisieren. Die Synchronisierung zwischen Azure AD und Azure AD DS ist ebenfalls betroffen. Stellen Sie sicher, dass die Standardports geöffnet bleiben, um Dienstunterbrechungen zu vermeiden.

Informationen zum Verstehen und Beheben häufiger Warnungen zu Konfigurationsproblemen bei der Netzwerksicherheitsgruppe finden Sie unter [Hinzufügen und Überprüfen von Sicherheitsgruppen](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
