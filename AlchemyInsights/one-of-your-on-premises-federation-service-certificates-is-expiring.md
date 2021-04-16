---
title: Ένα από τα πιστοποιητικά υπηρεσίας ομοσπονδίας εσωτερικής εγκατάστασης λήγει
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810052"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="baf8e-102">Ένα από τα πιστοποιητικά υπηρεσίας ομοσπονδίας εσωτερικής εγκατάστασης λήγει</span><span class="sxs-lookup"><span data-stu-id="baf8e-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="baf8e-103">Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="baf8e-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="baf8e-104">Εγκαταστήστε τη λειτουργική μονάδα Microsoft Azure Active Directory για Windows PowerShell στον υπολογιστή (εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένη).</span><span class="sxs-lookup"><span data-stu-id="baf8e-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="baf8e-105">Για να το κάνετε αυτό, μεταβείτε στο [Azure Active Directory PowerShell για Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="baf8e-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="baf8e-106">Ακολουθήστε τα βήματα στην ενότητα "Σενάριο 1: Το πιστοποιητικό υπογραφής διακριτικού AD FS έληξε" του σφάλματος "Παρουσιάστηκε πρόβλημα κατά την πρόσβαση στην τοποθεσία" από τις υπηρεσίες AD FS όταν ένας ομόσπονδος χρήστης κάνει είσοδο στο [Microsoft 365, το Azure ή το Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="baf8e-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="baf8e-107">Ακολουθήστε τα βήματα στο άρθρο Πώς μπορείτε να ενημερώσετε ή να επιδιορθώσετε τις ρυθμίσεις ενός ομόσπονδου τομέα [στο Microsoft 365, το Azure ή το Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)</span><span class="sxs-lookup"><span data-stu-id="baf8e-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="baf8e-108">Για περισσότερες πληροφορίες σχετικά με την ανανέωση πιστοποιητικών ομοσπονδίας, ανατρέξτε στο θέμα [Ανανέωση πιστοποιητικού για το O365 και το Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="baf8e-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

