---
title: Πολλοί χρήστες δεν βλέπουν πρόσθετα στο Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197973"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="36e41-102">Πολλοί χρήστες δεν βλέπουν πρόσθετα στο Outlook</span><span class="sxs-lookup"><span data-stu-id="36e41-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="36e41-103">Εάν ελέγξετε τα πρόσθετα του Outlook και κανένα δεν εμφανίζεται, ως πρώτο βήμα αντιμετώπισης προβλημάτων, χρησιμοποιήστε το cmdlet **Get-OrganizationConfig** PowerShell για να υποβάλετε ερώτημα στην παράμετρο _AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="36e41-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="36e41-104">Εάν το ερώτημα επιστρέψει μια τιμή **False**, ορίστε αυτήν την παράμετρο σε **True** χρησιμοποιώντας το cmdlet **Set-OrganizationConfig,** επομένως τα πρόσθετα εμφανίζονται όπως αναμένεται.</span><span class="sxs-lookup"><span data-stu-id="36e41-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="36e41-105">Δεν συνιστάται η _παράμετρος AppsForOfficeEnabled_ να έχει οριστεί σε **False**.</span><span class="sxs-lookup"><span data-stu-id="36e41-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="36e41-106">Η τιμή **false** παρακάμπτει όλες τις παραπάνω ρυθμίσεις ρόλου διαχείρισης και χρήστη και εμποδίζει την ενεργοποίηση νέων εφαρμογών από οποιονδήποτε χρήστη στον οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="36e41-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="36e41-107">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Καθορισμός των διαχειριστών και των χρηστών που μπορούν να εγκαταστήσουν και να διαχειριστούν πρόσθετα για το Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="36e41-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>