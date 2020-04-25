---
title: Διπλότυπη εγγραφή συσκευής στην πύλη
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789862"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="3924b-102">Διπλότυπη εγγραφή συσκευής στην πύλη</span><span class="sxs-lookup"><span data-stu-id="3924b-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="3924b-103">Ενδέχεται να δείτε 2 εγγραφές για μια συσκευή στην πύλη, εάν η συσκευή δεν αναφέρει σωστά την κατάσταση από κοινού διαχείρισης στην τοποθεσία Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="3924b-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="3924b-104">Για να ελέγξετε την κατάσταση από κοινού διαχείρισης μιας συσκευής, ελέγξτε τη στήλη **Από κοινού διαχείριση** για τη συσκευή στην κονσόλα Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="3924b-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="3924b-105">Εάν η στήλη δεν είναι ορατή, μπορείτε να την προσθέσετε κάνοντας δεξί κλικ σε οποιαδήποτε κεφαλίδα στήλης και επιλέγοντάς την από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="3924b-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="3924b-106">Η τιμή "από κοινού διαχείριση" πρέπει να είναι **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="3924b-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="3924b-107">Αν η τιμή είναι **Όχι**, ανοίξτε τη βοηθητική εφαρμογή του προγράμματος-πελάτη του Configuration Manager στη συσκευή του προγράμματος-πελάτη και ελέγξτε την ιδιότητα **Από κοινού διαχείριση** στην καρτέλα Γενικά.</span><span class="sxs-lookup"><span data-stu-id="3924b-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="3924b-108">Αν η τιμή είναι **Ενεργοποιήθηκε**, αυτό υποδεικνύει προβλήματα στην επικοινωνία του προγράμματος-πελάτη με το σημείο διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="3924b-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="3924b-109">Ελέγξτε το **CcmMessaging.log** στη συσκευή για να διερευνήσετε πιθανά προβλήματα συνδεσιμότητας.</span><span class="sxs-lookup"><span data-stu-id="3924b-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="3924b-110">Αν η τιμή είναι **Απενεργοποιήθηκε** και η συσκευή έχει εγγραφεί στο Intune, βεβαιωθείτε ότι η συσκευή έχει λάβει την πολιτική από κοινού διαχείρισης, ελέγχοντας το **CoManagementHandler.log** στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="3924b-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
