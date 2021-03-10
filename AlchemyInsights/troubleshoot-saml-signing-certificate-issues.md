---
title: Behandeln von Problemen mit SAML-Signaturzertifikaten
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529211"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Behandeln von Problemen mit SAML-Signaturzertifikaten

Führen Sie die folgenden empfohlenen Schritte aus, um Probleme mit SAML-Signaturzertifikaten zu beheben:

1. Wenn Sie eine Unternehmensanwendung hinzufügen, die SSO (einmaliges Anmelden) unterstützt, generiert Azure ein Zertifikat, das als [SAML-Signaturzertifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) bezeichnet wird. Dieses Zertifikat hat eine Gültigkeit von 3 Jahren. Informationen zum Ändern des Ablaufdatums Ihres Zertifikats finden Sie unter [Anpassen des Ablaufdatums eines Verbundzertifikats und dessen Rollup in ein neues Zertifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure verwendet dieses Zertifikat, um die von der Anwendung angeforderten SAML-Token zu signieren und an die Anwendung für ein erfolgreiches einmaliges Anmelden (Single Sign-On, SSO) zu senden. Damit dies durchgeführt werden kann, laden Sie das Zertifikat vom Azure-Portal herunter, und übermitteln Sie es an den Anwendungsanbieter, um den SSO-Prozess abzuschließen.

Nach Abschluss dieses Vorgangs vertraut die Anwendung diesem Zertifikat, und alle SAML-Token, die von diesem Zertifikat signiert sind, werden von ihr akzeptiert.

3. Wenn dieses Zertifikat abläuft, erstellen Sie ein neues, aktualisieren Sie es für den Anwendungsanbieter, und aktivieren Sie es dann auf Azure-Seite. Weitere Informationen finden Sie unter [Erneuern eines Zertifikats, das in Kürze abläuft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Wenn das Zertifikat abläuft, wird der Benutzer nicht blockiert.

4. [Fügen Sie eine E-Mail-Adresse für Benachrichtigung hinzu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration), die vor Ablauf des aktuellen Zertifikats versendet werden sollen.

> [!NOTE]
> Schritt 4 ist optional.

5. Ändern Sie die SAML-Zertifikatsignierungsoptionen einer Anwendung und den Zertifikatsignierungsalgorithmus. Weitere Informationen finden Sie unter [Ändern von Zertifikatsignierungsoptionen und Signierungsalgorithmus](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

