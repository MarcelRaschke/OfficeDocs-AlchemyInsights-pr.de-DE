---
title: Behandeln von Problemen mit SAML-Signaturzertifikaten
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004341"
- "9406"
ms.date: 03/08/2021
ms.openlocfilehash: 9922ebf94c6f63690f87aefd50882328800feaac
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66251398"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Behandeln von Problemen mit SAML-Signaturzertifikaten

Führen Sie die folgenden empfohlenen Schritte aus, um Probleme mit SAML-Signaturzertifikaten zu beheben:

1. Wenn Sie eine Unternehmensanwendung hinzufügen, die SSO (einmaliges Anmelden) unterstützt, generiert Azure ein Zertifikat, das als [SAML-Signaturzertifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) bezeichnet wird. Dieses Zertifikat hat eine Gültigkeit von 3 Jahren. Informationen zum Ändern des Ablaufdatums Ihres Zertifikats finden Sie unter [Anpassen des Ablaufdatums eines Verbundzertifikats und dessen Rollup in ein neues Zertifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure verwendet dieses Zertifikat, um die von der Anwendung angeforderten SAML-Token zu signieren und an die Anwendung für ein erfolgreiches einmaliges Anmelden (Single Sign-On, SSO) zu senden. Damit dies durchgeführt werden kann, laden Sie das Zertifikat vom Azure-Portal herunter, und übermitteln Sie es an den Anwendungsanbieter, um den SSO-Prozess abzuschließen.

Nach Abschluss dieses Vorgangs vertraut die Anwendung diesem Zertifikat, und alle SAML-Token, die von diesem Zertifikat signiert sind, werden von ihr akzeptiert.

3. Wenn dieses Zertifikat abläuft, erstellen Sie ein neues, aktualisieren Sie es für den Anwendungsanbieter, und aktivieren Sie es dann auf Azure-Seite. Weitere Informationen finden Sie unter [Erneuern eines Zertifikats, das in Kürze abläuft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

**Hinweis**: Wenn das Zertifikat abläuft, wird der Benutzer nicht blockiert.

4. [Fügen Sie eine E-Mail-Adresse für Benachrichtigungen hinzu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration), die Sie vor Ablauf des aktuellen Zertifikats erhalten wollen.

**Hinweis**: Schritt 4 ist optional.

5. Ändern Sie die SAML-Zertifikatsignierungsoptionen einer Anwendung und den Zertifikatsignierungsalgorithmus. Weitere Informationen finden Sie unter [Ändern von Zertifikatsignierungsoptionen und Signierungsalgorithmus](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

