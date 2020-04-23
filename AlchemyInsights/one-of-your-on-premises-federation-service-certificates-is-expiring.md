---
title: Ένα από τα πιστοποιητικά ομοσπονδιακής υπηρεσίας εσωτερικής εγκατάστασης λήγει
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785303"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Ένα από τα πιστοποιητικά ομοσπονδιακής υπηρεσίας εσωτερικής εγκατάστασης λήγει

Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:
  
- Εγκαταστήστε τη λειτουργική μονάδα της υπηρεσίας καταλόγου Microsoft Azure Active Directory για το Windows PowerShell στον υπολογιστή (εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένη). Για να το κάνετε αυτό, μεταβείτε στο [Azure Active Directory PowerShell για το γράφημα](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Ακολουθήστε τα βήματα στην ενότητα "Σενάριο 1: Το πιστοποιητικό υπογραφής διακριτικού AD FS έληξε" του [σφάλματος "Παρουσιάστηκε πρόβλημα κατά την πρόσβαση στην τοποθεσία" από το AD FS όταν ένας ομόσπονδος χρήστης συνδεθεί στο Microsoft 365, το Azure ή το Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Ακολουθήστε τα βήματα στο [θέμα Τρόπος ενημέρωσης ή επιδιόρθωσης των ρυθμίσεων ενός ομόσπονδου τομέα στο Microsoft 365, το Azure ή το Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Για περισσότερες πληροφορίες σχετικά με την ανανέωση πιστοποιητικών ομοσπονδίας, ανατρέξτε στο θέμα [Ανανέωση πιστοποιητικού για O365 και Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

