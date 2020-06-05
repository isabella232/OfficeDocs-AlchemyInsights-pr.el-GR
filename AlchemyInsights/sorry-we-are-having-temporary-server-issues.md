---
title: Επιδιόρθωση εφαρμογών Microsoft 365 Λυπούμαστε, έχουμε προσωρινό μήνυμα ζητημάτων διακομιστή
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582703"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="ad9d0-102">Επιδιόρθωση του μηνύματος "Λυπούμαστε, έχουμε προσωρινά προβλήματα διακομιστή"</span><span class="sxs-lookup"><span data-stu-id="ad9d0-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="ad9d0-103">Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="ad9d0-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ad9d0-104">Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης, για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet σε εφαρμογές της Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ad9d0-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="ad9d0-105">Ανατρέξτε [στην περιοχή URL και διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="ad9d0-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ad9d0-106">Μεταβείτε **στην έναρξη**  >  **εκτέλεσης**και, στη συνέχεια, πληκτρολογήστε **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="ad9d0-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ad9d0-107">Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:</span><span class="sxs-lookup"><span data-stu-id="ad9d0-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ad9d0-108">Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου</span><span class="sxs-lookup"><span data-stu-id="ad9d0-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ad9d0-109">Υπηρεσία λίστας δικτύου</span><span class="sxs-lookup"><span data-stu-id="ad9d0-109">Network List Service</span></span>
    - <span data-ttu-id="ad9d0-110">Ευαισθητοποίηση τοποθεσίας δικτύου</span><span class="sxs-lookup"><span data-stu-id="ad9d0-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ad9d0-111">Αρχείο καταγραφής συμβάντων των Windows</span><span class="sxs-lookup"><span data-stu-id="ad9d0-111">Windows Event Log</span></span>

<span data-ttu-id="ad9d0-112">Εάν μία από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="ad9d0-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ad9d0-113">Εάν αντιμετωπίσετε πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αυξημένα δικαιώματα:</span><span class="sxs-lookup"><span data-stu-id="ad9d0-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ad9d0-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="ad9d0-114">**sfc /scannow**</span></span>

<span data-ttu-id="ad9d0-115">Μετά την ολοκλήρωση αυτής της εντολής, κάντε επανεκκίνηση του υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="ad9d0-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ad9d0-116">Για λεπτομερείς πληροφορίες, [ανατρέξτε στην ενότητα "Λυπούμαστε, δεν μπορούμε να συνδεθούμε στο λογαριασμό σας. Προσπαθήστε ξανά αργότερα" σφάλμα κατά την ενεργοποίηση](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)του .</span><span class="sxs-lookup"><span data-stu-id="ad9d0-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>