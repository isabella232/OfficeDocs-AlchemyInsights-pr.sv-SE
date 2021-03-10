---
title: Felsöka problem med SAML-signeringscertifikat
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
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694451"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Felsöka problem med SAML-signeringscertifikat

Lös problemet med SAML-signeringscertifikat genom att utföra följande rekommenderade steg:

1. När du lägger till ett företagsprogram som har stöd för SSO genererar Azure ett certifikat som kallas [SAML-signeringscertifikat.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Certifikatet har ett utgångsdatum på 3 år. Information om hur du ändrar utgångsdatumet för certifikatet finns i Anpassa utgångsdatumet för federationscertifikatet och [föra över det till ett nytt certifikat.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Azure använder det här certifikatet för att signera DE SAML-token som begärs av programmet och skicka det till programmet för en lyckad SSO. För att det ska slutföras laddar du ned certifikatet från Azure Portal och skickar det till programleverantören för att slutföra SSO-processen.

När den här processen har slutförts kommer programmet att lita på certifikatet och alla SAML-token som har signerats med det här certifikatet godkänns av programmet.

3. Om certifikatet går ut skapar du ett nytt certifikat, uppdaterar det till programleverantören och gör det sedan aktivt på Azure-sidan. Mer information finns i Förnya [ett certifikat som snart förfaller.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Om certifikatet går ut blockeras inte användaren.

4. [Lägg till en e-postadress för att](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) få meddelanden innan det aktuella certifikatet går ut.

> [!NOTE]
> Steg 4 är ett valfritt.

5. Ändra ett programs SAML-certifikatsigneringsalternativ och algoritmen för certifikatsignering. Mer information finns i Ändra alternativ [för certifikatsignering och signeringsalgoritm.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

