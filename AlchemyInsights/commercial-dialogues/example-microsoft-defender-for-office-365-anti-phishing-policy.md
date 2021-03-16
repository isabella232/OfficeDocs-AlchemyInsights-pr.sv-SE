---
title: Exempel på en policy mot nätfiske i Microsoft Defender för Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750798"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="32791-102">Exempel på en policy mot nätfiske i Microsoft Defender för Office 365</span><span class="sxs-lookup"><span data-stu-id="32791-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="32791-103">De här inställningarna aktiverar en princip som *heter Domän och VD.*</span><span class="sxs-lookup"><span data-stu-id="32791-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="32791-104">Med den här principen skyddas både användare och domäner från personifiering och sedan tillämpas principen på all e-post som tas emot av användare i domänen.</span><span class="sxs-lookup"><span data-stu-id="32791-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="32791-105">Lägg först till följande information för att skapa principen:</span><span class="sxs-lookup"><span data-stu-id="32791-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="32791-106">**Namn**: Beskrivning av domän **och** VD : Säkerställer att VD och din domän inte utger sig för att vara.</span><span class="sxs-lookup"><span data-stu-id="32791-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="32791-107">**Används för:** Välj **Mottagarens domän är**.</span><span class="sxs-lookup"><span data-stu-id="32791-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="32791-108">Under **Valfri av dessa** väljer du **Välj** och sedan en domän.</span><span class="sxs-lookup"><span data-stu-id="32791-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="32791-109">Välj **+ Lägg till.**</span><span class="sxs-lookup"><span data-stu-id="32791-109">Select **+ Add**.</span></span> <span data-ttu-id="32791-110">Markera kryssrutan bredvid namnet på domänen i listan (till exempel klicka på *contoso.com*) och välj sedan Lägg **till**.</span><span class="sxs-lookup"><span data-stu-id="32791-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="32791-111">Välj **Klar**.</span><span class="sxs-lookup"><span data-stu-id="32791-111">Select **Done**.</span></span>
- <span data-ttu-id="32791-112">När principen har skapats kan du finjustera principen med hjälp av följande alternativ:</span><span class="sxs-lookup"><span data-stu-id="32791-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="32791-113">**Lägga till användare att skydda:** I det här exemplet ska du som minst lägga till VD:s e-postadress.</span><span class="sxs-lookup"><span data-stu-id="32791-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="32791-114">**Lägg till domäner att** skydda: Lägg till organisationsdomänen som innehåller vd:s kontor.</span><span class="sxs-lookup"><span data-stu-id="32791-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="32791-115">**Välj åtgärder:** För **Om** e-post skickas av en imiterad användare väljer du Omdirigera meddelandet till en annan e-postadress och anger sedan e-postadressen till säkerhetsadministratören (till *exempel securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="32791-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="32791-116">För **Om e-post skickas med en imiterad domän** väljer du Sätt meddelandet i **karantän.**</span><span class="sxs-lookup"><span data-stu-id="32791-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="32791-117">**Postlådeinformation:** Det här alternativet är valt som standard när du skapar en ny princip mot nätfiske.</span><span class="sxs-lookup"><span data-stu-id="32791-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="32791-118">Lämna den här inställningen **På** för bästa resultat.</span><span class="sxs-lookup"><span data-stu-id="32791-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="32791-119">**Lägga till betrodda avsändare och domäner:** I det här exemplet ska du inte definiera några åsidosättningar.</span><span class="sxs-lookup"><span data-stu-id="32791-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="32791-120">När du har granskat inställningarna väljer du Skapa **den här principen** eller **Spara** efter behov.</span><span class="sxs-lookup"><span data-stu-id="32791-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="32791-121">Mer information finns i [Principer för skydd mot nätfiske i Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="32791-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>