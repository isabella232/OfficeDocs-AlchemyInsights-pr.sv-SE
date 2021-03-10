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
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="06ba2-102">Felsöka problem med SAML-signeringscertifikat</span><span class="sxs-lookup"><span data-stu-id="06ba2-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="06ba2-103">Lös problemet med SAML-signeringscertifikat genom att utföra följande rekommenderade steg:</span><span class="sxs-lookup"><span data-stu-id="06ba2-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="06ba2-104">När du lägger till ett företagsprogram som har stöd för SSO genererar Azure ett certifikat som kallas [SAML-signeringscertifikat.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="06ba2-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="06ba2-105">Certifikatet har ett utgångsdatum på 3 år.</span><span class="sxs-lookup"><span data-stu-id="06ba2-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="06ba2-106">Information om hur du ändrar utgångsdatumet för certifikatet finns i Anpassa utgångsdatumet för federationscertifikatet och [föra över det till ett nytt certifikat.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="06ba2-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="06ba2-107">Azure använder det här certifikatet för att signera DE SAML-token som begärs av programmet och skicka det till programmet för en lyckad SSO.</span><span class="sxs-lookup"><span data-stu-id="06ba2-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="06ba2-108">För att det ska slutföras laddar du ned certifikatet från Azure Portal och skickar det till programleverantören för att slutföra SSO-processen.</span><span class="sxs-lookup"><span data-stu-id="06ba2-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="06ba2-109">När den här processen har slutförts kommer programmet att lita på certifikatet och alla SAML-token som har signerats med det här certifikatet godkänns av programmet.</span><span class="sxs-lookup"><span data-stu-id="06ba2-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="06ba2-110">Om certifikatet går ut skapar du ett nytt certifikat, uppdaterar det till programleverantören och gör det sedan aktivt på Azure-sidan.</span><span class="sxs-lookup"><span data-stu-id="06ba2-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="06ba2-111">Mer information finns i Förnya [ett certifikat som snart förfaller.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="06ba2-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="06ba2-112">Om certifikatet går ut blockeras inte användaren.</span><span class="sxs-lookup"><span data-stu-id="06ba2-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="06ba2-113">[Lägg till en e-postadress för att](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) få meddelanden innan det aktuella certifikatet går ut.</span><span class="sxs-lookup"><span data-stu-id="06ba2-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="06ba2-114">Steg 4 är ett valfritt.</span><span class="sxs-lookup"><span data-stu-id="06ba2-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="06ba2-115">Ändra ett programs SAML-certifikatsigneringsalternativ och algoritmen för certifikatsignering.</span><span class="sxs-lookup"><span data-stu-id="06ba2-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="06ba2-116">Mer information finns i Ändra alternativ [för certifikatsignering och signeringsalgoritm.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="06ba2-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

