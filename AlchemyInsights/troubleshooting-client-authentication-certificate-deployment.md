---
title: Problembehandlung bei der Bereitstellung von Clientauthentifizierungszertifikaten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 5bae3e7c155954b936562e5244c3b3c695387e04
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63281537"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Problembehandlung bei der Bereitstellung von Clientauthentifizierungszertifikaten

Intune-Profile für NDES/SCEP- und PKCS/PFX-Clientzertifikate werden häufig in Verbindung mit anderen Profiltypen wie WLAN, VPN und E-Mail verwendet, um Benutzern die Authentifizierung bei Unternehmensressourcen zu ermöglichen. Wenn diese Profiltypen mit einem Clientzertifikatprofil verknüpft sind, sind sie von der erfolgreichen Bereitstellung dieses Profils abhängig.

Das anfängliche Einrichten der Infrastruktur und die zugehörige Konfiguration des Clientzertifikatprofils erfordern häufig eine Problembehandlung. Eine schrittweise Anleitung für eine erfolgreiche Einrichten des NDES-Connectors sowie eine Anleitung zur Problembehandlung, um Probleme mit der Bereitstellung von Zertifikaten zu isolieren, finden Sie unter: 

- [Konfigurieren der Infrastruktur, sodass SCEP mit Intune unterstützt wird](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Übersicht für die Problembehandlung von SCEP-Zertifikatprofilen mit Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Verwenden Sie die referenzierten PowerShell-Skripts, um Ihre Konfiguration zu überprüfen. Weitere Informationen finden Sie unter [Skripts für die Überprüfung des Intune-Zertifikat-Connectors](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Sonstige häufig auftretende Probleme**

**Beim Versuch, den Intune-Zertifikat-Connector auf dem NDES-Connectorserver zu installieren, wird die Meldung „Das Kennwort in der Zertifikatanforderung kann nicht überprüft werden. Möglicherweise wurde es bereits verwendet. Rufen Sie ein neues Kennwort ab, um es mit diese Anforderung zu übermitteln.“ angezeigt.**  

Diese Meldung bedeutet, dass Sie die Installation des Zertifikat-Connectors als Administrator ausführen müssen.

In einigen Umgebungen müssen die Server, auf denen das Intune-Zertifikat ausgeführt wird, einen Proxyserver zum Herstellen einer Verbindung mit Intune verwenden, weshalb der Zertifikat-Connector ebenfalls einen Proxy verwenden muss. Unter bestimmten Umständen ignoriert der NDES-Connector die konfigurierten Proxyeinstellungen, und es kann notwendig sein, die Proxyeinstellungen während der Ausführung im Sicherheitskontext von „LocalSystem“ zu konfigurieren. 
 
Die Lösung besteht darin, Internet Explorer als SYSTEM auszuführen und einen Proxy in IE zu konfigurieren. Nach einem Neustart des Intune-Connectordiensts stellt der NDES-Connector eine Verbindung mit Intune her.

**Benutzergeräte empfangen keine SCEP-Zertifikate mehr von NDES.**

Es ist möglich, dass das Clientauthentifizierungszertifikat, das für den NDES-Server ausgestellt und während der NDES-Connectorinstallation angegeben wurde, abgelaufen oder nicht vorhanden ist. Gehen Sie zur Behebung folgendermaßen vor: 
 
1. Deinstallieren Sie den NDES-Connector.  
2. Verwenden Sie diese Details, um ein neues Clientauthentifizierungs- oder Serverauthentifizierungszertifikat anzufordern: 
 
    - Antragstellername: CN=externer FQDN  
    - Alternativer Antragstellername (beide sind erforderlich): DNS=externer FQDN, DNS=interner FQDN 
 
3. Installieren Sie den NDES-Connector erneut mit dem neuen Zertifikat.