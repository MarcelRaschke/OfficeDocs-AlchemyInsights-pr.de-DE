---
title: Kennworthashsynchronisierung für Domänendienst
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004400"
- "9003245"
- "8248"
- "8249"
ms.date: 02/09/2021
ms.openlocfilehash: 32fa4d82599f0b0ba81c78acba348b4a3034cc38
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66255970"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Kennworthashsynchronisierung für Domänendienst

**Wenn Sie von Ihrer Azure AD DS-Instanz aufgefordert werden, die Kennworthashsynchronisierung zu aktivieren**

Es trifft ein Szenario ein, in dem eine Hybridumgebung mit Benutzern ausgeführt wird, die aus einer lokalen Azure Active Directory Domain Services-Umgebung (AD DS) synchronisieren. Dieses Szenario ist eingetreten, obwohl die Kennworthashsynchronisierung zwischen dem lokalen AD DS und Ihrem Azure AD-Mandanten besteht.

**Ursache**

Dies geschieht, weil Azure AD Connect standardmäßig keine älteren New Technology LAN Manager (NTLM)- und Kerberos-Kennworthashwerte synchronisiert, die für Azure AD DS erforderlich sind.

**Problemumgehung** 

Sie müssen Azure AD Connect so konfigurieren, dass diese Kennworthashwerte synchronisiert werden, die für die NTLM- und Kerberos-Authentifizierung erforderlich sind.

Nachdem Azure AD Connect konfiguriert wurde, werden bei der Erstellung eines lokalen Kontos oder einem Kennwortänderungsereignis auch ältere Kennworthashwerte mit Azure AD synchronisiert. Weitere Informationen hierzu und Anleitungen zum Aktivieren der Kennwortsynchronisierung in Azure AD DS-Hybridumgebungen finden Sie [hier](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync).