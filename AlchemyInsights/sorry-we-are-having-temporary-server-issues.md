---
title: Επιδιόρθωση εφαρμογών του Microsoft 365 Δυστυχώς, έχουμε ένα μήνυμα προσωρινών προβλημάτων διακομιστή
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835271"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="f8a31-102">Επιδιόρθωση των εφαρμογών του Microsoft 365 "Λυπούμαστε, έχουμε προσωρινά προβλήματα διακομιστή"</span><span class="sxs-lookup"><span data-stu-id="f8a31-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="f8a31-103">Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="f8a31-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f8a31-104">Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet σε εφαρμογές του Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f8a31-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="f8a31-105">Δείτε [διευθύνσεις URL και περιοχές διευθύνσεων IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="f8a31-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="f8a31-106">Μεταβείτε στην **"Έναρξη**  >  **εκτέλεσης"** και, στη συνέχεια, **πληκτρολογήστε services.msc.**</span><span class="sxs-lookup"><span data-stu-id="f8a31-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="f8a31-107">Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:</span><span class="sxs-lookup"><span data-stu-id="f8a31-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="f8a31-108">Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου</span><span class="sxs-lookup"><span data-stu-id="f8a31-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="f8a31-109">Υπηρεσία λίστας δικτύου</span><span class="sxs-lookup"><span data-stu-id="f8a31-109">Network List Service</span></span>
    - <span data-ttu-id="f8a31-110">Αναγνώριση τοποθεσίας δικτύου</span><span class="sxs-lookup"><span data-stu-id="f8a31-110">Network Location Awareness</span></span>
    - <span data-ttu-id="f8a31-111">Αρχείο καταγραφής συμβάντων των Windows</span><span class="sxs-lookup"><span data-stu-id="f8a31-111">Windows Event Log</span></span>

<span data-ttu-id="f8a31-112">Εάν κάποια από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="f8a31-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="f8a31-113">Εάν έχετε κάποιο πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αναβαθμισμένα δικαιώματα:</span><span class="sxs-lookup"><span data-stu-id="f8a31-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="f8a31-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="f8a31-114">**sfc /scannow**</span></span>

<span data-ttu-id="f8a31-115">Αφού ολοκληρωθεί αυτή η εντολή, επανεκκινήστε τον υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="f8a31-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="f8a31-116">Για λεπτομερείς πληροφορίες, [ανατρέξτε στο θέμα "Λυπούμαστε, δεν είναι δυνατή η σύνδεση με το λογαριασμό σας. Προσπαθήστε ξανά αργότερα" κατά την ενεργοποίηση.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="f8a31-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>