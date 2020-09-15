---
title: Προβλήματα κατά την είσοδο σε εφαρμογές του Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695323"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="fc107-102">Επιδιόρθωση των εφαρμογών του Microsoft 365 "Λυπούμαστε, ένας άλλος λογαριασμός από τον οργανισμό σας έχει ήδη εισέλθει στο" μήνυμα</span><span class="sxs-lookup"><span data-stu-id="fc107-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="fc107-103">Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="fc107-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="fc107-104">Καταργήστε όλους τους λογαριασμούς εργασίας, εκτός από τον επηρεαζόμενο λογαριασμό, χρησιμοποιώντας τις ρυθμίσεις των Windows > την **εργασία ή το σχολείο της Access**.</span><span class="sxs-lookup"><span data-stu-id="fc107-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="fc107-105">[Καταργήστε τα διαπιστευτήρια του Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.</span><span class="sxs-lookup"><span data-stu-id="fc107-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="fc107-106">**Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16,0.</span><span class="sxs-lookup"><span data-stu-id="fc107-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="fc107-107">(Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="fc107-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="fc107-108">Ανοίξτε μια εφαρμογή του Office, επιλέξτε Έξοδος λογαριασμού **αρχείου**  >  **Account**  >  **Sign Out**. Στη συνέχεια, συνδεθείτε χρησιμοποιώντας ένα λογαριασμό χρήστη με μια έγκυρη άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="fc107-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="fc107-109">Για περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα [Λογαριασμοί στο Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="fc107-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="fc107-110">Για Mac, ανατρέξτε στο θέμα [Δεν μπορώ να συνδεθώ σε μια εφαρμογή Office 2016 για Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="fc107-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="fc107-111">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Λυπούμαστε, ένας άλλος λογαριασμός από τον οργανισμό σας έχει ήδη εισέλθει σε αυτόν τον υπολογιστή" στο Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="fc107-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>