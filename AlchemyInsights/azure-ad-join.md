---
title: Azure Active Directory-koppling
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405671"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="941fa-102">Azure Active Directory-koppling</span><span class="sxs-lookup"><span data-stu-id="941fa-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="941fa-103">Om du inställningar enhetsregistreringar för första gången bör du kontrollera att du har granskat Introduktion till enhetshantering i [Azure Active Directory](/azure/active-directory/devices/overview) som vägleder dig om hur du får enheter under kontroll till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="941fa-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="941fa-104">Om du registrerar enheter i Azure AD direkt och registrerar dem i Intune måste du se till [](/mem/intune/fundamentals/licenses-assign) att du har konfigurerat [Intune](/mem/intune/enrollment/device-enrollment) och har licensieringen först.</span><span class="sxs-lookup"><span data-stu-id="941fa-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="941fa-105">Se till att du har behörighet att utföra åtgärder i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="941fa-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="941fa-106">Endast en global administratör i Azure AD kan hantera inställningar för enhetsregistreringar.</span><span class="sxs-lookup"><span data-stu-id="941fa-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="941fa-107">Om du vill implementering av Azure AD-koppling kan du [gå med i Planera Azure AD-anslutning.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="941fa-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="941fa-108">Mer information om hur du löser vanliga problem med Azure AD-koppling finns i Vanliga frågor och svar om [Azure Ad Join](/azure/active-directory/devices/faq) och för Windows 10 Pro-enheter finns i Det går inte att ansluta Windows [10 Pro-datorn](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)till Azure AD - Behöver uppgradera till – Microsoft Community.</span><span class="sxs-lookup"><span data-stu-id="941fa-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
