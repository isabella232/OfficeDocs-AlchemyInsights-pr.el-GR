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
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495823"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας

Ροές εργασίας του SharePoint 2013 που προσπαθούν να σας στείλει ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint μπορεί να αποτύχει με μήνυμα λάθους "Δεν επιτρέπεται η πρόσβαση", εάν δεν έχει οριστεί η ιδιότητα μέλους της ομάδας του SharePoint σε όλους τους χρήστες.
  
 **Για να επιλύσετε αυτό το ζήτημα, κάντε τα εξής βήματα:**
  
 1. Επιτρέπονται όλοι οι συμμετέχοντες για να δείτε τα μέλη της ομάδας του SharePoint.
  
 2. Καταργήστε την ομάδα του SharePoint από το "προς" ή "Κοιν." γραμμή του μηνύματος ηλεκτρονικού ταχυδρομείου.
  
 3. Ρητά, προσθέστε τους χρήστες για να "προς" ή "Κοιν." γραμμή Εάν δεν μπορεί να αλλάξει την ορατότητα της ιδιότητας μέλους ομάδας του SharePoint.
  
Για να προβάλετε περισσότερες λεπτομέρειες, ανατρέξτε σε [Μη εξουσιοδοτημένη HTTP για να /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  