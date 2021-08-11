---
title: Δοκιμή ρύθμισης παραμέτρων IRM για νέες δυνατότητες OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812435"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Δοκιμή ρύθμισης παραμέτρων IRM για νέες δυνατότητες OME

Για να επαληθεύσετε ότι ο Microsoft 365 σας έχει ρυθμιστεί ώστε να χρησιμοποιεί νέες δυνατότητες OME, εκτελέστε τα ακόλουθα cmdlet ενώ είστε συνδεδεμένοι [στο Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Ελέγξτε τη ρύθμιση παραμέτρων IRM του μισθωτή σας εκτελώντας `Get-IRMConfiguration` το . Βεβαιωθείτε ότι αυτές οι τιμές έχουν οριστεί σε **True:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Χρησιμοποιώντας τον τομέα, τη διεύθυνση αποστολέα και τον παραλήπτη, εκτελέστε `Test-IRMConfiguration` το . Εάν ο έλεγχος δεν περάσει, διερευνάτε τη ρύθμιση παραμέτρων IRM.

Για περισσότερες πληροφορίες σχετικά με τον τρόπο επαλήθευσης της ρύθμισης παραμέτρων IRM, ανατρέξτε στο θέμα Επαλήθευση νέας ρύθμισης [παραμέτρων OME Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)