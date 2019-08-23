---
title: Ένα από τα πιστοποιητικά σας υπηρεσία Ομοσπονδία εσωτερικής εγκατάστασης λήγει
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543565"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="d6db6-102">Ένα από τα πιστοποιητικά σας υπηρεσία Ομοσπονδία εσωτερικής εγκατάστασης λήγει</span><span class="sxs-lookup"><span data-stu-id="d6db6-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="d6db6-103">Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="d6db6-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="d6db6-104">Εγκαταστήστε το Microsoft Azure Active Directory λειτουργική μονάδα για Windows PowerShell στον υπολογιστή (Εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένο).</span><span class="sxs-lookup"><span data-stu-id="d6db6-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="d6db6-105">Για να γίνει αυτό, μεταβείτε στο [Azure Active Directory PowerShell για γράφημα](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="d6db6-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="d6db6-106">Ακολουθήστε τα βήματα του "σενάριο 1: λήξει το πιστοποιητικό υπογραφής διακριτικό AD FS" ενότητα ["Παρουσιάστηκε ένα πρόβλημα κατά την πρόσβαση στην τοποθεσία" σφάλμα από AD FS όταν μια ομόσπονδη χρήστης υπογράφει Office 365, Azure, ή Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="d6db6-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="d6db6-107">Ακολουθήστε τα βήματα της t[πώς μπορείτε να ενημερώσετε ή να επιδιορθώσετε τις ρυθμίσεις ομόσπονδη τομέα στο Office 365, Azure, ή Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="d6db6-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="d6db6-108">Για περισσότερες πληροφορίες σχετικά με την ανανέωση πιστοποιητικών Ομοσπονδία, ανατρέξτε στο θέμα [ανανέωσης πιστοποιητικού για O365 και Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="d6db6-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

