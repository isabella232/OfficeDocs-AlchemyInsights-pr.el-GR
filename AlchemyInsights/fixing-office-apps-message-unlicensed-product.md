---
title: Δεν είναι δυνατή η ενεργοποίηση του Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798680"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="fe70a-102">Δεν είναι δυνατή η ενεργοποίηση του Office</span><span class="sxs-lookup"><span data-stu-id="fe70a-102">Unable to activate Office</span></span>

<span data-ttu-id="fe70a-103">**Σημείωση:** Εάν χρησιμοποιείτε μια παλαιότερη έκδοση του Windows (Για παράδειγμα, Windows 7), βεβαιωθείτε ότι το TLS 1.2 είναι ενεργοποιημένο ως προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="fe70a-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="fe70a-104">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Ενημέρωση για την ενεργοποίηση [των TLS 1.1 και TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP στο Windows.</span><span class="sxs-lookup"><span data-stu-id="fe70a-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="fe70a-105">Ελέγξτε εάν έχει λήξει η κατάσταση της συνδρομής σας.</span><span class="sxs-lookup"><span data-stu-id="fe70a-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="fe70a-106">Βεβαιωθείτε ότι έχετε μια συνδρομή που επιτρέπει άδειες χρήσης προγράμματος-πελάτη, όπως το Office 365 για Επιχειρήσεις ή το Office 365 Premium για Επιχειρήσεις και [βεβαιωθείτε ότι έχει εκχωρηθεί άδεια στον χρήστη](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="fe70a-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="fe70a-107">Βεβαιωθείτε ότι ο χρήστης πραγματοποιεί είσοδο στο Office με τον ίδιο λογαριασμό στον οποίο έχει εκχωρηθεί η άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="fe70a-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="fe70a-108">Επισκεφθείτε τη [σελίδα εύρυθμης λειτουργίας των υπηρεσιών του Office 365](/office365/enterprise/view-service-health) για να δείτε αν υπάρχουν γνωστά προβλήματα με την υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="fe70a-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="fe70a-109">Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet στις εφαρμογές του Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fe70a-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="fe70a-110">Ανατρέξτε στο θέμα [Διευθύνσεις URL και εύρη διευθύνσεων IP του Office 365](/office365/enterprise/urls-and-ip-address-ranges "Διευθύνσεις URL και εύρη διευθύνσεων IP του Office 365").</span><span class="sxs-lookup"><span data-stu-id="fe70a-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="fe70a-111">**Συμβουλή** Σε υπολογιστές με Windows, μπορούμε να διαγνώσουμε και να διορθώσουμε αυτόματα αρκετά κοινά προβλήματα εισόδου του Office για εσάς.</span><span class="sxs-lookup"><span data-stu-id="fe70a-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="fe70a-112">Κατεβάστε και εκτελέστε τον **[Βοηθό υποστήριξης και αποκατάστασης για το Office 365](https://aka.ms/SaRA-OfficeSignInScenario)** για να χρησιμοποιήσετε το αυτοματοποιημένο εργαλείο μας.</span><span class="sxs-lookup"><span data-stu-id="fe70a-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="fe70a-113">Χρησιμοποιήστε τις παρακάτω ενέργειες αντιμετώπισης προβλημάτων:</span><span class="sxs-lookup"><span data-stu-id="fe70a-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="fe70a-114">Ανοίξτε μια εφαρμογή του Office και [Αποσυνδεθείτε](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) από όλους τους υπάρχοντες λογαριασμούς χρηστών.</span><span class="sxs-lookup"><span data-stu-id="fe70a-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="fe70a-115">[Κατάργηση](/microsoft-365/admin/manage/remove-licenses-from-users) και [εκ νέου ανάθεση](/microsoft-365/admin/manage/assign-licenses-to-users)της άδεια χρήσης του Office και, στη συνέχεια, [συνδεθείτε στο Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) χρησιμοποιώντας το λογαριασμό χρήστη που επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="fe70a-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="fe70a-116">Εκτέλεση του προγράμματος [Αντιμετώπιση προβλημάτων ενεργοποίησης](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="fe70a-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="fe70a-117">Επαναφορά κατάστασης ενεργοποίησης του Office</span><span class="sxs-lookup"><span data-stu-id="fe70a-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Επαναφορά κατάστασης ενεργοποίησης του Office")
- [<span data-ttu-id="fe70a-118">Πραγματοποίηση επιδιόρθωσης του Office μέσω Internet</span><span class="sxs-lookup"><span data-stu-id="fe70a-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="fe70a-119">Για πρόσθετες λύσεις αντιμετώπισης προβλημάτων, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="fe70a-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="fe70a-120">Σφάλματα "Προϊόν χωρίς άδεια χρήσης" και σφάλματα ενεργοποίησης στο Office</span><span class="sxs-lookup"><span data-stu-id="fe70a-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="fe70a-121">"Λυπούμαστε, δεν είναι δυνατή η σύνδεση στο λογαριασμό σας. Σφάλμα "Δοκιμάστε ξανά αργότερα" κατά την ενεργοποίηση του Office</span><span class="sxs-lookup"><span data-stu-id="fe70a-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)