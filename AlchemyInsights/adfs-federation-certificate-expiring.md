---
title: ADFS πιστοποιητικού Ομοσπονδίας που λήγει
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737189"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS πιστοποιητικού Ομοσπονδίας που λήγει

Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:
  
1. Εγκαταστήστε τη λειτουργική μονάδα καταλόγου Active Directory Microsoft Azure για Windows PowerShell στον υπολογιστή (εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένη). Για να γίνει αυτό, μεταβείτε στη [Διαχείριση AD Azure χρησιμοποιώντας το Windows PowerShell](https://aka.ms/aadposh).

2. Ακολουθήστε τα βήματα στο "σενάριο 1: το πιστοποιητικό AD FS διακριτικού υπογραφής έληξε" ενότητα ["Παρουσιάστηκε ένα πρόβλημα κατά την πρόσβαση στην τοποθεσία" σφάλμα από AD FS όταν μια ομόσπονδης χρήστης υπογράφει στο Office 365, Azure ή Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Ακολουθήστε τα βήματα στην [ενημερωμένη έκδοση ή να επιδιορθώσετε τις ρυθμίσεις ενός ομόσπονδη τομέα στο Office 365, Azure ή Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Για να μάθετε περισσότερα σχετικά με την ανανέωση πιστοποιητικών Ομοσπονδία, ανατρέξτε [στο θέμα ανανέωση πιστοποιητικών Ομοσπονδία για το Office 365 και Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
