---
title: Προβλήματα κατά την είσοδο σε εφαρμογές του Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833075"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="3a774-102">Επιδιόρθωση των εφαρμογών Microsoft 365 "Λυπούμαστε, ένας άλλος λογαριασμός από την εταιρεία σας έχει ήδη συνδεθεί"</span><span class="sxs-lookup"><span data-stu-id="3a774-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="3a774-103">Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="3a774-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="3a774-104">Καταργήστε όλους τους λογαριασμούς εργασίας, εκτός από τον λογαριασμό που επηρεάζεται, χρησιμοποιώντας τις Ρυθμίσεις των Windows > **access στην εργασία ή το σχολείο.**</span><span class="sxs-lookup"><span data-stu-id="3a774-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="3a774-105">[Καταργήστε τα διαπιστευτήρια του Office χρησιμοποιώντας](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) τη Διαχείριση διαπιστευτηρίων των Windows.</span><span class="sxs-lookup"><span data-stu-id="3a774-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="3a774-106">**Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0.</span><span class="sxs-lookup"><span data-stu-id="3a774-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3a774-107">(Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="3a774-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="3a774-108">Ανοίξτε μια εφαρμογή του Office, επιλέξτε  >  **"Είσοδος**  >  **λογαριασμού αρχείου".** Στη συνέχεια, πραγματοποιήστε είσοδο χρησιμοποιώντας ένα λογαριασμό χρήστη με έγκυρη άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="3a774-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="3a774-109">Για περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα [Λογαριασμοί στο Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="3a774-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="3a774-110">Για Mac, ανατρέξτε στο θέμα [Δεν μπορώ να συνδεθώ σε μια εφαρμογή Office 2016 για Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="3a774-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="3a774-111">Για περισσότερες πληροφορίες, [ανατρέξτε στο θέμα "Λυπούμαστε, ένας άλλος](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)λογαριασμός από την εταιρεία σας έχει ήδη εισέλθει σε αυτόν τον υπολογιστή" στο Office.</span><span class="sxs-lookup"><span data-stu-id="3a774-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>