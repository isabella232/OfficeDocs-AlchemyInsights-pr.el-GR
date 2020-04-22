---
title: ADFS Πιστοποιητικό Ομοσπονδίας Λήξη
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710407"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Πιστοποιητικό Ομοσπονδίας Λήξη

Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:
  
1. Εγκαταστήστε τη λειτουργική μονάδα της υπηρεσίας καταλόγου Microsoft Azure Active Directory για το Windows PowerShell στον υπολογιστή (εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένη). Για να το κάνετε αυτό, μεταβείτε στην [ενότητα Διαχείριση διαφήμισης Azure χρησιμοποιώντας το Windows PowerShell](https://aka.ms/aadposh).

2. Ακολουθήστε τα βήματα στην ενότητα "Σενάριο 1: Το πιστοποιητικό υπογραφής διακριτικού AD FS έληξε" του [σφάλματος "Παρουσιάστηκε πρόβλημα κατά την πρόσβαση στην τοποθεσία" από το AD FS όταν ένας ομόσπονδος χρήστης συνδεθεί στο Microsoft 365, το Azure ή το Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Ακολουθήστε τα βήματα στο θέμα [Ενημέρωση ή επιδιόρθωση των ρυθμίσεων ενός ομόσπονδου τομέα στη Microsoft, το Azure ή το Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Για να μάθετε περισσότερα σχετικά με την ανανέωση πιστοποιητικών ομοσπονδίας, ανατρέξτε στο θέμα [Ανανέωση πιστοποιητικών ομοσπονδίας για το Microsoft 365 και την υπηρεσία καταλόγου Active Directory Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
