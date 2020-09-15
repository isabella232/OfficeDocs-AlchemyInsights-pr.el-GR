---
title: Λήξη πιστοποιητικού Ομοσπονδίας ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686714"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="50608-102">Λήξη πιστοποιητικού Ομοσπονδίας ADFS</span><span class="sxs-lookup"><span data-stu-id="50608-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="50608-103">Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="50608-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="50608-104">Εγκαταστήστε τη λειτουργική μονάδα Microsoft Azure Active Directory για Windows PowerShell στον υπολογιστή (εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένη).</span><span class="sxs-lookup"><span data-stu-id="50608-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="50608-105">Για να το κάνετε αυτό, μεταβείτε στη [Διαχείριση AD Azure χρησιμοποιώντας το Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="50608-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="50608-106">Ακολουθήστε τα βήματα που περιγράφονται στην ενότητα "σενάριο 1: το πιστοποιητικό υπογραφής διακριτικού AD FS έχει λήξει" του [σφάλματος "Παρουσιάστηκε πρόβλημα κατά την πρόσβαση στην τοποθεσία" από το AD FS όταν ένας χρήστης ομόσπονδη συνδέεται στο Microsoft 365, το Azure ή το Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="50608-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="50608-107">Ακολουθήστε τα βήματα στην [ενότητα Ενημέρωση ή επιδιόρθωση των ρυθμίσεων ενός τομέα ομόσπονδη στο Microsoft, το Azure ή το Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="50608-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="50608-108">Για να μάθετε περισσότερα σχετικά με την ανανέωση των πιστοποιητικών Ομοσπονδίας, ανατρέξτε στο θέμα [Ανανέωση πιστοποιητικών Ομοσπονδίας για το Microsoft 365 και το Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="50608-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
