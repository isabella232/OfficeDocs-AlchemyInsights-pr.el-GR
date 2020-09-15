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
# <a name="access-denied-when-viewing-a-workflow"></a>Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας

Οι ροές εργασίας του SharePoint 2013 που επιχειρούν να στείλουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint μπορούν να αποτύχουν με ένα μήνυμα σφάλματος "δεν επιτρέπεται η πρόσβαση" Εάν η ιδιότητα μέλους της ομάδας του SharePoint δεν έχει τεθεί σε όλους.
  
 **Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:**
  
 1. Να επιτρέπεται σε όλους να βλέπουν τα μέλη της ομάδας του SharePoint.
  
 2. Καταργήστε την ομάδα του SharePoint από τη γραμμή "προς" ή "Κοιν." του μηνύματος ηλεκτρονικού ταχυδρομείου.
  
 3. Προσθέστε ρητά τους χρήστες στη γραμμή προς ή Κοιν., εάν δεν είναι δυνατή η αλλαγή της ορατότητας της ιδιότητας μέλους για την ομάδα του SharePoint.
  
Για να δείτε περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα [http μη εξουσιοδοτημένο προς/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  