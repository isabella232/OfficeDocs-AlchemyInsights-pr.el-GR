---
title: Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918828"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="41db1-102">Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας</span><span class="sxs-lookup"><span data-stu-id="41db1-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="41db1-103">Ροές εργασίας του SharePoint 2013 που προσπαθούν να σας στείλει ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint μπορεί να αποτύχει με μήνυμα λάθους "Δεν επιτρέπεται η πρόσβαση", εάν δεν έχει οριστεί η ιδιότητα μέλους της ομάδας του SharePoint σε όλους τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="41db1-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="41db1-104">**Για να επιλύσετε αυτό το ζήτημα, κάντε τα εξής βήματα:**</span><span class="sxs-lookup"><span data-stu-id="41db1-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="41db1-105">Επιτρέπονται όλοι οι συμμετέχοντες για να δείτε τα μέλη της ομάδας του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="41db1-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="41db1-106">Καταργήστε την ομάδα του SharePoint από το "προς" ή "Κοιν." γραμμή του μηνύματος ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="41db1-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="41db1-107">Ρητά, προσθέστε τους χρήστες για να "προς" ή "Κοιν." γραμμή Εάν δεν μπορεί να αλλάξει την ορατότητα της ιδιότητας μέλους ομάδας του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="41db1-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="41db1-108">Για να προβάλετε περισσότερες λεπτομέρειες, ανατρέξτε σε [Μη εξουσιοδοτημένη HTTP για να /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="41db1-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

