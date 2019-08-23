---
title: Ζητήματα με ΣΠΙ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545166"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="7df45-102">Ζητήματα με ΣΠΙ</span><span class="sxs-lookup"><span data-stu-id="7df45-102">Issues with MFA</span></span>
<span data-ttu-id="7df45-103">Υπάρχουν μερικά πράγματα που πρέπει να ελέγξετε αν οι χρήστες δεν είναι δυνατό να συνδεθεί χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων (ΣΠΙ)</span><span class="sxs-lookup"><span data-stu-id="7df45-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="7df45-104">Ο χρήστης που έχει επηρεαστεί μπορεί να έχει αποκλειστεί στο Active Directory Azure στο εμπόριο.</span><span class="sxs-lookup"><span data-stu-id="7df45-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="7df45-105">Εάν συμβαίνει αυτό, ο έλεγχος ταυτότητας επιχειρεί ότι συγκεκριμένος χρήστης δεν θα έχει αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="7df45-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="7df45-106">Ακολουθήστε τα βήματα σε αυτό το άρθρο για να καταργήσετε τον αποκλεισμό τους.</span><span class="sxs-lookup"><span data-stu-id="7df45-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="7df45-107">Εάν η κατάργηση του αποκλεισμού του χρήστη δεν σας βοήθησε ή ο χρήστης δεν αποκλείεται να δοκιμάσετε να επαναφέρετε ΣΠΙ για το χρήστη και θα μεταβούν στη διαδικασία εγγραφή ξανά.</span><span class="sxs-lookup"><span data-stu-id="7df45-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="7df45-108">Ακολουθήστε τα βήματα σε αυτό το άρθρο.</span><span class="sxs-lookup"><span data-stu-id="7df45-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="7df45-109">Εάν αυτή είναι η πρώτη φορά που δεν ΣΠΙ ενεργοποιημένο και οι χρήστες σας είναι δυνατό να συνδεθείτε στους υπολογιστές-πελάτες δεν είναι προγράμματα περιήγησης όπως το Outlook, Skype, κλπ, ίσως ADAL (βιβλιοθήκη ελέγχου ταυτότητας Active Directory) δεν είναι ενεργοποιημένη για τη συνδρομή σας O365.</span><span class="sxs-lookup"><span data-stu-id="7df45-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="7df45-110">Στην περίπτωση αυτή θα πρέπει να συνδεθείτε με το Exchange Online Powershell και να εκτελέσετε αυτό το cmdlet:  *σύνολο-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="7df45-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>