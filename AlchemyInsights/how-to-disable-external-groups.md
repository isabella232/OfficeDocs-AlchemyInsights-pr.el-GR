---
title: Τρόπος απενεργοποίησης εξωτερικών ομάδων
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720768"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="06136-102">Τρόπος απενεργοποίησης εξωτερικών ομάδων</span><span class="sxs-lookup"><span data-stu-id="06136-102">How to disable External Groups</span></span>

<span data-ttu-id="06136-103">Η εξωτερική ανταλλαγή μηνυμάτων Του Yammer εφαρμόζει τους Κανόνες μεταφοράς του Exchange (ETRs), ένα σύνολο προληπτικών στοιχείων ελέγχου για την αποτροπή της κοινής χρήσης των εταιρικών πληροφοριών.</span><span class="sxs-lookup"><span data-stu-id="06136-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="06136-104">Για να περιορίσετε τους χρήστες από τη δημιουργία εξωτερικών ομάδων, πρέπει να ρυθμίσετε τις παραμέτρους ενός κανόνα μεταφοράς του Exchange (ETR) και, στη συνέχεια, να ρυθμίσετε τις παραμέτρους του Yammer ώστε να χρησιμοποιεί τον κανόνα μεταφοράς του Exchange για τον αποκλεισμό εξωτερικών μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="06136-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="06136-105">Αφού δημιουργήσετε έναν κανόνα στο Κέντρο διαχείρισης του Exchange Online, ακολουθήστε τα εξής βήματα για να ορίσετε το ETR να εφαρμόζεται στο Yammer:</span><span class="sxs-lookup"><span data-stu-id="06136-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="06136-106">Συνδεθείτε στο Yammer ως επαληθευμένοδιαχειριστή και στο **κέντρο διαχείρισης του Yammer**, μεταβείτε στις **Ρυθμίσεις \> c περιεχομένου και ασφαλείας ασφαλείας.**</span><span class="sxs-lookup"><span data-stu-id="06136-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="06136-107">Στην περιοχή **Εξωτερική ανταλλαγή μηνυμάτων**, επιλέξτε **Επιβολή των κανόνων μεταφοράς του Exchange online exchange (ETRs) στο Yammer.**</span><span class="sxs-lookup"><span data-stu-id="06136-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="06136-108">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="06136-108">Choose **Save**.</span></span>

<span data-ttu-id="06136-109">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Απενεργοποίηση εξωτερικής ανταλλαγής μηνυμάτων σε δίκτυο Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="06136-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  