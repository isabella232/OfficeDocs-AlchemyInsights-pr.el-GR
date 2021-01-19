---
title: Θέματα συναίνεσης διαχειριστή
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901129"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="dd63c-102">Θέματα συναίνεσης διαχειριστή</span><span class="sxs-lookup"><span data-stu-id="dd63c-102">Admin consent issues</span></span>

1. <span data-ttu-id="dd63c-103">Ενεργοποιήστε τη [ροή εργασίας συναίνεσης διαχειριστή](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) για να επιτρέψετε στους χρήστες να ζητούν έγκριση διαχειριστή απευθείας από την οθόνη συγκατάθεσης.</span><span class="sxs-lookup"><span data-stu-id="dd63c-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="dd63c-104">Εάν εσείς ή οι χρήστες της εφαρμογής σας βλέπετε μη αναμενόμενα σφάλματα κατά τη διαδικασία συναίνεσης, ανατρέξτε σε αυτό το άρθρο για τα βήματα αντιμετώπισης προβλημάτων: [μη αναμενόμενο σφάλμα κατά την εκτέλεση συναίνεσης σε μια εφαρμογή](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="dd63c-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="dd63c-105">Μάθετε περισσότερα σχετικά με [τη συναίνεση διαχειριστή στην πλατφόρμα ταυτοτήτων της Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), τον τρόπο λειτουργίας της [προτροπής συναίνεσης](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) και τον τρόπο με τον οποίο μπορείτε να [αξιολογήσετε μια αίτηση συναίνεσης διαχειριστή σε επίπεδο μισθωτών](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="dd63c-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="dd63c-106">Οι εφαρμογές που ενσωματώνονται με την πλατφόρμα ταυτοτήτων της Microsoft ακολουθούν ένα μοντέλο εξουσιοδότησης που παρέχει στους χρήστες και τους διαχειριστές τον έλεγχο του τρόπου με τον οποίο είναι δυνατή η πρόσβαση στα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="dd63c-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="dd63c-107">Η εφαρμογή του μοντέλου εξουσιοδότησης έχει ενημερωθεί στο τελικό σημείο της πλατφόρμας ταυτοτήτων της Microsoft και αλλάζει τον τρόπο με τον οποίο μια εφαρμογή πρέπει να αλληλεπιδρά με την πλατφόρμα ταυτοτήτων της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dd63c-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="dd63c-108">Ανατρέξτε [στο θέμα δικαιώματα και συγκατάθεση στο τελικό σημείο της πλατφόρμας ταυτότητας της Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) για μια επισκόπηση αυτού του μοντέλου εξουσιοδότησης, συμπεριλαμβανομένων των εύρους, των δικαιωμάτων και της συγκατάθεσης.</span><span class="sxs-lookup"><span data-stu-id="dd63c-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>