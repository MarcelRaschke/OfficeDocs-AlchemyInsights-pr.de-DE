---
title: 'Domänencontroller '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9003233"
- "7909"
ms.date: 01/17/2021
ms.openlocfilehash: 6ab8f4e73b02974de3eb003124220fa5ff48a9f0
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66507018"
---
# <a name="domain-controller"></a>Domänencontroller

**AAD-DS kann nicht aktiviert werden oder die Bereitstellung schlägt fehl**

Führen Sie die folgenden Schritte durch, um das Problem zu beheben, dass der Azure AD Domain Service (AAD-DS) nicht aktiviert ist oder nicht bereitgestellt werden kann:

1. Wenn Sie ein bereits bestehendes virtuelles Netzwerk verwenden, überprüfen Sie Ihren NSG auf Regeln, die Ports blockieren, die für die Synchronisierung in AAD-DS im Portal https://aka.ms/aadds-networking benötigt werden.
2. Überprüfen Sie, ob Ihre Fehlermeldung in dieser Anleitung zur Problembehandlung beantwortet wird, die unter   https://aka.ms/aadds-troubleshoot-enable verfügbar ist.
3. Versuchen Sie, Azure AD Domain Services in einem neuen virtuellen Netzwerk bereitzustellen.
4. Folgen Sie der Anleitung „Erste Schritte zum Bereitstellen von AAD-DS“, die im [Lernprogramm zum Thema Azure AD Domain Services erstellen](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance) verfügbar ist.
5. Wenn Sie Probleme mit der Bereitstellung von Azure AD Domain Services haben, finden Sie unter [Problembehandlung für Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) häufige Fehler, um alles wieder zum Laufen zu bringen. 

**AAD-DS kann nicht deaktiviert werden**

AAD-DS kann nicht angehalten werden. Wenn Sie Ihre verwaltete Domäne nicht mehr verwenden möchten, muss sie gelöscht werden.

Wenn Sie auf Probleme stoßen, finden Sie unter [Problembehandlung für Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) Informationen zur Behebung häufiger Fehlermeldungen und zugehörige Schritte zur Problembehandlung, die Ihnen helfen, alles wieder zum Laufen zu bringen.
