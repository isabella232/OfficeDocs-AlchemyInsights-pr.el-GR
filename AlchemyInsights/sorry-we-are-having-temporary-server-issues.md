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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627990"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="fab41-102">Επιδιόρθωση των εφαρμογών του Office "Λυπούμαστε, έχουμε προσωρινά ζητήματα διακομιστή" μήνυμα</span><span class="sxs-lookup"><span data-stu-id="fab41-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="fab41-103">Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="fab41-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="fab41-104">Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet σε εφαρμογές του Office.</span><span class="sxs-lookup"><span data-stu-id="fab41-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="fab41-105">Δείτε [διευθύνσεις URL του Office 365 και περιοχές διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="fab41-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="fab41-106">Μεταβείτε στην **Έναρξη** > **εκτέλεσης**και, στη συνέχεια, πληκτρολογήστε **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="fab41-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="fab41-107">Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:</span><span class="sxs-lookup"><span data-stu-id="fab41-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="fab41-108">Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου</span><span class="sxs-lookup"><span data-stu-id="fab41-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="fab41-109">Υπηρεσία λίστας δικτύου</span><span class="sxs-lookup"><span data-stu-id="fab41-109">Network List Service</span></span>
    - <span data-ttu-id="fab41-110">Ενημέρωση τοποθεσίας δικτύου</span><span class="sxs-lookup"><span data-stu-id="fab41-110">Network Location Awareness</span></span>
    - <span data-ttu-id="fab41-111">Αρχείο καταγραφής συμβάντων των Windows</span><span class="sxs-lookup"><span data-stu-id="fab41-111">Windows Event Log</span></span>

<span data-ttu-id="fab41-112">Εάν μια από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="fab41-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="fab41-113">Εάν έχετε πρόβλημα με την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αυξημένα δικαιώματα:</span><span class="sxs-lookup"><span data-stu-id="fab41-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="fab41-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="fab41-114">**sfc /scannow**</span></span>

<span data-ttu-id="fab41-115">Μετά την ολοκλήρωση αυτής της εντολής, επανεκκινήστε τον υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="fab41-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="fab41-116">Για αναλυτικές πληροφορίες, ανατρέξτε [στην «Λυπούμαστε, δεν μπορούμε να συνδεθούμε με το λογαριασμό σας. Προσπαθήστε ξανά αργότερα "σφάλμα κατά την ενεργοποίηση του Office από 365 του Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="fab41-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>