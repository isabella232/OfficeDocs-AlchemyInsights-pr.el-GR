---
title: Ο καθορισμός εφαρμογών του Microsoft 365 δεν μπόρεσε να εντοπίσει το συσχετισμένο μήνυμα των αδειών χρήσης
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747695"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="3252b-102">Επιδιόρθωση των εφαρμογών του Microsoft 365 "δεν ήταν δυνατή η εύρεση των σχετικών αδειών χρήσης του Office"</span><span class="sxs-lookup"><span data-stu-id="3252b-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="3252b-103">Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="3252b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="3252b-104">Επιλέξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις του διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet στις εφαρμογές Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3252b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="3252b-105">Ανατρέξτε στο θέμα [διευθύνσεις URL και περιοχές διευθύνσεων IP του Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="3252b-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="3252b-106">Κατάργηση και [εκ νέου εκχώρηση της άδειας χρήσης του Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) για τον επηρεαζόμενο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="3252b-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="3252b-107">Ανοίξτε μια εφαρμογή του Office και [αποσυνδεθείτε](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) από οποιουσδήποτε υπάρχοντες λογαριασμούς χρηστών.</span><span class="sxs-lookup"><span data-stu-id="3252b-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="3252b-108">Μεταβείτε στις ρυθμίσεις των Windows **> λογαριασμούς**  >  **ηλεκτρονικού ταχυδρομείου &** λογαριασμούς και καταργήστε όλους τους λογαριασμούς εργασίας εκτός από τον επηρεαζόμενο λογαριασμό.</span><span class="sxs-lookup"><span data-stu-id="3252b-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="3252b-109">Μεταβείτε στις ρυθμίσεις των Windows **Accounts**>  >  την**εργασία ή το σχολείο της Access**για λογαριασμούς και αποσυνδέστε όλους τους λογαριασμούς εργασίας εκτός από τον επηρεαζόμενο λογαριασμό.</span><span class="sxs-lookup"><span data-stu-id="3252b-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="3252b-110">Επαναφέρετε την κατάσταση ενεργοποίησης του Office.</span><span class="sxs-lookup"><span data-stu-id="3252b-110">Reset the Office activation state.</span></span> <span data-ttu-id="3252b-111">[Μάθετε πώς](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="3252b-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="3252b-112">[Πραγματοποιήστε είσοδο](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) χρησιμοποιώντας το λογαριασμό χρήστη που επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="3252b-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="3252b-113">Για πρόσθετες λύσεις αντιμετώπισης προβλημάτων, ανατρέξτε [στο θέμα σφάλματα προϊόντος και ενεργοποίησης χωρίς άδεια χρήσης στο Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="3252b-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>