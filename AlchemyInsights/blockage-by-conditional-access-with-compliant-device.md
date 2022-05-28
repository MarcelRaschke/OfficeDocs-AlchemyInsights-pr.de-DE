---
title: Ich werde mit einem kompatiblen Gerät durch bedingten Zugriff blockiert.
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 2e83a74be981c84ef4cd4f27555dc6a4ff03f34d
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65734700"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Ich werde mit einem kompatiblen Gerät durch bedingten Zugriff blockiert.

**Sehr empfehlenswerte Tools**

- [Problembehandlungstool für Geräteregistrierung](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – Ein umfassendes Tool zur Behebung der häufigsten Probleme bei der Geräteregistrierung.
- [Skript zum Testen der Verbindung der Geräteregistrierung](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Ein Tool, mit dem sichergestellt wird, dass ein Gerät unter dem Systemkonto auf Endpunkte der Geräteregistrierung zugreifen kann.
- [Azure AD Gerätebereinigungsskript](https://github.com/mzmaili/AzureADDeviceCleanup) – Ein Tool, um verwaltete Geräte in Ihrer Umgebung aufzufinden und zu verwalten.

Hier sind einige häufige Gründe, warum der bedingte Zugriff für ein kompatibles Gerät fehlschlägt oder warum Ihre Benutzer während einer Anmeldeanforderung für eine Organisationsressource die Meldung **Sie können von hier aus nicht dorthin gelangen** erhalten.

1. **Das Gerät ist nicht in einem erforderlichen Gerätstatus mit einem MDM**:

Überprüfen Sie, ob das Gerät bei einem zugelassenen MDM-Anbieter wie Intune angemeldet und *als konform gekennzeichnet* ist. Weitere Informationen über Intune finden Sie in diesem [Dokument](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Für ein besseres Verständnis über die Geräte-Compliance und Intune lesen Sie [Compliance-Richtlinie verwenden, um Regeln für Geräte festzulegen, die Sie mit Intune verwalten](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Wenn Sie Probleme haben, ein Gerät bei Intune anzumelden, finden Sie Details zur Fehlerbehebung unter [Problembehandlung bei der Geräteanmeldung in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Für weiteren Intune-Support erstellen Sie eine Supportanforderung. Dies tun Sie über die [Intune-Hilfe- und Support-Seite](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Das Gerät ist nicht mit dem Organisationsnetzwerk verbunden**:

Für den Zugriff auf Organisationsressourcen muss das Gerät entweder über eine direkte Verbindung oder ein virtuelles privates Netzwerk (VPN) mit dem Netzwerk der Organisation und außerdem mit einem lokalen Verzeichnis oder mit Azure Active Directory verbunden sein. Informationen zum Verbinden eines Arbeitsgeräts mit dem Organisationsnetzwerk finden Sie unter [Verbinden Ihres Arbeitsgeräts mit dem Netzwerk Ihrer Organisation](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Informationen zum Registrieren eines persönlichen/BYOD-Gerätes finden Sie unter [Registrieren Ihres persönlichen Geräts im Netzwerk Ihrer Organisation](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Um zu überprüfen, ob das Gerät mit dem Netzwerk verbunden ist, können Sie [hier](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) die Schritte für registrierte Geräte oder [hier](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) die Schritte für Arbeitsgeräte ausführen. Um das Problem auf die Organisations-Netzwerkverbindung einzugrenzen, befolgen Sie die nachstehenden Anleitungen:

    1. Melden Sie sich mit Ihrem Geschäfts-, Schul- oder Unikonto bei Windows an, beispielsweise als alain@contoso.com.
    2. Verbinden Sie sich über ein VPN oder mit DirectAccess zum Netzwerk Ihrer Organisation.
    3. Nachdem Sie verbunden sind, drücken Sie die **WINDOWS-TASTE+L**, um Ihr Gerät zu sperren.
    4. Entsperren sie Ihre Gerät mit Ihrem Geschäfts-, Schul- oder Unikonto, und versuchen Sie den Zugriff auf die problematische App oder den problematischen Dienst erneut.

Wenn Sie die Fehlermeldung **Sie können von hier aus nicht dorthin gelangen** sehen, dann liegt das Problem wahrscheinlich an einem anderen Ort.

3. **Das Betriebssystem ist nicht unterstützt**:

Stellen Sie sicher, dass Sie eine unterstützte Version Ihres Betriebssystems ausführen, einschließlich:

- **Windows-Client**: Windows 7 oder später

- **Windows-Server** Windows Server 2008 R2 oder später

- **macOS**: macOS X oder später

- **Android und iOS**: Neueste Version der Android- und iOS-Mobilgeräte-Betriebssysteme.

4. **Der Webbrowser ist nicht unterstützt**:

Nachfolgend finden Sie die unterstützten Browser. Für die Chrome-Unterstützung mit Windows 1703 oder späteren Versionen ist eine Erweiterung für Windows 10-Konten erforderlich. Für Microsoft Edge 85+ muss der Benutzer angemeldet sein, um die Informationen zur Gerätekompatibilität korrekt weiterzugeben. Weitere Informationen finden Sie [hier](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune-verwalteter Browser, Safari
- **Android**: **Microsoft Edge**: Intune-verwalteter Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Weitere Informationen über die Nachricht **Sie können nicht dorthin gehen** und zu Problembehandlungsschritten finden Sie [hier](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
