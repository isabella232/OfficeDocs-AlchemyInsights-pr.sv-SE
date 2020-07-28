---
title: Apple MDM Push-certifikat har inte ställts in
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440009"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="cdf43-102">Apple MDM Push-certifikat har inte ställts in</span><span class="sxs-lookup"><span data-stu-id="cdf43-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="cdf43-103">Ett Apple MDM Push-certifikat (även kallat APNS-certifikat (Apple Push Notification Service) har inte konfigurerats för prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="cdf43-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="cdf43-104">Utan ett Apple MDM Push-certifikat konfigurerat kan du inte registrera och hantera iOS- och Mac OS-enheter.</span><span class="sxs-lookup"><span data-stu-id="cdf43-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="cdf43-105">När du har lagt till certifikatet i Intune kan användare installera företagsportalappen för att registrera sina iOS-enheter.</span><span class="sxs-lookup"><span data-stu-id="cdf43-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="cdf43-106">Välj **"Jag godkänner".**</span><span class="sxs-lookup"><span data-stu-id="cdf43-106">Select **"I agree."**</span></span> <span data-ttu-id="cdf43-107">för att ge Microsoft behörighet att skicka data till Apple.</span><span class="sxs-lookup"><span data-stu-id="cdf43-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="cdf43-108">Välj **Hämta din CSR** den Intune-certifikatsigneringsbegäran som krävs för att skapa ett Apple MDM-push-certifikat.</span><span class="sxs-lookup"><span data-stu-id="cdf43-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="cdf43-109">Filen används för att begära ett certifikat för förtroenderelation från Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="cdf43-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="cdf43-110">Välj **Skapa ditt MDM-push-certifikat** för att gå till Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="cdf43-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="cdf43-111">Logga in med ditt företags Apple-ID och välj sedan **Skapa ett certifikat**.</span><span class="sxs-lookup"><span data-stu-id="cdf43-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="cdf43-112">Välj **Välj fil**, bläddra till certifikatsigneringsbegäran och välj sedan Ladda **upp**.</span><span class="sxs-lookup"><span data-stu-id="cdf43-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="cdf43-113">På sidan Bekräftelse väljer du **Hämta** för att hämta certifikatfilen (.pem) och spara filen lokalt.</span><span class="sxs-lookup"><span data-stu-id="cdf43-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="cdf43-114">**Certifikatet**är associerat med det Apple-ID som används för att skapa det.</span><span class="sxs-lookup"><span data-stu-id="cdf43-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="cdf43-115">Det bästa är att använda ett apple-ID för hanteringsuppgifter och se till att postlådan övervakas av mer än en person eller med hjälp av en distributionslista.</span><span class="sxs-lookup"><span data-stu-id="cdf43-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="cdf43-116">Använd aldrig ett personligt Apple-ID.</span><span class="sxs-lookup"><span data-stu-id="cdf43-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="cdf43-117">Använd samma Apple-ID för att förnya Apple Push-certifikatet var tolfte månad.</span><span class="sxs-lookup"><span data-stu-id="cdf43-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="cdf43-118">Ange det Apple-ID som används för att skapa ditt Apple MDM-push-certifikat.</span><span class="sxs-lookup"><span data-stu-id="cdf43-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="cdf43-119">Registrera det här ID:t som en påminnelse om när du behöver förnya certifikatet.</span><span class="sxs-lookup"><span data-stu-id="cdf43-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="cdf43-120">Gå till certifikatfilen (.pem), välj **Öppna**och välj sedan **Ladda upp**.</span><span class="sxs-lookup"><span data-stu-id="cdf43-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="cdf43-121">Med push-certifikatet kan Intune registrera och hantera Apple-enheter.</span><span class="sxs-lookup"><span data-stu-id="cdf43-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>