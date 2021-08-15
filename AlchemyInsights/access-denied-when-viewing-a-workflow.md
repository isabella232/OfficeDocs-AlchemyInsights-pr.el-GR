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
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955201"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Δεν επιτρέπεται η πρόσβαση κατά την προβολή μιας ροής εργασίας

SharePoint ροές εργασιών του 2013 που επιχειρούν να στείλουν ένα μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του SharePoint μπορεί να αποτύχουν με ένα μήνυμα σφάλματος "Δεν επιτρέπεται η πρόσβαση", εάν η ιδιότητα μέλους της ομάδας SharePoint δεν έχει οριστεί σε "Όλοι".
  
 **Για να επιλύσετε αυτό το πρόβλημα, κάντε τα εξής βήματα:**
  
 1. Επιτρέψτε σε όλους να βλέπουν τα μέλη της SharePoint ομάδας.
  
 2. Καταργήστε την SharePoint ομάδας από τη γραμμή "Προς" ή "Κοιν." του μηνύματος ηλεκτρονικού ταχυδρομείου.
  
 3. Προσθέστε ρητά τους χρήστες στη γραμμή "Προς" ή "Κοιν.", εάν η ορατότητα των μελών δεν μπορεί να αλλάξει SharePoint ομάδας.
  
Για να δείτε περισσότερες λεπτομέρειες, ανατρέξτε στο [http unauthorized to /_vti_bin/client.svc/sp.utilities.utility.sendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  