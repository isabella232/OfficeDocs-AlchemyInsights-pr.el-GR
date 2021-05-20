---
title: Προβλήματα με την κατάργηση μιας συσκευής εκτός πίνακα ή μιας συσκευής που έχει απενεργοποιηθεί από το Απόθεμα συσκευών
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564172"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="f091c-102">Προβλήματα με την κατάργηση μιας συσκευής εκτός πίνακα ή μιας συσκευής που έχει απενεργοποιηθεί από το Απόθεμα συσκευών</span><span class="sxs-lookup"><span data-stu-id="f091c-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="f091c-103">Προς το παρόν, ο Microsoft Defender για τελικό σημείο δεν επιτρέπει τη μη αυτόματη κατάργηση της εγγραφής συσκευής μιας συσκευής εκτός πίνακα ή μιας συσκευής που έχει απενεργοποιηθεί από το απόθεμα συσκευών.</span><span class="sxs-lookup"><span data-stu-id="f091c-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="f091c-104">Για λόγους ασφαλείας, η συσκευή παραμένει στην πύλη ως ιστορικό αρχείο για έως και 180 ημέρες.</span><span class="sxs-lookup"><span data-stu-id="f091c-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="f091c-105">Ωστόσο, τα δεδομένα της συσκευής εκκαθαρίστηκε σύμφωνα με τη ρυθμισμένη περίοδο διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="f091c-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="f091c-106">**Σημείωση:** Μια συσκευή χωρίς πίνακα ή συσκευή εκτός λειτουργίας μεταβαίνει αυτόματα σε **κατάσταση αδράνειας** μετά από επτά ημέρες.</span><span class="sxs-lookup"><span data-stu-id="f091c-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="f091c-107">Επιπλέον, οι συσκευές που δεν είναι ενεργές τις τελευταίες 30 ημέρες δεν λαμβάνονται υπόψη στα δεδομένα που απεικονίζουν τη βαθμολογία Διαχείριση απειλών και ευπαθειών έκθεσης του οργανισμού σας ή τη Βαθμολογία ασφαλείας της Microsoft για συσκευές.</span><span class="sxs-lookup"><span data-stu-id="f091c-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="f091c-108">Εάν εξακολουθείτε να μην θέλετε να βλέπετε συγκεκριμένες συσκευές στην προβολή "Απόθεμα συσκευών", δοκιμάστε να τοποθετήσετε μια ετικέτα συσκευής για να φιλτράρετε τη συσκευή που έχει τεθεί εκτός λειτουργίας από την προβολή "Απόθεμα συσκευών".</span><span class="sxs-lookup"><span data-stu-id="f091c-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="f091c-109">Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="f091c-109">For more information, see:</span></span>

[<span data-ttu-id="f091c-110">Συσκευές offboard από την υπηρεσία Microsoft Defender για τελικά σημεία</span><span class="sxs-lookup"><span data-stu-id="f091c-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="f091c-111">Βαθμολογία έκθεσης σε Διαχείριση απειλών και ευπαθειών</span><span class="sxs-lookup"><span data-stu-id="f091c-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="f091c-112">Επιδιόρθωση ανθυγιεινών αισθητήρων στο Microsoft Defender για το τελικό σημείο</span><span class="sxs-lookup"><span data-stu-id="f091c-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="f091c-113">Τρόπος αποτελεσματικής χρήσης της προσθήκης ετικετών (Μέρος 1)</span><span class="sxs-lookup"><span data-stu-id="f091c-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="f091c-114">Τρόπος αποτελεσματικής χρήσης της προσθήκης ετικετών (Μέρος 2)</span><span class="sxs-lookup"><span data-stu-id="f091c-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="f091c-115">Τρόπος αποτελεσματικής χρήσης της προσθήκης ετικετών (Μέρος 3)</span><span class="sxs-lookup"><span data-stu-id="f091c-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




