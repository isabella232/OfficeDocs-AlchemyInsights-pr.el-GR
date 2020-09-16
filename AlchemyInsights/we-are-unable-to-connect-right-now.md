---
title: Πρόβλημα ενεργοποίησης-δεν είναι δυνατή η σύνδεση αυτή τη στιγμή
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725983"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="baf20-102">Μήνυμα για τη διόρθωση των εφαρμογών Microsoft 365 "δεν είναι δυνατή η σύνδεση αυτή τη στιγμή"</span><span class="sxs-lookup"><span data-stu-id="baf20-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="baf20-103">Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="baf20-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="baf20-104">Επιλέξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις του διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet στις εφαρμογές Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="baf20-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="baf20-105">Ανατρέξτε στο θέμα [διευθύνσεις URL και περιοχές διευθύνσεων IP του Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="baf20-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="baf20-106">Μεταβείτε στην **Έναρξη**  >  **εκτέλεση**και, στη συνέχεια, πληκτρολογήστε **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="baf20-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="baf20-107">Βεβαιωθείτε ότι όλες οι υπηρεσίες που ακολουθούν εκτελούνται:</span><span class="sxs-lookup"><span data-stu-id="baf20-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="baf20-108">Αυτόματη ρύθμιση συσκευών με σύνδεση δικτύου</span><span class="sxs-lookup"><span data-stu-id="baf20-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="baf20-109">Υπηρεσία λίστας δικτύου</span><span class="sxs-lookup"><span data-stu-id="baf20-109">Network List Service</span></span>
    - <span data-ttu-id="baf20-110">Συνειδητοποίηση τοποθεσίας δικτύου</span><span class="sxs-lookup"><span data-stu-id="baf20-110">Network Location Awareness</span></span>
    - <span data-ttu-id="baf20-111">Αρχείο καταγραφής συμβάντων των Windows</span><span class="sxs-lookup"><span data-stu-id="baf20-111">Windows Event Log</span></span>

<span data-ttu-id="baf20-112">Εάν μία από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την εκκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="baf20-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="baf20-113">Εάν αντιμετωπίζετε πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή, ανοίγοντας μια γραμμή εντολών με αναβαθμισμένα δικαιώματα:</span><span class="sxs-lookup"><span data-stu-id="baf20-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="baf20-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="baf20-114">**sfc /scannow**</span></span>

<span data-ttu-id="baf20-115">Μετά την ολοκλήρωση αυτής της εντολής, επανεκκινήστε τον υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="baf20-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="baf20-116">Για λεπτομερείς πληροφορίες, ανατρέξτε [στο θέμα "Λυπούμαστε, δεν είναι δυνατή η σύνδεση με το λογαριασμό σας. Παρακαλούμε δοκιμάστε ξανά αργότερα "σφάλμα κατά την ενεργοποίηση του Office από το Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="baf20-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>