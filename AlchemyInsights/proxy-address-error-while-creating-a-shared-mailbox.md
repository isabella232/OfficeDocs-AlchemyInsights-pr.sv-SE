---
title: Proxyadressfel när en delad postlåda skapas
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568308"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="1e472-102">Proxyadressfel när en postlåda eller ett annat e-postaktivat objekt skapas</span><span class="sxs-lookup"><span data-stu-id="1e472-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="1e472-103">Om du försökte skapa ett e-postaktivat objekt (postlåda, delad postlåda osv.) och fick felmeddelandet "Proxyadressen "SMTP:alias@domain.com" används redan...", används den e-postadress du valde redan av ett annat e-postaktivat objekt i organisationen.</span><span class="sxs-lookup"><span data-stu-id="1e472-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="1e472-104">Du måste hitta den användare, grupp, delade postlåda eller gemensamma mapp som har den här e-postadressen och ta bort den eller ändra dess e-postadress.</span><span class="sxs-lookup"><span data-stu-id="1e472-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="1e472-105">Sedan kan du skapa ett nytt e-postaktiverat objekt med den lediga e-postadressen.</span><span class="sxs-lookup"><span data-stu-id="1e472-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="1e472-106">Använd Sök på startsidan för att hitta den.</span><span class="sxs-lookup"><span data-stu-id="1e472-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="1e472-107">Du kan också använda följande Exchange Online PowerShell-kommando för att söka efter det:</span><span class="sxs-lookup"><span data-stu-id="1e472-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="1e472-108">Om du inte vill ta bort den befintliga e-postadressen väljer du en ny e-postadress för det nya objektet du skapar.</span><span class="sxs-lookup"><span data-stu-id="1e472-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  