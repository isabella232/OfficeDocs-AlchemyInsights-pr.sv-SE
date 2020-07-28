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
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push-certifikat har inte ställts in

Ett Apple MDM Push-certifikat (även kallat APNS-certifikat (Apple Push Notification Service) har inte konfigurerats för prenumerationen. Utan ett Apple MDM Push-certifikat konfigurerat kan du inte registrera och hantera iOS- och Mac OS-enheter. När du har lagt till certifikatet i Intune kan användare installera företagsportalappen för att registrera sina iOS-enheter.

1. Välj **"Jag godkänner".** för att ge Microsoft behörighet att skicka data till Apple.

2. Välj **Hämta din CSR** den Intune-certifikatsigneringsbegäran som krävs för att skapa ett Apple MDM-push-certifikat. Filen används för att begära ett certifikat för förtroenderelation från Apple Push Certificates Portal.

3. Välj **Skapa ditt MDM-push-certifikat** för att gå till Apple Push Certificates Portal. Logga in med ditt företags Apple-ID och välj sedan **Skapa ett certifikat**. Välj **Välj fil**, bläddra till certifikatsigneringsbegäran och välj sedan Ladda **upp**. På sidan Bekräftelse väljer du **Hämta** för att hämta certifikatfilen (.pem) och spara filen lokalt.
 
**Certifikatet**är associerat med det Apple-ID som används för att skapa det. Det bästa är att använda ett apple-ID för hanteringsuppgifter och se till att postlådan övervakas av mer än en person eller med hjälp av en distributionslista. Använd aldrig ett personligt Apple-ID. Använd samma Apple-ID för att förnya Apple Push-certifikatet var tolfte månad.
 
4. Ange det Apple-ID som används för att skapa ditt Apple MDM-push-certifikat. Registrera det här ID:t som en påminnelse om när du behöver förnya certifikatet.

5. Gå till certifikatfilen (.pem), välj **Öppna**och välj sedan **Ladda upp**. Med push-certifikatet kan Intune registrera och hantera Apple-enheter.