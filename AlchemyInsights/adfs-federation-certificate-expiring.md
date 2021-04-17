---
title: Λήξη πιστοποιητικού ομοσπονδίας ADFS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821951"
---
# <a name="adfs-federation-certificate-expiring"></a>Λήξη πιστοποιητικού ομοσπονδίας ADFS

Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:
  
1. Εγκαταστήστε τη λειτουργική μονάδα Microsoft Azure Active Directory για Windows PowerShell στον υπολογιστή (εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένη). Για να το κάνετε αυτό, μεταβείτε στη [διαχείριση του Azure AD χρησιμοποιώντας το Windows PowerShell.](https://aka.ms/aadposh)

2. Ακολουθήστε τα βήματα στην ενότητα "Σενάριο 1: Το πιστοποιητικό υπογραφής διακριτικού AD FS έληξε" του σφάλματος "Παρουσιάστηκε πρόβλημα κατά την πρόσβαση στην τοποθεσία" από τις υπηρεσίες AD FS όταν ένας ομόσπονδος χρήστης κάνει είσοδο στο [Microsoft 365, το Azure ή το Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Ακολουθήστε τα βήματα στην [ενημέρωση ή επιδιορθώστε τις ρυθμίσεις ενός ομόσπονδου τομέα στο Microsoft, το Azure ή το Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Για να μάθετε περισσότερα σχετικά με την ανανέωση πιστοποιητικών ομοσπονδίας, ανατρέξτε στο θέμα [Ανανέωση πιστοποιητικών ομοσπονδίας για το Microsoft 365 και το Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
