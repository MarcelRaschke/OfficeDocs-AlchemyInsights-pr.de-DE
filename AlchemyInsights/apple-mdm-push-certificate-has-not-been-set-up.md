---
title: Das Apple MDM-Push-Zertifikat wurde nicht eingerichtet
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 239804d08413f9b4ab6fa6b7df2496c5c0268204
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62658904"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Das Apple MDM-Push-Zertifikat wurde nicht eingerichtet

Ein Apple MDM-Push-Zertifikat (auch bekannt als Apple-Push-Benachrichtigungsdienst-Zertifikat (Apple Push Notification Service, APNS)) wurde nicht für Ihr Abonnement konfiguriert. Ohne ein konfiguriertes Apple MDM-Push-Zertifikat, können Sie keine iOS-und Mac OS-Geräte registrieren und verwalten. Nachdem Sie das Zertifikat zu Intune hinzugefügt haben, können Benutzer die Unternehmensportal-App installieren, um ihre iOS-Geräte zu registrieren.

1. Wählen Sie **Ich stimme zu** aus, um Microsoft die Berechtigung zum Senden von Daten an Apple zu erteilen.

2. Wählen Sie **CSR herunterladen**, die Intune-Zertifikatsignieranforderung, die zum Erstellen eines Apple MDM-Push-Zertifikats erforderlich ist. Die Datei wird verwendet, um ein Vertrauensstellungszertifikat vom Apple-Portal für Push-Zertifikate anzufordern.

3. Wählen Sie **Eigenes MDM-Push-Zertifikat erstellen** aus, um zum Apple-Portal für Push-Zertifikate zu wechseln. Melden Sie sich mit der Apple-ID Ihres Unternehmens an, und wählen Sie dann **Zertifikat erstellen** aus. Wählen Sie **Datei auswählen** aus, wechseln Sie zur Zertifikatsignieranforderungs-Datei, und wählen Sie dann **Hochladen** aus. Wählen Sie auf der Seite „Bestätigung“ **Herunterladen** aus, um die Zertifikatdatei (.pem) herunterzuladen, und speichern Sie die Datei lokal.
 
**Hinweis**: Das Zertifikat ist der Apple-ID zugeordnet, mit der es erstellt wurde. Verwenden Sie als bewährte Methode eine Apple-ID des Unternehmens für Verwaltungsaufgaben, und stellen Sie sicher, dass das Postfach von mehr als einer Person überwacht wird, oder indem Sie eine Verteilerliste verwenden. Verwenden Sie niemals eine persönliche Apple-ID. Verwenden Sie dieselbe Apple-ID, um das Apple-Push-Zertifikat alle 12 Monate zu verlängern.
 
4. Geben Sie die Apple-ID ein, mit der Sie Ihr Apple MDM-Push-Zertifikat erstellt haben. Notieren Sie sich diese ID, damit Sie sie zur Hand haben, wenn Sie das Zertifikat verlängern müssen.

5. Wechseln Sie zur Zertifikatdatei (.pem), wählen Sie **Öffnen** aus, und wählen Sie dann **Hochladen** aus. Mit dem Push-Zertifikat kann Intune Apple-Geräte registrieren und verwalten.