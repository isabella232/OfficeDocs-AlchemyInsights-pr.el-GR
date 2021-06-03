---
title: Δημιουργία και διαχείριση ετικετών ή ομάδων συσκευών
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731664"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="34962-102">Δημιουργία και διαχείριση ετικετών ή ομάδων συσκευών</span><span class="sxs-lookup"><span data-stu-id="34962-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="34962-103">Προσθέστε ετικέτες σε συσκευές για να δημιουργήσετε μια λογική ομαδοποίηση.</span><span class="sxs-lookup"><span data-stu-id="34962-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="34962-104">Οι ετικέτες συσκευών υποστηρίζουν τη σωστή αντιστοίχιση του δικτύου, επιτρέποντάς σας να επισυνάψετε διαφορετικές ετικέτες για την καταγραφή του περιβάλλοντος και να ενεργοποιήσετε τη δημιουργία δυναμικής λίστας ως μέρος ενός συμβάντος.</span><span class="sxs-lookup"><span data-stu-id="34962-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="34962-105">Οι ετικέτες μπορούν να χρησιμοποιηθούν ως φίλτρο στην προβολή λίστας συσκευών ή για την ομαδοποίηση συσκευών.</span><span class="sxs-lookup"><span data-stu-id="34962-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="34962-106">Για περισσότερες πληροφορίες σχετικά με την ομαδοποίηση συσκευών, ανατρέξτε στο θέμα [Δημιουργία και διαχείριση ετικετών συσκευής.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="34962-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="34962-107">Μπορείτε να προσθέσετε ετικέτες σε συσκευές:</span><span class="sxs-lookup"><span data-stu-id="34962-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="34962-108">Χρήση της πύλης</span><span class="sxs-lookup"><span data-stu-id="34962-108">Using the portal</span></span>

- <span data-ttu-id="34962-109">Ορισμός τιμής κλειδιού μητρώου</span><span class="sxs-lookup"><span data-stu-id="34962-109">Setting a registry key value</span></span>
 
<span data-ttu-id="34962-110">**Σημείωση:** Ενδέχεται να υπάρχει λανθάνων χρόνος μεταξύ του χρόνου προσθήκης μιας ετικέτας σε μια συσκευή και της διαθεσιμότητάς της στη λίστα συσκευών και στη σελίδα της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="34962-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="34962-111">Για να προσθέσετε ετικέτες συσκευών χρησιμοποιώντας το API, ανατρέξτε στο [θέμα "Προσθήκη ή κατάργηση ετικετών συσκευής API".](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="34962-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="34962-112">Προσθήκη και διαχείριση ετικετών συσκευής με χρήση της πύλης</span><span class="sxs-lookup"><span data-stu-id="34962-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="34962-113">Επιλέξτε τη συσκευή στην οποία θέλετε να διαχειριστείτε ετικέτες.</span><span class="sxs-lookup"><span data-stu-id="34962-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="34962-114">Μπορείτε να επιλέξετε ή να αναζητήσετε μια συσκευή από οποιαδήποτε από τις παρακάτω προβολές:</span><span class="sxs-lookup"><span data-stu-id="34962-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="34962-115">**Πίνακας εργαλείων λειτουργιών ασφαλείας** Επιλέξτε το όνομα της συσκευής από την ενότητα "Κορυφαίες συσκευές με ενεργές ειδοποιήσεις".</span><span class="sxs-lookup"><span data-stu-id="34962-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="34962-116">**Ουρά ειδοποιήσεων** - Επιλέξτε το όνομα της συσκευής δίπλα στο εικονίδιο της συσκευής από την ουρά ειδοποιήσεων.</span><span class="sxs-lookup"><span data-stu-id="34962-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="34962-117">**Λίστα συσκευών** - Επιλέξτε το όνομα της συσκευής από τη λίστα των συσκευών.</span><span class="sxs-lookup"><span data-stu-id="34962-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="34962-118">**Πλαίσιο αναζήτησης** - Επιλέξτε "Συσκευή" από το αναπτυσσόμενο μενού και πληκτρολογήστε το όνομα της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="34962-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="34962-119">Μπορείτε επίσης να λάβετε τη σελίδα ειδοποίησης μέσω των προβολών αρχείου και IP.</span><span class="sxs-lookup"><span data-stu-id="34962-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="34962-120">Επιλέξτε **"Διαχείριση ετικετών"** από τη γραμμή ενεργειών απόκρισης.</span><span class="sxs-lookup"><span data-stu-id="34962-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="34962-121">Πληκτρολογήστε για να βρείτε ή να δημιουργήσετε ετικέτες.</span><span class="sxs-lookup"><span data-stu-id="34962-121">Type to find or create tags.</span></span>

<span data-ttu-id="34962-122">Οι ετικέτες προστίθενται στην προβολή συσκευής και αντικατοπτρίζονται στην προβολή λίστας συσκευών.</span><span class="sxs-lookup"><span data-stu-id="34962-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="34962-123">Στη συνέχεια, μπορείτε να χρησιμοποιήσετε το φίλτρο "Ετικέτες" για να δείτε τη σχετική λίστα συσκευών.</span><span class="sxs-lookup"><span data-stu-id="34962-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="34962-124">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δημιουργία και διαχείριση ετικετών συσκευής.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="34962-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>