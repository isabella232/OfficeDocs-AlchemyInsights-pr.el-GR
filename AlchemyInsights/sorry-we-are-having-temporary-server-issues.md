---
title: Επιδιόρθωση εφαρμογών του Office Λυπούμαστε, έχουμε προσωρινό μήνυμα ζητημάτων διακομιστή
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764117"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="343cd-102">Επιδιόρθωση του μηνύματος "Λυπούμαστε, έχουμε προσωρινά προβλήματα διακομιστή"</span><span class="sxs-lookup"><span data-stu-id="343cd-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="343cd-103">Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="343cd-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="343cd-104">Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης, για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet στις εφαρμογές του Office.</span><span class="sxs-lookup"><span data-stu-id="343cd-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="343cd-105">Ανατρέξτε [στην περιοχή URL και διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="343cd-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="343cd-106">Μεταβείτε **στην έναρξη** > **εκτέλεσης**και, στη συνέχεια, πληκτρολογήστε **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="343cd-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="343cd-107">Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:</span><span class="sxs-lookup"><span data-stu-id="343cd-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="343cd-108">Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου</span><span class="sxs-lookup"><span data-stu-id="343cd-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="343cd-109">Υπηρεσία λίστας δικτύου</span><span class="sxs-lookup"><span data-stu-id="343cd-109">Network List Service</span></span>
    - <span data-ttu-id="343cd-110">Ευαισθητοποίηση τοποθεσίας δικτύου</span><span class="sxs-lookup"><span data-stu-id="343cd-110">Network Location Awareness</span></span>
    - <span data-ttu-id="343cd-111">Αρχείο καταγραφής συμβάντων των Windows</span><span class="sxs-lookup"><span data-stu-id="343cd-111">Windows Event Log</span></span>

<span data-ttu-id="343cd-112">Εάν μία από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="343cd-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="343cd-113">Εάν αντιμετωπίσετε πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αυξημένα δικαιώματα:</span><span class="sxs-lookup"><span data-stu-id="343cd-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="343cd-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="343cd-114">**sfc /scannow**</span></span>

<span data-ttu-id="343cd-115">Μετά την ολοκλήρωση αυτής της εντολής, κάντε επανεκκίνηση του υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="343cd-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="343cd-116">Για λεπτομερείς πληροφορίες, [ανατρέξτε στην ενότητα "Λυπούμαστε, δεν μπορούμε να συνδεθούμε στο λογαριασμό σας. Προσπαθήστε ξανά αργότερα" σφάλμα κατά την ενεργοποίηση](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)του .</span><span class="sxs-lookup"><span data-stu-id="343cd-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>