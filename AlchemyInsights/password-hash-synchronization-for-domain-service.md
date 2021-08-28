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
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040865"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Kennworthashsynchronisierung für Domänendienst

**Wenn Sie von Ihrer Azure AD DS-Instanz aufgefordert werden, die Kennworthashsynchronisierung zu aktivieren**

Es trifft ein Szenario ein, in dem eine Hybridumgebung mit Benutzern ausgeführt wird, die aus einer lokalen Azure Active Directory Domain Services-Umgebung (AD DS) synchronisieren. Dieses Szenario ist eingetreten, obwohl die Kennworthashsynchronisierung zwischen dem lokalen AD DS und Ihrem Azure AD-Mandanten besteht.

**Ursache**

Dies geschieht, weil Azure AD Connect standardmäßig keine älteren New Technology LAN Manager (NTLM)- und Kerberos-Kennworthashwerte synchronisiert, die für Azure AD DS erforderlich sind.

**Problemumgehung** 

Sie müssen Azure AD Connect so konfigurieren, dass diese Kennworthashwerte synchronisiert werden, die für die NTLM- und Kerberos-Authentifizierung erforderlich sind.

Nachdem Azure AD Connect konfiguriert wurde, werden bei der Erstellung eines lokalen Kontos oder einem Kennwortänderungsereignis auch ältere Kennworthashwerte mit Azure AD synchronisiert. Weitere Informationen hierzu und Anleitungen zum Aktivieren der Kennwortsynchronisierung in Azure AD DS-Hybridumgebungen finden Sie [hier](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync).