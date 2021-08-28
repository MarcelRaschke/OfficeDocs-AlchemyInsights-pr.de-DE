---
title: Domänendienst konfigurieren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: cf8ea7d73adf36f71ae92abad48ef9b664eb0c96094a38750c86cf42958b5323
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994756"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>AAD-DS kann nicht aktiviert werden oder die Bereitstellung schlägt fehl

Führen Sie die folgenden Schritte durch, um das Problem zu beheben, dass der Azure AD Domain Service (AAD-DS) nicht aktiviert ist oder nicht bereitgestellt werden kann:

1. Wenn Sie ein bereits bestehendes virtuelles Netzwerk verwenden, überprüfen Sie Ihren NSG auf Regeln, die Ports blockieren, die für die Synchronisierung in AAD-DS im Portal https://aka.ms/aadds-networking benötigt werden.
2. Überprüfen Sie, ob Ihre Fehlermeldung in dieser Anleitung zur Problembehandlung beantwortet wird, die unter   https://aka.ms/aadds-troubleshoot-enable verfügbar ist.
3. Versuchen Sie, Azure AD Domain Services in einem neuen virtuellen Netzwerk bereitzustellen.
4. Folgen Sie der Anleitung „Erste Schritte zum Bereitstellen von AAD-DS“: [AAD Domain Services erstellen und konfigurieren](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Wenn Sie Probleme mit der Bereitstellung von Azure AD Domain Services haben, finden Sie unter [Problembehandlung für Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) häufige Fehler, um alles wieder zum Laufen zu bringen. 

**AAD-DS kann nicht deaktiviert werden**

AAD-DS kann nicht angehalten werden. Wenn Sie Ihre verwaltete Domäne nicht mehr verwenden möchten, muss sie gelöscht werden.
Informationen zum Löschen der verwalteten Domäne finden Sie unter [AAD Domain Service löschen](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



