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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952969"
---
# <a name="adfs-federation-certificate-expiring"></a>Λήξη πιστοποιητικού ομοσπονδίας ADFS

Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:
  
1. Εγκαταστήστε Microsoft Azure Active Directory λειτουργική μονάδα Windows PowerShell στον υπολογιστή (εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένη). Για να το κάνετε αυτό, μεταβείτε [στη διαχείριση του Azure AD χρησιμοποιώντας Windows PowerShell.](https://aka.ms/aadposh)

2. Ακολουθήστε τα βήματα στην ενότητα "Σενάριο 1: Το πιστοποιητικό υπογραφής διακριτικών AD FS έληξε" του σφάλματος "Παρουσιάστηκε πρόβλημα κατά την πρόσβαση στην τοποθεσία" από τις υπηρεσίες AD FS όταν ένας ομόσπονδος χρήστης κάνει είσοδο στο Microsoft 365, το [Azure ή το Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Ακολουθήστε τα βήματα στην [ενημέρωση ή επιδιορθώστε τις ρυθμίσεις ενός ομόσπονδου τομέα στο Microsoft, το Azure ή το Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Για να μάθετε περισσότερα σχετικά με την ανανέωση πιστοποιητικών ομοσπονδίας, ανατρέξτε στο θέμα Ανανέωση πιστοποιητικών [ομοσπονδίας για Microsoft 365 και Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
