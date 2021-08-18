---
title: Blockera eller avblockera extern automatisk vidarebefordran av e-post
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315892"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blockera eller avblockera automatisk vidarebefordran av e-post

Information om hur du aktiverar eller inaktiverar vidarebefordran av e-post för en viss postlåda finns i [Konfigurera vidarebefordran av e-post.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Administratörer kan styra extern vidarebefordran för organisationen med hjälp av [principer för utgående skräppost.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Du hanterar principer för utgående skräppost i Microsoft 365 Defender-portalen på eller med <https://security.microsoft.com/antispam> cmdleten [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) i Exchange Online PowerShell.

Om du får följande felmeddelande: **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**, kontrollerar du att principen är konfigurerad för att aktivera externa meddelanden som vidarebefordras automatiskt.

**Obs!** Vi rekommenderade standardvärdet Automatisk –  **System** reglerad för inställningen Automatiska vidarebeskickningsregler i standardprincipen för skräppostfilter för utgående trafik (automatisk extern vidarebefordran blockeras, intern automatisk vidarebefordran fungerar fortfarande). Du bör skapa egna principer för skräppostfilter och använda värdet På **– Vidarebefordran** är endast aktiverat för användare som behöver extern automatisk vidarebefordran av e-post. Mer information finns i Konfigurera [vidarebefordran av extern e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
