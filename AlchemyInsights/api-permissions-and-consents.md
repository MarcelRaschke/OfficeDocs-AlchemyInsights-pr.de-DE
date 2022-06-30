---
title: API-Berechtigungen und Zustimmung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004343"
- "7756"
ms.date: 01/25/2021
ms.openlocfilehash: c4a55914dc8866e4809c9e5fd94bfcb20f7502e6
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66301039"
---
# <a name="api-permissions-and-consent"></a>API-Berechtigungen und Zustimmung

Anwendungen, die in Microsoft Identity Platform integrieren, folgen einem Autorisierungsmodell, das Benutzern und Administratoren die Kontrolle darüber gibt, wie auf Daten zugegriffen werden kann. Die Implementierung des Autorisierungsmodells wurde auf dem Microsoft Identity Platform Endpunkt aktualisiert. Es ändert die Interaktion einer App mit dem Microsoft Identity Platform. [Berechtigungen und Zustimmungen im Microsoft Identity Platform Endpunkt](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) decken die grundlegenden Konzepte dieses Autorisierungsmodells ab, einschließlich Bereiche, Berechtigungen und Zustimmung.

Das [Azure Active Directory (Azure AD)-Zustimmungsframework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) erleichtert die Entwicklung von mehrinstanzenfähigen Web- und nativen Clientanwendungen. Diese Anwendungen ermöglichen die Anmeldung durch Benutzerkonten von einem Azure AD-Mandanten, der sich von dem unterscheidet, in dem die Anwendung registriert ist. Möglicherweise müssen sie zusätzlich zu Ihren eigenen Web-APIs auch auf Web-APIs wie die Microsoft Graph-API (für den Zugriff auf Azure AD, Intune und Dienste in Microsoft 365) und die APIs anderer Microsoft-Dienste zugreifen.

