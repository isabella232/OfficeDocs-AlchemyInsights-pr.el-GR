---
title: Τρόπος απενεργοποίησης εξωτερικών ομάδων
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
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704128"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="4e8c0-102">Τρόπος απενεργοποίησης εξωτερικών ομάδων</span><span class="sxs-lookup"><span data-stu-id="4e8c0-102">How to disable External Groups</span></span>

<span data-ttu-id="4e8c0-103">Το Yammer εξωτερική ανταλλαγή μηνυμάτων εφαρμόζει κανόνες μεταφοράς του Exchange (ETR), ένα πρόγραμμα στοιχείων ενεργητικού για να αποτρέψει την κοινή χρήση των πληροφοριών της εταιρείας.</span><span class="sxs-lookup"><span data-stu-id="4e8c0-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="4e8c0-104">Για να περιορίσετε τους χρήστες από τη δημιουργία εξωτερικών ομάδων, πρέπει να ρυθμίσετε τις παραμέτρους ενός κανόνα μεταφοράς του Exchange (ETR) και, στη συνέχεια, να ρυθμίσετε τις παραμέτρους του Yammer ώστε να χρησιμοποιεί τον κανόνα μεταφοράς του Exchange για τον αποκλεισμό εξωτερικών μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="4e8c0-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="4e8c0-105">Αφού δημιουργήσετε έναν κανόνα στο κέντρο διαχείρισης του Exchange Online, ακολουθήστε τα παρακάτω βήματα για να ορίσετε το ETR να εφαρμόζεται στο Yammer:</span><span class="sxs-lookup"><span data-stu-id="4e8c0-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="4e8c0-106">Συνδεθείτε στο Yammer ως επαληθευμένος διαχειριστής και στο **Κέντρο διαχείρισης του Yammer**, μεταβείτε στις \*\* \> ρυθμίσεις ασφαλείας του περιεχομένου C και ασφαλείας.\*\*</span><span class="sxs-lookup"><span data-stu-id="4e8c0-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="4e8c0-107">Στην περιοχή **εξωτερική ανταλλαγή μηνυμάτων**, επιλέξτε **επιβολή των κανόνων μεταφοράς του Exchange Online Exchange (ETR) στο Yammer.**</span><span class="sxs-lookup"><span data-stu-id="4e8c0-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="4e8c0-108">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="4e8c0-108">Choose **Save**.</span></span>

<span data-ttu-id="4e8c0-109">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα απενεργοποίηση εξωτερικής ανταλλαγής μηνυμάτων σε δίκτυο Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="4e8c0-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  