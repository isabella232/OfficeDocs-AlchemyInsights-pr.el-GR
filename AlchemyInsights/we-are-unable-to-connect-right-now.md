---
title: Ζήτημα ενεργοποίησης - Δεν είναι δυνατή η σύνδεση αυτήν τη στιγμή
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581875"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="52825-102">Επιδιόρθωση του μηνύματος "Δεν είναι δυνατή η σύνδεση των εφαρμογών microsoft 365 αυτήν τη στιγμή"</span><span class="sxs-lookup"><span data-stu-id="52825-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="52825-103">Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="52825-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="52825-104">Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης, για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet σε εφαρμογές της Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="52825-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="52825-105">Ανατρέξτε στο θέμα [Διευθύνσεις URL της Microsoft και περιοχές διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="52825-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="52825-106">Μεταβείτε **στην έναρξη**  >  **εκτέλεσης**και, στη συνέχεια, πληκτρολογήστε **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="52825-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="52825-107">Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:</span><span class="sxs-lookup"><span data-stu-id="52825-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="52825-108">Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου</span><span class="sxs-lookup"><span data-stu-id="52825-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="52825-109">Υπηρεσία λίστας δικτύου</span><span class="sxs-lookup"><span data-stu-id="52825-109">Network List Service</span></span>
    - <span data-ttu-id="52825-110">Ευαισθητοποίηση τοποθεσίας δικτύου</span><span class="sxs-lookup"><span data-stu-id="52825-110">Network Location Awareness</span></span>
    - <span data-ttu-id="52825-111">Αρχείο καταγραφής συμβάντων των Windows</span><span class="sxs-lookup"><span data-stu-id="52825-111">Windows Event Log</span></span>

<span data-ttu-id="52825-112">Εάν μία από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="52825-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="52825-113">Εάν αντιμετωπίσετε πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αυξημένα δικαιώματα:</span><span class="sxs-lookup"><span data-stu-id="52825-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="52825-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="52825-114">**sfc /scannow**</span></span>

<span data-ttu-id="52825-115">Μετά την ολοκλήρωση αυτής της εντολής, κάντε επανεκκίνηση του υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="52825-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="52825-116">Για λεπτομερείς πληροφορίες, [ανατρέξτε στην ενότητα "Λυπούμαστε, δεν μπορούμε να συνδεθούμε στο λογαριασμό σας. Προσπαθήστε ξανά αργότερα" σφάλμα κατά την ενεργοποίηση του Office από το Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="52825-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>