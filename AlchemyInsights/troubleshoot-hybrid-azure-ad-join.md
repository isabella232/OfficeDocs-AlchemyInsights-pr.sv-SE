---
title: Felsöka hybrid Azure AD-anslutning
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401925"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="aeb48-102">Felsöka hybrid Azure AD-anslutning</span><span class="sxs-lookup"><span data-stu-id="aeb48-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="aeb48-103">Rekommenderas starkt för att se till att en enhet kan komma åt slutpunkter för enhetsregistrering under systemkontot genom att använda [Skriptet för att testa anslutningen för enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="aeb48-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="aeb48-104">Om du konfigurerar enhetsregistreringar för första gången bör du läsa [Introduktion till enhetshantering i Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), för att lära dig hur du får Azure AD att kontrollera enheter.</span><span class="sxs-lookup"><span data-stu-id="aeb48-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="aeb48-105">Om du registrerar enheter direkt i Azure AD och registrerar dem i Intune ska du kontrollera att du har [konfigurerat Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) och har all [licensiering](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) klart först.</span><span class="sxs-lookup"><span data-stu-id="aeb48-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="aeb48-106">Se till att du är behörig att utföra åtgärder i Azure AD och lokala AD.</span><span class="sxs-lookup"><span data-stu-id="aeb48-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="aeb48-107">Endast en global administratör i Azure AD kan hantera inställningar för enhetsregistreringar.</span><span class="sxs-lookup"><span data-stu-id="aeb48-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="aeb48-108">Om du konfigurerar automatiska registreringar i din lokala Active Directory måste du dessutom vara administratör för Active Directory och AD FS (om tillämpligt).</span><span class="sxs-lookup"><span data-stu-id="aeb48-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="aeb48-109">Mer information om hur du kan lösa eventuella problem med hybridanslutning finns i [Felsöka hybridanslutning](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). För att konfigurera hybrid Azure AD-anslutningar och hantera enheter med hjälp av Azure Ad-portalen, gå till [Konfigurera hybrid Azure AD-anslutna (lokala domänanslutna) enheter](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) och [Hantera enheter med hjälp av Azure-portalen](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="aeb48-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="aeb48-110">Information om hur du löser vanliga problem med hybridanslutningen för Azure Active Directory (AD) finns [Vanliga frågor och svar om hybrid Azure AD-anslutning](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="aeb48-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
