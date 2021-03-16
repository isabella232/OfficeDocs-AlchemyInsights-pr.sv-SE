---
title: Felsöka sömlös enkel inloggning (SSO) för lokal
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816348"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="00671-102">Felsöka sömlös enkel inloggning (SSO) för lokal</span><span class="sxs-lookup"><span data-stu-id="00671-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="00671-103">Så här löser du problem med sömlös enkel inloggning (SSO):</span><span class="sxs-lookup"><span data-stu-id="00671-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="00671-104">**Hur för jag över Kerberos-dekrypteringsnyckeln för AZUREADSSO-datorkontot?**</span><span class="sxs-lookup"><span data-stu-id="00671-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="00671-105">Vi rekommenderar att du för över Kerberos-dekrypteringsnyckeln minst var 30:e dag.</span><span class="sxs-lookup"><span data-stu-id="00671-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="00671-106">Mer information om hur du gör det [manuellt finns i Så här för du över Kerberos-dekrypteringstangenter.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)</span><span class="sxs-lookup"><span data-stu-id="00671-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="00671-107">**Konfigurera sömlös enkel inloggning**</span><span class="sxs-lookup"><span data-stu-id="00671-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="00671-108">Om du vill distribuera sömlös enkel inloggning följer du stegen i Sömlös enkel [inloggning i Azure Active Directory: Snabbstart.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)</span><span class="sxs-lookup"><span data-stu-id="00671-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="00671-109">**Rådgivning**</span><span class="sxs-lookup"><span data-stu-id="00671-109">**Advisory**</span></span>

- <span data-ttu-id="00671-110">[Smidig enkel inloggning i Azure Active Directory:](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) Vanliga frågor och svar – I den här artikeln besvarar vi vanliga frågor och svar om sömlös enkel inloggning i Azure Active Directory Sign-On (Seamless SSO).</span><span class="sxs-lookup"><span data-stu-id="00671-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="00671-111">Återse nytt innehåll.</span><span class="sxs-lookup"><span data-stu-id="00671-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="00671-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) – Den här artikeln innehåller information om hur du begär funktioner eller ställer tekniska frågor om sömlös enkel inloggning.</span><span class="sxs-lookup"><span data-stu-id="00671-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="00671-113">**Felsökning**</span><span class="sxs-lookup"><span data-stu-id="00671-113">**Troubleshoot**</span></span>

<span data-ttu-id="00671-114">[Felsöka sömlös enkel](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) inloggning i Azure Active Directory – den här artikeln hjälper dig att hitta felsökningsinformation om vanliga problem med sömlös enkel Sign-On inloggning i Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="00671-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







