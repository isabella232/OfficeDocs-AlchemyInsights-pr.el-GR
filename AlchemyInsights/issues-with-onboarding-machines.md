---
title: Προβλήματα με τα μηχανήματα onboarding
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141467"
---
# <a name="issues-with-onboarding-machines"></a>Προβλήματα με τα μηχανήματα onboarding

Μπορεί να αντιμετωπίζετε προβλήματα με μηχανές ενσωμάτωσης στην υπηρεσία MDATP. Εάν μπορείτε να αποκτήσετε πρόσβαση στον υπολογιστή τελικού χρήστη, ακολουθήστε τα εξής βήματα:

1. Κάντε λήψη του διαγνωστικού [εργαλείου ανάλυσης συνδεσιμότητας προγράμματος-πελάτη.](https://aka.ms/mdatpanalyzer)
2. Εξαγάγετε και εκτελέστε το MDATPAnalyzer.cmd.
3. Εντοπίστε το αρχείο καταγραφής διαγνωστικών στο φάκελο που ονομάζεται MDATPClientAnalyzerResult, στον ίδιο φάκελο όπου γίνεται λήψη του εργαλείου ανάλυσης.
4. Εξετάστε το αρχείο καταγραφής, MDATPClientAnalyzer.txt, για να βρείτε ζητήματα σύνδεσης ή ρυθμίσεων διακομιστή μεσολάβησης Internet.