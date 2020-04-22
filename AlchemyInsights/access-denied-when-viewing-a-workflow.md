---
title: Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687330"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας

Οι ροές εργασίας του SharePoint 2013 που επιχειρούν να στείλουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint ενδέχεται να αποτύχουν με ένα μήνυμα λάθους "Δεν επιτρέπεται η πρόσβαση", εάν η ιδιότητα μέλους της ομάδας του SharePoint δεν έχει οριστεί σε όλους.
  
 **Για να επιλύσετε αυτό το ζήτημα, κάντε τα εξής βήματα:**
  
 1. Επιτρέψτε σε όλους να βλέπουν τα μέλη της ομάδας του SharePoint.
  
 2. Καταργήστε την ομάδα του SharePoint από τη γραμμή Προς ή ΚΟΙΝΑ του μηνύματος ηλεκτρονικού ταχυδρομείου.
  
 3. Προσθέστε ρητά τους χρήστες στη γραμμή Προς ή ΚΟΙΝΑ, εάν δεν είναι δυνατή η αλλαγή της ορατότητας ιδιότητας μέλους για την ομάδα του SharePoint.
  
Για να προβάλετε περισσότερες λεπτομέρειες, ανατρέξτε στο [HTTP Μη εξουσιοδοτημένο στο /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  