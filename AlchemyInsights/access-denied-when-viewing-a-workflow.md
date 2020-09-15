---
title: Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688802"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="05be8-102">Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας</span><span class="sxs-lookup"><span data-stu-id="05be8-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="05be8-103">Οι ροές εργασίας του SharePoint 2013 που επιχειρούν να στείλουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint μπορούν να αποτύχουν με ένα μήνυμα σφάλματος "δεν επιτρέπεται η πρόσβαση" Εάν η ιδιότητα μέλους της ομάδας του SharePoint δεν έχει τεθεί σε όλους.</span><span class="sxs-lookup"><span data-stu-id="05be8-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="05be8-104">**Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:**</span><span class="sxs-lookup"><span data-stu-id="05be8-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="05be8-105">Να επιτρέπεται σε όλους να βλέπουν τα μέλη της ομάδας του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="05be8-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="05be8-106">Καταργήστε την ομάδα του SharePoint από τη γραμμή "προς" ή "Κοιν." του μηνύματος ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="05be8-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="05be8-107">Προσθέστε ρητά τους χρήστες στη γραμμή προς ή Κοιν., εάν δεν είναι δυνατή η αλλαγή της ορατότητας της ιδιότητας μέλους για την ομάδα του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="05be8-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="05be8-108">Για να δείτε περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα [http μη εξουσιοδοτημένο προς/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="05be8-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  