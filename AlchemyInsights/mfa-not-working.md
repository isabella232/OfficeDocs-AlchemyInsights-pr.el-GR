---
title: Θέματα με τη ΜΧΣ
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545166"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="4cbc1-102">Θέματα με τη ΜΧΣ</span><span class="sxs-lookup"><span data-stu-id="4cbc1-102">Issues with MFA</span></span>
<span data-ttu-id="4cbc1-103">Υπάρχουν μερικά πράγματα για να ελέγξετε αν οι χρήστες δεν μπορούν να συνδεθούν χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων (ΣΠΙ)</span><span class="sxs-lookup"><span data-stu-id="4cbc1-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="4cbc1-104">Ο χρήστης που επηρεάζεται ενδέχεται να αποκλειστεί στην πύλη Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4cbc1-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="4cbc1-105">Σε αυτήν την περίπτωση, οι απόπειρες ελέγχου ταυτότητας για τον συγκεκριμένο χρήστη θα απορρίπτονται αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="4cbc1-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="4cbc1-106">Ακολουθήστε τα βήματα σε αυτό το άρθρο για να καταργήσετε τον αποκλεισμό τους.</span><span class="sxs-lookup"><span data-stu-id="4cbc1-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="4cbc1-107">Εάν ξεμπλοκάρισμα ο χρήστης δεν βοήθησε ή ο χρήστης δεν είναι αποκλεισμένη μπορείτε να προσπαθήσετε να επαναφέρετε ΣΠΙ για το χρήστη και θα περάσουν από τη διαδικασία εγγραφής και πάλι.</span><span class="sxs-lookup"><span data-stu-id="4cbc1-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="4cbc1-108">Ακολουθήστε τα βήματα σε αυτό το άρθρο.</span><span class="sxs-lookup"><span data-stu-id="4cbc1-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="4cbc1-109">Εάν αυτή είναι η πρώτη φορά που ενεργοποιήσατε τη ΜΧΣ και οι χρήστες σας δεν είναι σε θέση να συνδεθείτε σε προγράμματα-πελάτες που δεν είναι προγράμματα περιήγησης, όπως το Outlook, Skype, κλπ, ίσως δεν είναι ενεργοποιημένο (βιβλιοθήκη ελέγχου ταυτότητας Active Directory) στη συνδρομή σας O365.</span><span class="sxs-lookup"><span data-stu-id="4cbc1-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="4cbc1-110">Σε αυτήν την περίπτωση θα πρέπει να συνδεθείτε με το Exchange Online PowerShell και να εκτελέσετε αυτό το cmdlet:  *set-οργάνωση config-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="4cbc1-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>