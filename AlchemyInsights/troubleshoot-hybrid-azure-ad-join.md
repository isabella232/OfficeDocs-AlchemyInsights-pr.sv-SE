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
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939289"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Felsöka hybrid Azure AD-anslutning

Rekommenderas starkt för att se till att en enhet kan komma åt slutpunkter för enhetsregistrering under systemkontot genom att använda [Skriptet för att testa anslutningen för enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Om du konfigurerar enhetsregistreringar för första gången bör du läsa [Introduktion till enhetshantering i Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), för att lära dig hur du får Azure AD att kontrollera enheter.
1. Om du registrerar enheter direkt i Azure AD och registrerar dem i Intune ska du kontrollera att du har [konfigurerat Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) och har all [licensiering](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) klart först.
1. Se till att du är behörig att utföra åtgärder i Azure AD och lokala AD. Endast en global administratör i Azure AD kan hantera inställningar för enhetsregistreringar. Om du konfigurerar automatiska registreringar i din lokala Active Directory måste du dessutom vara administratör för Active Directory och AD FS (om tillämpligt).

Mer information om hur du kan lösa eventuella problem med hybridanslutning finns i [Felsöka hybridanslutning](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). För att konfigurera hybrid Azure AD-anslutningar och hantera enheter med hjälp av Azure Ad-portalen, gå till [Konfigurera hybrid Azure AD-anslutna (lokala domänanslutna) enheter](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) och [Hantera enheter med hjälp av Azure-portalen](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Information om hur du löser vanliga problem med hybridanslutningen för Azure Active Directory (AD) finns [Vanliga frågor och svar om hybrid Azure AD-anslutning](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
