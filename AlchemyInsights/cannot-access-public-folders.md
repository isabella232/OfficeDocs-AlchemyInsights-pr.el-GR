---
title: Δεν είναι δυνατή η πρόσβαση σε δημόσιους φακέλους
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959495"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="4eeb3-102">Δεν είναι δυνατή η σύνδεση του Outlook με δημόσιους φακέλους</span><span class="sxs-lookup"><span data-stu-id="4eeb3-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="4eeb3-103">Εάν η πρόσβαση σε δημόσιους φακέλους δεν λειτουργεί για λίγους χρήστες, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="4eeb3-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="4eeb3-104">Σύνδεση με εξω PowerShell και ρυθμίστε τις παραμέτρους του γραμματοκιβωτίου Προεπιλεγήςφάκελος στο λογαριασμό χρήστη του προβλήματος για να ταιριάζει με μία σε ένα λογαριασμό χρήστη που λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="4eeb3-105">Παράδειγμα:</span><span class="sxs-lookup"><span data-stu-id="4eeb3-105">Example:</span></span>

<span data-ttu-id="4eeb3-106">Λήψη-γραμματοκιβώτιο WorkingUser | Γραμματοκιβωτίου EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="4eeb3-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="4eeb3-107">Set-γραμματοκιβώτιο Πρόβλήσενος χρήστη προεπιλεγμένη τιμή γραμματοκιβωτίου \<από την προηγούμενη εντολή></span><span class="sxs-lookup"><span data-stu-id="4eeb3-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="4eeb3-108">Περιμένετε τουλάχιστον μία ώρα για να τεθεί σε ισχύ η αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-108">Wait at least one hour for the change to take effect.</span></span>