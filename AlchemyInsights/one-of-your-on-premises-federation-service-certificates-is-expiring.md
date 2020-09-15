---
title: Ένα από τα πιστοποιητικά υπηρεσίας Ομοσπονδία εσωτερικής εγκατάστασης λήγει
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673497"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="1f90d-102">Ένα από τα πιστοποιητικά υπηρεσίας Ομοσπονδία εσωτερικής εγκατάστασης λήγει</span><span class="sxs-lookup"><span data-stu-id="1f90d-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="1f90d-103">Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="1f90d-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="1f90d-104">Εγκαταστήστε τη λειτουργική μονάδα Microsoft Azure Active Directory για Windows PowerShell στον υπολογιστή (εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένη).</span><span class="sxs-lookup"><span data-stu-id="1f90d-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="1f90d-105">Για να το κάνετε αυτό, μεταβείτε στο αρχείο [PowerShell του Azure Active Directory για το Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="1f90d-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="1f90d-106">Ακολουθήστε τα βήματα που περιγράφονται στην ενότητα "σενάριο 1: το πιστοποιητικό υπογραφής διακριτικού AD FS έχει λήξει" του [σφάλματος "Παρουσιάστηκε πρόβλημα κατά την πρόσβαση στην τοποθεσία" από το AD FS όταν ένας χρήστης ομόσπονδη συνδέεται στο Microsoft 365, το Azure ή το Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="1f90d-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="1f90d-107">Ακολουθήστε τα βήματα στον [τρόπο με τον οποίο μπορείτε να ενημερώσετε ή να επιδιορθώσετε τις ρυθμίσεις ενός τομέα ομόσπονδη στο Microsoft 365, το Azure ή το Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="1f90d-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="1f90d-108">Για περισσότερες πληροφορίες σχετικά με την ανανέωση των πιστοποιητικών Ομοσπονδίας, ανατρέξτε στο θέμα [Ανανέωση πιστοποιητικού για το O365 και το Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="1f90d-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

