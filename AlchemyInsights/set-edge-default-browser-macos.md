---
title: Ορισμός του Microsoft Edge ως προεπιλεγμένου προγράμματος περιήγησης σε συσκευή macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491553"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="e0762-102">Ορισμός του Microsoft Edge ως προεπιλεγμένου προγράμματος περιήγησης σε συσκευή macOS</span><span class="sxs-lookup"><span data-stu-id="e0762-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="e0762-103">Χρησιμοποιήστε μία από αυτές τις δύο μεθόδους για να ορίσετε τον Microsoft Edge ως το προεπιλεγμένο πρόγραμμα περιήγησης:</span><span class="sxs-lookup"><span data-stu-id="e0762-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="e0762-104">Μέθοδος 1: Αναβοσβήνουν τη συσκευή με μια εικόνα του macOS όπου ο Microsoft Edge έχει ήδη οριστεί ως το προεπιλεγμένο πρόγραμμα περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="e0762-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="e0762-105">Μέθοδος 2: Ορίστε την πολιτική DefaultBrowserSettingEnabled ώστε να ζητά από το χρήστη να ορίσει τον Microsoft Edge ως το προεπιλεγμένο πρόγραμμα περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="e0762-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="e0762-106">Οποιαδήποτε από τις δύο μεθόδους επιτρέπει σε ένα χρήστη να αλλάξει το προεπιλεγμένο πρόγραμμα περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="e0762-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="e0762-107">Για το λόγο αυτό, συνιστάται να αναπτύξετε την πολιτική DefaultBrowserSettingEnabled ακόμα και αν χρησιμοποιήσατε τη μέθοδο 1.</span><span class="sxs-lookup"><span data-stu-id="e0762-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="e0762-108">Εάν ένας χρήστης αλλάξει το προεπιλεγμένο πρόγραμμα περιήγησης μετά την ανάπτυξη της πολιτικής, η πολιτική ζητά από το χρήστη να ορίσει ξανά το προεπιλεγμένο πρόγραμμα περιήγησης στον Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="e0762-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
