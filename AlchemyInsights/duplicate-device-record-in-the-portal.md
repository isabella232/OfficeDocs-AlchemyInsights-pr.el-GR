---
title: Διπλότυπη εγγραφή συσκευής στην πύλη
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
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814516"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="c5060-102">Διπλότυπη εγγραφή συσκευής στην πύλη</span><span class="sxs-lookup"><span data-stu-id="c5060-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="c5060-103">Ενδέχεται να δείτε 2 εγγραφές για μια συσκευή στην πύλη, εάν η συσκευή δεν αναφέρει σωστά την κατάσταση από κοινού διαχείρισης στην τοποθεσία Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="c5060-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="c5060-104">Για να ελέγξετε την κατάσταση από κοινού διαχείρισης μιας συσκευής, ελέγξτε τη στήλη **Από κοινού διαχείριση** για τη συσκευή στην κονσόλα Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="c5060-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="c5060-105">Εάν η στήλη δεν είναι ορατή, μπορείτε να την προσθέσετε κάνοντας δεξί κλικ σε οποιαδήποτε κεφαλίδα στήλης και επιλέγοντάς την από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="c5060-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="c5060-106">Η τιμή "από κοινού διαχείριση" πρέπει να είναι **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="c5060-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="c5060-107">Αν η τιμή είναι **Όχι**, ανοίξτε τη βοηθητική εφαρμογή του προγράμματος-πελάτη του Configuration Manager στη συσκευή του προγράμματος-πελάτη και ελέγξτε την ιδιότητα **Από κοινού διαχείριση** στην καρτέλα Γενικά.</span><span class="sxs-lookup"><span data-stu-id="c5060-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="c5060-108">Αν η τιμή είναι **Ενεργοποιήθηκε**, αυτό υποδεικνύει προβλήματα στην επικοινωνία του προγράμματος-πελάτη με το σημείο διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="c5060-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="c5060-109">Ελέγξτε το **CcmMessaging.log** στη συσκευή για να διερευνήσετε πιθανά προβλήματα συνδεσιμότητας.</span><span class="sxs-lookup"><span data-stu-id="c5060-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="c5060-110">Αν η τιμή είναι **Απενεργοποιήθηκε** και η συσκευή έχει εγγραφεί στο Intune, βεβαιωθείτε ότι η συσκευή έχει λάβει την πολιτική από κοινού διαχείρισης, ελέγχοντας το **CoManagementHandler.log** στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="c5060-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
