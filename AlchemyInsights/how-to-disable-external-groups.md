---
title: Τρόπος απενεργοποίησης των εξωτερικών ομάδων
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015620"
---
# <a name="how-to-disable-external-groups"></a>Τρόπος απενεργοποίησης των εξωτερικών ομάδων

Yammer εξωτερική ανταλλαγή μηνυμάτων εφαρμόζει Exchange μεταφοράς (ETR), ένα σύνολο προληπτικών ελέγχων για την αποτροπή της κοινής χρήσης εταιρικών πληροφοριών. Για να περιορίσετε τους χρήστες από τη δημιουργία εξωτερικών ομάδων, πρέπει να ρυθμίσετε τις παραμέτρους ενός κανόνα μεταφοράς του Exchange (ETR) και, στη συνέχεια, να ρυθμίσετε τις παραμέτρους του Yammer για να χρησιμοποιήσετε τον κανόνα μεταφοράς του Exchange για να αποκλείσετε την εξωτερική ανταλλαγή μηνυμάτων.
  
Αφού έχετε δημιουργήσει έναν κανόνα στο κέντρο διαχείρισης Exchange Online, ακολουθήστε τα παρακάτω βήματα για να ορίσετε το ETR να εφαρμόζεται σε Yammer:
  
- Συνδεθείτε στο Yammer ως επαληθευμένος διαχειριστής και, στο **κέντρο διαχείρισης Yammer,** μεταβείτε στην περιοχή "Περιεχόμενο C" και **\> "Ασφάλεια Ρυθμίσεις".**

- Στην **περιοχή "Εξωτερικά μηνύματα",** επιλέξτε **"Επιβολή κανόνων Exchange Online Exchange μεταφοράς" (ETR) στο Yammer.**

- Επιλέξτε **"Αποθήκευση".**

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Απενεργοποίηση της εξωτερικής ανταλλαγής μηνυμάτων σε Yammer δικτύου.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  