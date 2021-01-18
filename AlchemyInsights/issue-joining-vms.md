---
title: Problem med att ansluta till virtuella datorer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885660"
---
# <a name="issue-joining-vms"></a>Problem med att ansluta till virtuella datorer

Så här löser du problem som uppstår när du försöker ansluta till virtuella datorer:

1. Försök att logga in med **UPN** -formatet (till exempel "joeuser@contoso.com") i stället för **sAMAccountName** -formatet ("CONTOSO\joeuser").
2. Kontrol lera att du har aktiverat Lösenordssynkronisering enligt anvisningarna i *komma igång* -guiden.
3. Kontrol lera att det användar konto som påverkas inte är ett externt konto i Azure AD-innehavaren. Externa användare kan inte logga in på den hanterade domänen eftersom Azure AD Domain Services inte har autentiseringsuppgifter för sådana användar konton.
4. Om det berörda användar kontot är ett moln-Only-konto kontrollerar du att användarna har ändrat sitt lösen ord efter att du aktiverat Azure AD Domain Services. Det här steget gör att hash-värden för autentiseringsuppgifter krävs för att Azure AD Domain Services ska kunna genereras.
5. Om de berörda användar kontona synkroniseras från en lokal katalog kontrollerar du att Rekommenderad version av Azure AD Connect har kon figurer ATS för en fullständig synkronisering.
6. Om problemen kvarstår efter att du har bekräftat steg 4 kör du följande kommandon från synkkabeln:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.