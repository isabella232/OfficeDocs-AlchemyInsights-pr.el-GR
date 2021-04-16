---
title: Το OneDrive για επιχειρήσεις Web OneDrive ανακατευθύνει στο Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799989"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="2c343-102">Ανακατεύθυνση στο Delve αφού κάνετε κλικ στο OneDrive</span><span class="sxs-lookup"><span data-stu-id="2c343-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="2c343-103">Ανατρέξτε στον αναλυτικό [οδηγό αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="2c343-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="2c343-104">Για να επιλύσετε αυτό το πρόβλημα, ο διαχειριστής πρέπει να εκχωρήσει στους χρήστες το δικαίωμα να δημιουργήσουν την τοποθεσία "Οι τοποθεσίες μου".</span><span class="sxs-lookup"><span data-stu-id="2c343-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="2c343-105">Αυτό συμβαίνει επειδή η σελίδα του OneDrive για επιχειρήσεις δημιουργείται στις "Οι τοποθεσίες μου".</span><span class="sxs-lookup"><span data-stu-id="2c343-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="2c343-106">Για να εκχωρήσετε αυτό το δικαίωμα, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="2c343-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="2c343-107">Στο κέντρο διαχείρισης του SharePoint, κάντε κλικ **στα προφίλ χρηστών.**</span><span class="sxs-lookup"><span data-stu-id="2c343-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="2c343-108">Στην ενότητα **"Άτομα",** κάντε κλικ **στην επιλογή "Διαχείριση δικαιωμάτων χρήστη".**</span><span class="sxs-lookup"><span data-stu-id="2c343-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="2c343-109">Προσθέστε χρήστες που απαιτούν δικαιώματα για να δημιουργήσουν την τοποθεσία "Οι τοποθεσίες μου".</span><span class="sxs-lookup"><span data-stu-id="2c343-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="2c343-110">Από προεπιλογή, αυτή η ρύθμιση έχει οριστεί σε **"Όλοι", εκτός από εξωτερικούς χρήστες.**</span><span class="sxs-lookup"><span data-stu-id="2c343-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="2c343-111">Αφού έχετε προσθέσει το χρήστη, τους χρήστες ή την ομάδα, βεβαιωθείτε ότι είναι επιλεγμένος ο χρήστης, οι χρήστες ή η ομάδα που προστέθηκε, κάντε κύλιση στην ενότητα δικαιωμάτων και, στη συνέχεια, επιλέξτε το πλαίσιο ελέγχου δίπλα στην επιλογή "Δημιουργία προσωπικής τοποθεσίας" (απαιτείται για προσωπικό χώρο αποθήκευσης, τροφοδοσία ειδήσεων και περιεχόμενο **που παρακολουθείται)**. </span><span class="sxs-lookup"><span data-stu-id="2c343-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="2c343-112">Κάντε **κλικ στο κουμπί OK** και, στη συνέχεια, κατόπιν, κάντε αναζήτηση στη σελίδα του OneDrive για να δημιουργήσετε την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="2c343-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
