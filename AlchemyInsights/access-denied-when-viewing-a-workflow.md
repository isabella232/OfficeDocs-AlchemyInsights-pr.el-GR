---
title: Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747748"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="0a04c-102">Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας</span><span class="sxs-lookup"><span data-stu-id="0a04c-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="0a04c-103">Ροές εργασίας του SharePoint 2013 που επιχειρούν να στείλουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint μπορεί να αποτύχει με ένα μήνυμα λάθους "δεν επιτρέπεται η πρόσβαση" Εάν η ιδιότητα μέλους της ομάδας του SharePoint δεν έχει οριστεί σε όλους.</span><span class="sxs-lookup"><span data-stu-id="0a04c-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="0a04c-104">**Για να επιλύσετε αυτό το ζήτημα, κάντε τα εξής βήματα:**</span><span class="sxs-lookup"><span data-stu-id="0a04c-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="0a04c-105">Να επιτρέπεται σε όλους να βλέπουν τα μέλη της ομάδας του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0a04c-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="0a04c-106">Καταργήστε την ομάδα του SharePoint από τη γραμμή προς ή CC του μηνύματος ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="0a04c-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="0a04c-107">Προσθέστε ρητά τους χρήστες στη γραμμή "προς" ή "Κοιν." Εάν δεν είναι δυνατή η αλλαγή της ορατότητας ιδιότητας μέλους για την ομάδα του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0a04c-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="0a04c-108">Για να δείτε περισσότερες λεπτομέρειες, ανατρέξτε στο [http μη εξουσιοδοτημένο στο/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="0a04c-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  