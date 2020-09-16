---
title: Meddelanden i Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: c1fbeea7bf4269e90e52cf5c129e904c99714926
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662811"
---
# <a name="notifications-in-yammer"></a>Meddelanden i Yammer

[Yammer skickar meddelanden](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) som meddelar användarna om ny aktivitet i konversationer de följer antingen via e-postmeddelanden eller, för användare med mobila enheter, push-meddelanden. Som standard skickar Yammer meddelanden för många typer av aktivitet i ditt nätverk. Användare kan uppdatera sina e-postinställningar via Yammer-webbplatsen och push-meddelanden konfigureras via mobilappen. 

Yammer har lagt till stöd för [interaktiva e-postmeddelanden i Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Vissa e-postmeddelanden (kopior av meddelande) blir interaktiva i Outlook på webben. En kommande uppdatering kommer att lägga till detta till andra versioner av Outlook.

**Typer av meddelanden i Yammer**

- E-postmeddelanden (uppdateringar från en grupp, någon bjuder in dig till en grupp, du får ett meddelande i Inkorgen osv.)
- Push-meddelanden (skickas till mobila enheter när du nämns får du ett meddelande i Inkorgen osv.)
- Popup-fönster på Skrivbordet (om du har Yammer Skrivbordsprogrammet installerat visas meddelanden för användare som kallas "popup-meddelanden".)
- Klockmeddelanden (på Yammer-webbplatsen ser användarna meddelanden för olika händelser. Dessa meddelanden kanske inte alltid har ett kopplat e-postmeddelande eller en push-avisering.)

Mer [detaljerad information om meddelanden](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) är tillgänglig.

**Hantera meddelanden**

Användare måste administrera sina egna meddelanden. Information finns i [hur du aktiverar och inaktiverar e-post och push-avisering för Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Det är inte att möjligt för administratörer att inaktivera alla aviseringar eller kontrollmeddelanden för användare. Administratörer kan [styra vilken logotyp som ingår i e-postmeddelandena och om användarna ska behöva bekräfta meddelanden](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) skickade via e-post.

**E-postmeddelanden som skickas till flera användare i organisationen**

Ibland skickas ett enskilt e-postmeddelande av Yammer och tas emot av många fler användare i organisationen än förväntat. Detta inträffar när en distributionslista eller annan typ av icke-enskild e-postadress läggs till i Yammer. Yammer vet inte i alla fall, om en e-postadress tillhör en enskild användare eller är en e-postadress som gör att ett e-postmeddelande levereras till många mottagare. När det här problemet uppstår måste du vidta åtgärder för att [göra uppehåll för (inaktivera) den ogiltiga användaren med den e-postadress](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) i Yammer. 

Om du vill minska risken för att problemet ska uppstår ska du:

1. [Tillämpa Office 365-identitet](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) för Yammer-användare.
2. Blockera externa avsändare från att skicka e-post till din organisation eller begränsa avsändare till en godkänd lista.

Om det här problemet uppstår:

1. Identifiera mottagaren av e-postmeddelandet, som ska matcha användaren i Yammer. All-in-sales@fabrikam.com är till exempel en DL för alla säljare. Denna DL skulle kunna identifieras från e-postmeddelandet från Yammer som tagits emot av användarna.
2. Använd funktionen [inaktivera (suspend) i Nätverksadministration](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) för att avbryta användaren med e-postadressen all-in-sales@fabrikam.com. Inaktiveringen kan inte tas bort vilket gör det säkrare än radering. Radering av användaren sker automatiskt efter 90 dagar.
3. Om du vill kan du granska [Användarexport](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) för att hitta andra e-postadresser som inte ska finns i gruppen.
