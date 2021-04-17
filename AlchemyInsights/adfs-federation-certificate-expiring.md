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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="2b453-102">Λήξη πιστοποιητικού ομοσπονδίας ADFS</span><span class="sxs-lookup"><span data-stu-id="2b453-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="2b453-103">Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="2b453-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="2b453-104">Εγκαταστήστε τη λειτουργική μονάδα Microsoft Azure Active Directory για Windows PowerShell στον υπολογιστή (εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένη).</span><span class="sxs-lookup"><span data-stu-id="2b453-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="2b453-105">Για να το κάνετε αυτό, μεταβείτε στη [διαχείριση του Azure AD χρησιμοποιώντας το Windows PowerShell.](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="2b453-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="2b453-106">Ακολουθήστε τα βήματα στην ενότητα "Σενάριο 1: Το πιστοποιητικό υπογραφής διακριτικού AD FS έληξε" του σφάλματος "Παρουσιάστηκε πρόβλημα κατά την πρόσβαση στην τοποθεσία" από τις υπηρεσίες AD FS όταν ένας ομόσπονδος χρήστης κάνει είσοδο στο [Microsoft 365, το Azure ή το Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="2b453-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="2b453-107">Ακολουθήστε τα βήματα στην [ενημέρωση ή επιδιορθώστε τις ρυθμίσεις ενός ομόσπονδου τομέα στο Microsoft, το Azure ή το Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="2b453-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="2b453-108">Για να μάθετε περισσότερα σχετικά με την ανανέωση πιστοποιητικών ομοσπονδίας, ανατρέξτε στο θέμα [Ανανέωση πιστοποιητικών ομοσπονδίας για το Microsoft 365 και το Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="2b453-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
