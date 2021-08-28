---
title: API-Berechtigungen und Zustimmung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932096"
---
# <a name="api-permissions-and-consent"></a>API-Berechtigungen und Zustimmung

Anwendungen, die in Microsoft Identity Platform integriert werden, folgen einem Autorisierungsmodell, das Benutzern und Administratoren die Kontrolle darüber gibt, wie auf Daten zugegriffen werden kann. Die Implementierung des Autorisierungsmodells wurde auf dem Microsoft Identity Platform Endpunkt aktualisiert. Es ändert, wie eine App mit dem Microsoft Identity Platform interagieren muss. [Berechtigungen und Zustimmung im Microsoft Identity Platform Endpunkt](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) umfassen die grundlegenden Konzepte dieses Autorisierungsmodells, einschließlich Bereichen, Berechtigungen und Zustimmung.

Das [Azure Active Directory (Azure AD)-Zustimmungsframework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) erleichtert die Entwicklung von mehrinstanzenfähigen Web- und systemeigenen Clientanwendungen. Diese Anwendungen ermöglichen die Anmeldung von Benutzerkonten von einem Azure AD-Mandanten, der sich von dem unterscheidet, in dem die Anwendung registriert ist. Sie müssen möglicherweise auch auf Web-APIs wie die Microsoft Graph-API (um auf Azure AD, Intune und Dienste in Microsoft 365 zuzugreifen) und andere APIs der Microsoft-Dienste zugreifen, zusätzlich zu Ihren eigenen Web-APIs.

