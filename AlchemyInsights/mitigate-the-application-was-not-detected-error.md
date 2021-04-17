---
title: Αντιμετώπιση του σφάλματος "Η εφαρμογή δεν εντοπίστηκε"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836351"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="7346b-102">Αντιμετώπιση του σφάλματος "Η εφαρμογή δεν εντοπίστηκε"</span><span class="sxs-lookup"><span data-stu-id="7346b-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="7346b-103">Το σφάλμα εγκατάστασης εφαρμογής, "Η εφαρμογή δεν εντοπίστηκε μετά την επιτυχή ολοκλήρωση της εγκατάστασης", που αναφέρθηκε από το Intune, ενδέχεται να προκύψει σε όλες τις μεγάλες πλατφόρμες λειτουργικών συστημάτων (Windows, iOS και Android).</span><span class="sxs-lookup"><span data-stu-id="7346b-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="7346b-104">Τα πιο συνηθισμένα σενάρια που δημιουργούν αυτό το σφάλμα είναι τα εξής:</span><span class="sxs-lookup"><span data-stu-id="7346b-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="7346b-105">Η εφαρμογή ενημερώθηκε εκτός του Intune (από ένα κατάστημα εφαρμογών τρίτου κατασκευαστή) μετά την αρχική ανάπτυξη.</span><span class="sxs-lookup"><span data-stu-id="7346b-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="7346b-106">Για παράδειγμα, ορισμένες εφαρμογές, όπως το Google Chrome, ενδέχεται να εκτελούν αυτόματες ενημερώσεις.</span><span class="sxs-lookup"><span data-stu-id="7346b-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="7346b-107">Ένας χρήστης έχει καταργήσει την εφαρμογή μετά την αρχική εγκατάσταση.</span><span class="sxs-lookup"><span data-stu-id="7346b-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="7346b-108">Για να αντιμετωπίσετε αυτό το πρόβλημα, εκτελέστε πρώτα μια αναθεώρηση των επηρεαζόμενων συσκευών για να προσδιορίσετε το σενάριο που οφείλεται για τη δημιουργία του σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="7346b-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="7346b-109">Εάν η εφαρμογή έχει ενημερωθεί εκτός του Intune, η ανάπτυξη εφαρμογών μπορεί να ρυθμιστεί ώστε να παραβλέπει την έκδοση της εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="7346b-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="7346b-110">Για να το κάνετε αυτό, στην επιλογή **Ρύθμιση παραμέτρων της εφαρμογής > Πληροφορίες εφαρμογής**, ορίστε **Παράβλεψη της έκδοσης εφαρμογής** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="7346b-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="7346b-111">Όταν στοχεύετε στον πελάτη, μπορεί να είναι καλύτερο να εγκαταστήσετε την εφαρμογή ως "υποχρεωτικό" και να διασφαλίσετε ότι γίνεται εγκατάστασης της πιο πρόσφατης έκδοσης.</span><span class="sxs-lookup"><span data-stu-id="7346b-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="7346b-112">Εναλλακτικά, στην πλατφόρμα iOS, μπορείτε να χρησιμοποιήσετε την **λειτουργικότητα αυτόματης ενημέρωσης** που σχετίζεται με το Apple Volume Purchase Program, το οποίο μπορεί να ρυθμιστεί ώστε να ενημερώνεται αυτόματα σε νέες εκδόσεις εφαρμογών καθώς καθίστανται διαθέσιμες.</span><span class="sxs-lookup"><span data-stu-id="7346b-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="7346b-113">Για περισσότερες πληροφορίες σχετικά με την αντιμετώπιση προβλημάτων εγκατάστασης εφαρμογών, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων εγκατάστασης εφαρμογών](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="7346b-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
