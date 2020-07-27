---
title: Παράκαμψη κλειδώματος ενεργοποίησης σε εποπτευόμενες συσκευές iOS με το Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423734"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="bbacc-102">Παράκαμψη κλειδώματος ενεργοποίησης σε εποπτευόμενες συσκευές iOS με το Intune</span><span class="sxs-lookup"><span data-stu-id="bbacc-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="bbacc-103">Η δυνατότητα παράκαμψης του κλειδώματος ενεργοποίησης σε συσκευές iOS διευκολύνει την ανάκτηση από το σενάριο όπου ένας χρήστης επιτρέπει κλείδωμα ενεργοποίησης σε μια εταιρική συσκευή και, στη συνέχεια, εγκαταλείπει την εταιρεία.</span><span class="sxs-lookup"><span data-stu-id="bbacc-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="bbacc-104">Οι προϋποθέσεις για την παράκαμψη ενός κλειδώματος ενεργοποίησης περιλαμβάνουν:</span><span class="sxs-lookup"><span data-stu-id="bbacc-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="bbacc-105">Μια συσκευή είναι ότι είναι "εποπτεύεται".</span><span class="sxs-lookup"><span data-stu-id="bbacc-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="bbacc-106">Το κλείδωμα ενεργοποίησης ενεργοποιείται με επιτυχία χρησιμοποιώντας την πολιτική περιορισμού συσκευών iOS στο Intune.</span><span class="sxs-lookup"><span data-stu-id="bbacc-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="bbacc-107">Επιπλέον, όταν παρακάμπτετε ένα κλείδωμα ενεργοποίησης, θα πρέπει:</span><span class="sxs-lookup"><span data-stu-id="bbacc-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="bbacc-108">Φυσικά κατέχουν τη συσκευή που σκουπίζεται.</span><span class="sxs-lookup"><span data-stu-id="bbacc-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="bbacc-109">Αντιγράψτε τον κώδικα πριν να εκδώσετε το σβήσιμο.</span><span class="sxs-lookup"><span data-stu-id="bbacc-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="bbacc-110">**Σημείωση:** Ο κωδικός σβησίματος δεν κάνει διάκριση πεζών-κεφαλαίων, επομένως οι χαρακτήρες "-" δεν απαιτούνται.</span><span class="sxs-lookup"><span data-stu-id="bbacc-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="bbacc-111">Για λεπτομέρειες, ανατρέξτε στο θέμα [Παράκαμψη κλειδώματος ενεργοποίησης σε εποπτευόμενες συσκευές iOS με το Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="bbacc-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="bbacc-112">**ΣΥΝΗΘΕΙΣ ΕΡΩΤΉΣΕΙΣ**</span><span class="sxs-lookup"><span data-stu-id="bbacc-112">**FAQ**</span></span>

<span data-ttu-id="bbacc-113">Ε: **Εξέδωσα μια απομακρυσμένη ενέργεια για την κατάργηση εταιρικών δεδομένων από μια συσκευή και τώρα έχει κολλήσει σε κατάσταση εκκρεμότητας.**</span><span class="sxs-lookup"><span data-stu-id="bbacc-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="bbacc-114">Α: Για να ολοκληρωθεί με επιτυχία μια απομακρυσμένη ενέργεια, η στοχευμένη συσκευή πρέπει να είναι συνδεδεμένη και υγιής.</span><span class="sxs-lookup"><span data-stu-id="bbacc-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="bbacc-115">Στις ακόλουθες περιπτώσεις, η απομακρυσμένη ενέργεια παραμένει σε κατάσταση εκκρεμότητας για 30 ημέρες ή μέχρι η συσκευή να αναγνωρίσει την εντολή όταν η συσκευή:</span><span class="sxs-lookup"><span data-stu-id="bbacc-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="bbacc-116">Δεν έχει σύνδεση.</span><span class="sxs-lookup"><span data-stu-id="bbacc-116">Does not have connectivity.</span></span>
- <span data-ttu-id="bbacc-117">Χάνει το καθεστώς διαχείρισης με το Intune.</span><span class="sxs-lookup"><span data-stu-id="bbacc-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="bbacc-118">Αν πιστεύετε ότι μια συσκευή δεν κάνει πλέον μεταβίβαση ελέγχου και ότι δεν θα καταργήσει τα δεδομένα της εταιρείας, επιλέξτε Διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="bbacc-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="bbacc-119">Η διαγραφή καταργεί την εγγραφή συσκευής, ώστε να μην εμφανίζεται πλέον στη λίστα συσκευών Intune.</span><span class="sxs-lookup"><span data-stu-id="bbacc-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="bbacc-120">Για να ενεργοποιηθεί ξανά η συσκευή, ο χρήστης πρέπει να εγγράψει ξανά τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="bbacc-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="bbacc-121">Ε: **Γιατί ορισμένες απομακρυσμένες ενέργειες δεν είναι διαθέσιμες για χρήση;**</span><span class="sxs-lookup"><span data-stu-id="bbacc-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="bbacc-122">Α: Δεν υποστηρίζουν όλες οι πλατφόρμες όλες τις ενέργειες απομακρυσμένης συσκευής.</span><span class="sxs-lookup"><span data-stu-id="bbacc-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="bbacc-123">Οι ακόλουθες απομακρυσμένες ενέργειες αφορούν συγκεκριμένη πλατφόρμα.</span><span class="sxs-lookup"><span data-stu-id="bbacc-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="bbacc-124">Παράκαμψη κλειδώματος ενεργοποίησης (μόνο για iOS)</span><span class="sxs-lookup"><span data-stu-id="bbacc-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="bbacc-125">Νέα αρχή (μόνο για Windows)</span><span class="sxs-lookup"><span data-stu-id="bbacc-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="bbacc-126">Κατάσταση απώλειας (μόνο για iOS)</span><span class="sxs-lookup"><span data-stu-id="bbacc-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="bbacc-127">Εντοπισμός συσκευής (μόνο για iOS)</span><span class="sxs-lookup"><span data-stu-id="bbacc-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="bbacc-128">Επανεκκίνηση (μόνο για Windows)</span><span class="sxs-lookup"><span data-stu-id="bbacc-128">Restart (Windows only)</span></span>

<span data-ttu-id="bbacc-129">Για περισσότερες λεπτομέρειες σχετικά με κάθε ενέργεια, ανατρέξτε στο θέμα [Διαθέσιμες ενέργειες συσκευής](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="bbacc-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>