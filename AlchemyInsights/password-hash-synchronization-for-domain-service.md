---
title: Kennworthashsynchronisierung für Domänendienst
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
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3128062ee4d835544784b5923988550e83f56155
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63213873"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Kennworthashsynchronisierung für Domänendienst

**Wenn Sie von Ihrer Azure AD DS-Instanz aufgefordert werden, die Kennworthashsynchronisierung zu aktivieren**

Es trifft ein Szenario ein, in dem eine Hybridumgebung mit Benutzern ausgeführt wird, die aus einer lokalen Azure Active Directory Domain Services-Umgebung (AD DS) synchronisieren. Dieses Szenario ist eingetreten, obwohl die Kennworthashsynchronisierung zwischen dem lokalen AD DS und Ihrem Azure AD-Mandanten besteht.

**Ursache**

Dies geschieht, weil Azure AD Connect standardmäßig keine älteren New Technology LAN Manager (NTLM)- und Kerberos-Kennworthashwerte synchronisiert, die für Azure AD DS erforderlich sind.

**Problemumgehung** 

Sie müssen Azure AD Connect so konfigurieren, dass diese Kennworthashwerte synchronisiert werden, die für die NTLM- und Kerberos-Authentifizierung erforderlich sind.

Nachdem Azure AD Connect konfiguriert wurde, werden bei der Erstellung eines lokalen Kontos oder einem Kennwortänderungsereignis auch ältere Kennworthashwerte mit Azure AD synchronisiert. Weitere Informationen hierzu und Anleitungen zum Aktivieren der Kennwortsynchronisierung in Azure AD DS-Hybridumgebungen finden Sie [hier](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync).