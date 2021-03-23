---
title: Konfigurera SCP (Service Connection Point)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037290"
---
# <a name="configure-service-connection-point-scp"></a>Konfigurera SCP (Service Connection Point)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Orsak:** Det går inte att läsa SCP-objektet och få information om Azure AD-klientorganisationen
- **Lösning:** Se avsnittet Konfigurera [en tjänstanslutningspunkt](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Handlingsplan**

- Kontrollera om enheten har fått GPO:t för kontrollerad verifiering.
- Kontrollera att GPO:t har skapat registernycklarna.
- Kontrollera att du har två nycklar skapade med ditt katalog-ID och onmicrosoft-domän.

**Konfigurera registerinställning på klientsidan för SCP**

Använd följande exempel för att skapa ett grupprincipobjekt (GPO) för att distribuera en registerinställning som konfigurerar en SCP-post i registret på dina enheter.

1. Öppna en konsol för hantering av grupprinciper och skapa ett nytt GPO på domänen.
     - Ange ditt nya GPO ett namn (till exempel ClientSideSCP)

2. Redigera GPO:t och leta reda på följande sökväg: **Datorkonfiguration > inställningar > Windows-> register**.

3. Högerklicka på registret **och** välj Ny **> registerpost.**

4. På **fliken Allmänt** konfigurerar du följande:
  
- **Åtgärd:** Uppdatera
    
- **Registreringsdatafil**: HKEY_LOCAL_MACHINE
    
- **Nyckelsökväg:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Värdenamn**: TenantId
    
- **Värdetyp:** REG_SZ
    
- **Värdedata:** GUID- eller katalog-ID för Azure AD-instansen (Det här värdet finns i **Azure Portal > Azure Active Directory > Egenskaper > Katalog-ID**)
 
- Klicka på **OK**.
 
5. Högerklicka på registret **och** välj Ny **> registerpost.**

6. På **fliken Allmänt** konfigurerar du följande:
  
- **Åtgärd:** Uppdatera
    
- **Registreringsdatafil**: HKEY_LOCAL_MACHINE
    
- **Nyckelsökväg:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Värdenamn**: TenantName
    
- **Värdetyp:** REG_SZ
    
- **Värdedata:** Ditt verifierade domännamn om du använder federerad miljö, till exempel AD FS. Ditt verifierade domännamn eller ditt onmicrosoft.com (till exempel contoso.onmicrosoft).com om du använder hanterad miljö

- Klicka på **OK**.

7. Stäng redigeraren för det nya GPO:t.

8. Länka det nya GPO:t till önskad OU som innehåller domänbaserade datorer som tillhör din kontrollerade utrullningspopulation.

Mer information finns i [Kontrollerad validering av hybrid-AD-koppling för Azure – Azure AD | Microsoft-dokument och](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) [felsökningshybrid för Azure Active Directory-anslutna enheter | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)









