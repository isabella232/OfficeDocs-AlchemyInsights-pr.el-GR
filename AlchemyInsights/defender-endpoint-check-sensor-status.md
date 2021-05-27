---
title: Κατάσταση αισθητήρα ελέγχου τελικού σημείου defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676180"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="9ab1f-102">Κατάσταση αισθητήρα ελέγχου τελικού σημείου defender</span><span class="sxs-lookup"><span data-stu-id="9ab1f-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="9ab1f-103">Το **πλακίδιο "Συσκευές με προβλήματα αισθητήρα"** βρίσκεται στον πίνακα εργαλείων "Λειτουργίες ασφαλείας".</span><span class="sxs-lookup"><span data-stu-id="9ab1f-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="9ab1f-104">Αυτό το πλακίδιο παρέχει πληροφορίες σχετικά με τη δυνατότητα της μεμονωμένης συσκευής να παρέχει δεδομένα αισθητήρα και να επικοινωνεί με τον Defender για την υπηρεσία endpoint.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="9ab1f-105">Αναφέρει πόσες συσκευές απαιτούν προσοχή και σας βοηθά να εντοπίσετε προβληματικές συσκευές και να κάνετε ενέργειες για να διορθώσετε γνωστά προβλήματα.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="9ab1f-106">Δύο ενδείξεις κατάστασης στο πλακίδιο παρέχουν πληροφορίες σχετικά με τον αριθμό των συσκευών που δεν αναφέρουν σωστά στην υπηρεσία:</span><span class="sxs-lookup"><span data-stu-id="9ab1f-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="9ab1f-107">**Εσφαλμένες ρυθμίσεις παραμέτρων** Συσκευές που ενδέχεται να αναφέρουν μερικώς δεδομένα αισθητήρα στην υπηρεσία Defender για τελικά σημεία και ενδέχεται να έχουν σφάλματα ρύθμισης παραμέτρων που πρέπει να διορθωθούν.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="9ab1f-108">**Ανενεργός** Συσκευές που έχουν σταματήσει να αναφέρουν στον Defender για την υπηρεσία τελικού σημείου για περισσότερες από επτά ημέρες τον προηγούμενο μήνα.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="9ab1f-109">Κάνοντας κλικ σε οποιαδήποτε από τις ομάδες κατευθύνετε τη λίστα "Συσκευές", φιλτραρισμένο σύμφωνα με τις επιλογές σας.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="9ab1f-110">Στη λίστα "Συσκευές", μπορείτε να φιλτράρετε τη λίστα κατάστασης λειτουργίας με την ακόλουθη κατάσταση:</span><span class="sxs-lookup"><span data-stu-id="9ab1f-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="9ab1f-111">**Ενεργό** Συσκευές που αναφέρουν ενεργά στον Defender για την υπηρεσία τελικού σημείου.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="9ab1f-112">**Εσφαλμένες ρυθμίσεις παραμέτρων** Συσκευές που μπορεί να αναφέρουν μερικώς δεδομένα αισθητήρα στην υπηρεσία Defender για τελικά σημεία, αλλά έχουν σφάλματα ρύθμισης παραμέτρων που πρέπει να διορθωθούν.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="9ab1f-113">Οι συσκευές που έχουν εσφαλμένες παραμέτρους μπορεί να έχουν ένα ή ένα συνδυασμό από τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="9ab1f-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="9ab1f-114">Δεν υπάρχουν δεδομένα αισθητήρα - Οι συσκευές έχουν σταματήσει να στέλνουν δεδομένα αισθητήρα.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="9ab1f-115">Περιορισμένες ειδοποιήσεις μπορούν να ενεργοποιούνται από τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="9ab1f-116">Μειωμένη επικοινωνία - Η δυνατότητα επικοινωνίας με τη συσκευή είναι μειωμένη.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="9ab1f-117">Η αποστολή αρχείων για λεπτομερή ανάλυση, αποκλεισμό αρχείων, απομόνωση συσκευής από το δίκτυο και άλλες ενέργειες που απαιτούν επικοινωνία με τη συσκευή ενδέχεται να μην λειτουργούν.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="9ab1f-118">**Ανενεργός** Συσκευές που έχουν σταματήσει να αναφέρουν στον Defender για την υπηρεσία τελικού σημείου.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="9ab1f-119">Μπορείτε να κάνετε λήψη ολόκληρης της λίστας σε μορφή CSV χρησιμοποιώντας τη δυνατότητα "Εξαγωγή".</span><span class="sxs-lookup"><span data-stu-id="9ab1f-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="9ab1f-120">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Έλεγχος κατάστασης της υγείας των αισθητήρων στο Microsoft Defender για το τελικό σημείο.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="9ab1f-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="9ab1f-121">Για περισσότερες πληροφορίες σχετικά με το τι προκάλεσε την αδράνεια ή την εσφαλμένη ρύθμιση παραμέτρων μιας συσκευής, ανατρέξτε στο θέμα Επιδιόρθωση ανθυγιεινών αισθητήρων [στο Microsoft Defender για το Τελικό σημείο.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="9ab1f-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
