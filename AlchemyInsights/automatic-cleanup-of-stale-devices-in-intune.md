---
title: Αυτόματος καθαρισμός παλιών συσκευών στο Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554967"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="81474-102">Αυτόματος καθαρισμός παλιών συσκευών στο Intune</span><span class="sxs-lookup"><span data-stu-id="81474-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="81474-103">Το Intune επιτρέπει στο διαχειριστή να ρυθμίσει ένα χρονικό διάστημα μεταξύ 90 και 270 ημερών, μετά την οποία οι παλιές συσκευές καταργούνται από την υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="81474-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="81474-104">Αυτή η ρύθμιση είναι ευρεία σε επίπεδο οργάνωσης και μόλις ενεργοποιηθεί τίθεται σε ισχύ αμέσως.</span><span class="sxs-lookup"><span data-stu-id="81474-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="81474-105">Οι συσκευές που δεν έχουν γίνει έλεγχο στο διακομιστή Intune για περίοδο που υπερβαίνει τη ρύθμιση διαγράφονται οριστικά.</span><span class="sxs-lookup"><span data-stu-id="81474-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="81474-106">**Σημείωση** Μόνο τα αντικείμενα συσκευής MDM είναι κατάλληλα για αυτήν την ενέργεια εκκαθάρισης.</span><span class="sxs-lookup"><span data-stu-id="81474-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="81474-107">Εξαιρούνται μόνο αντικείμενα συσκευών EAS.</span><span class="sxs-lookup"><span data-stu-id="81474-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="81474-108">Για πρόσθετες πληροφορίες σχετικά με το πότε μια συσκευή καθίσταται επιλέξιμη για διαγραφή με βάση τη ρύθμιση εκκαθάρισης της συσκευής και την "κατάστασή" της:</span><span class="sxs-lookup"><span data-stu-id="81474-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="81474-109">Ρύθμιση: **Διαγραφή συσκευών μετά την τελευταία ημερομηνία μεταβίβασης ελέγχου: Ναι (κάποια τιμή (N) σε καθορισμένες ημέρες)**</span><span class="sxs-lookup"><span data-stu-id="81474-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="81474-110">Με βάση την τιμή (N) που έχει ρυθμιστεί στη ρύθμιση, η υπηρεσία Intune διαγράφει τη συσκευή τις καθορισμένες ημέρες μετά την τελευταία επιτυχημένη check-in.</span><span class="sxs-lookup"><span data-stu-id="81474-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="81474-111">Ρύθμιση: **Διαγραφή συσκευών μετά την τελευταία ημερομηνία μεταβίβασης ελέγχου: Όχι**</span><span class="sxs-lookup"><span data-stu-id="81474-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="81474-112">180 ημέρες μετά τη λήξη του πιστοποιητικού συσκευής και δεν ανανεώνεται, η συσκευή διαγράφεται.</span><span class="sxs-lookup"><span data-stu-id="81474-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="81474-113">**Σημείωση** Και στις δύο περιπτώσεις, η συσκευή πρέπει να καταχωρηθεί με επιτυχία στο Intune.</span><span class="sxs-lookup"><span data-stu-id="81474-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="81474-114">Η εγγραφή πραγματοποιείται κατά τον πρώτο έλεγχο της συσκευής με την υπηρεσία Intune.</span><span class="sxs-lookup"><span data-stu-id="81474-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="81474-115">Εάν μια συσκευή εγγραφεί με επιτυχία στο Intune αλλά δεν καταχωρηθεί στο Intune, η συσκευή διαγράφεται 270 ημέρες μετά την εγγραφή.</span><span class="sxs-lookup"><span data-stu-id="81474-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="81474-116">(90 ημέρες για να επισημάνετε τη συσκευή ως ανακλημένη και, στη συνέχεια, άλλες 180 ημέρες για να διαγράψετε την εγγραφή.)</span><span class="sxs-lookup"><span data-stu-id="81474-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="81474-117">Προς το παρόν δεν υπάρχει μηχανισμός στην κονσόλα Intune για τον καθορισμό της ημερομηνίας λήξης της πιστοποίησης συσκευής για οποιαδήποτε δεδομένη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="81474-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>