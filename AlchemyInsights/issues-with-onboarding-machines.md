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
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="4fd29-102">Προβλήματα με τα μηχανήματα onboarding</span><span class="sxs-lookup"><span data-stu-id="4fd29-102">Issues with onboarding machines</span></span>

<span data-ttu-id="4fd29-103">Μπορεί να αντιμετωπίζετε προβλήματα με μηχανές ενσωμάτωσης στην υπηρεσία MDATP.</span><span class="sxs-lookup"><span data-stu-id="4fd29-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="4fd29-104">Εάν μπορείτε να αποκτήσετε πρόσβαση στον υπολογιστή τελικού χρήστη, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="4fd29-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="4fd29-105">Κάντε λήψη του διαγνωστικού [εργαλείου ανάλυσης συνδεσιμότητας προγράμματος-πελάτη.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="4fd29-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="4fd29-106">Εξαγάγετε και εκτελέστε το MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="4fd29-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="4fd29-107">Εντοπίστε το αρχείο καταγραφής διαγνωστικών στο φάκελο που ονομάζεται MDATPClientAnalyzerResult, στον ίδιο φάκελο όπου γίνεται λήψη του εργαλείου ανάλυσης.</span><span class="sxs-lookup"><span data-stu-id="4fd29-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="4fd29-108">Εξετάστε το αρχείο καταγραφής, MDATPClientAnalyzer.txt, για να βρείτε ζητήματα σύνδεσης ή ρυθμίσεων διακομιστή μεσολάβησης Internet.</span><span class="sxs-lookup"><span data-stu-id="4fd29-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>