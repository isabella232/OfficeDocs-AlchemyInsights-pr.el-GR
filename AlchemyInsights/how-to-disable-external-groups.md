---
title: Τρόπος απενεργοποίησης της εξωτερικής ομάδες
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 09d8b134a4e99912301aa92c2e989fec9dd30a7b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656387"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="09fb5-102">Τρόπος απενεργοποίησης της εξωτερικής ομάδες</span><span class="sxs-lookup"><span data-stu-id="09fb5-102">How to disable External Groups</span></span>

<span data-ttu-id="09fb5-p101">Yammer εξωτερική ανταλλαγή μηνυμάτων εφαρμόζει κανόνες μεταφοράς (ETRs), ένα σύνολο πριν από την ενεργοποίηση στοιχείων ελέγχου για να αποτρέψετε την κοινή χρήση πληροφοριών εταιρεία Exchange. Για να περιορίσετε τους χρήστες από τη δημιουργία εξωτερικών ομάδων, πρέπει να ρυθμίσετε τις παραμέτρους ενός κανόνα μεταφοράς του Exchange (ETR) και, στη συνέχεια, ρυθμίστε τις παραμέτρους Yammer, για να χρησιμοποιήσετε τον κανόνα μεταφοράς του Exchange για να αποκλείσετε την εξωτερική ανταλλαγή μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="09fb5-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="09fb5-105">Αφού έχετε δημιουργήσει έναν κανόνα στο Exchange Online Κέντρο διαχείρισης, ακολουθήστε τα εξής βήματα για να ορίσετε ETR για να εφαρμόσετε στο Yammer:</span><span class="sxs-lookup"><span data-stu-id="09fb5-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="09fb5-106">Συνδεθείτε στο Yammer ως διαχειριστής επιβεβαιωμένα, και το **Yammer Κέντρο διαχείρισης**, μεταβείτε στο C **λλονται και ασφάλεια \> ρυθμίσεις ασφαλείας.**</span><span class="sxs-lookup"><span data-stu-id="09fb5-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="09fb5-107">Στην περιοχή **Εξωτερική ανταλλαγή μηνυμάτων**, επιλέξτε **εφαρμογή σας Exchange Online Exchange μεταφοράς κανόνες (ETRs) στο Yammer.**</span><span class="sxs-lookup"><span data-stu-id="09fb5-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="09fb5-108">Επιλέξτε " **Αποθήκευση**".</span><span class="sxs-lookup"><span data-stu-id="09fb5-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="09fb5-109">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Έλεγχος εξωτερικού ανταλλαγής μηνυμάτων στο δίκτυο Yammer με κανόνες μεταφοράς του Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="09fb5-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

