---
title: Τρόπος απενεργοποίησης της εξωτερικής ομάδες
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384825"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="ea272-102">Τρόπος απενεργοποίησης της εξωτερικής ομάδες</span><span class="sxs-lookup"><span data-stu-id="ea272-102">How to disable External Groups</span></span>

<span data-ttu-id="ea272-103">Yammer εξωτερική ανταλλαγή μηνυμάτων εφαρμόζει κανόνες μεταφοράς (ETRs), ένα σύνολο πριν από την ενεργοποίηση στοιχείων ελέγχου για να αποτρέψετε την κοινή χρήση πληροφοριών εταιρεία Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea272-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="ea272-104">Για να περιορίσετε τους χρήστες από τη δημιουργία εξωτερικών ομάδων, πρέπει να ρυθμίσετε τις παραμέτρους ενός κανόνα μεταφοράς του Exchange (ETR) και, στη συνέχεια, ρυθμίστε τις παραμέτρους Yammer, για να χρησιμοποιήσετε τον κανόνα μεταφοράς του Exchange για να αποκλείσετε την εξωτερική ανταλλαγή μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="ea272-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="ea272-105">Αφού έχετε δημιουργήσει έναν κανόνα στο Exchange Online Κέντρο διαχείρισης, ακολουθήστε τα εξής βήματα για να ορίσετε ETR για να εφαρμόσετε στο Yammer:</span><span class="sxs-lookup"><span data-stu-id="ea272-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="ea272-106">Συνδεθείτε στο Yammer ως διαχειριστής επιβεβαιωμένα, και το **Yammer Κέντρο διαχείρισης**, μεταβείτε στο C **περιεχομένου και ασφαλείας \> ρυθμίσεις ασφαλείας.**</span><span class="sxs-lookup"><span data-stu-id="ea272-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="ea272-107">Στην περιοχή **Εξωτερική ανταλλαγή μηνυμάτων**, επιλέξτε **εφαρμογή σας Exchange Online Exchange μεταφοράς κανόνες (ETRs) στο Yammer.**</span><span class="sxs-lookup"><span data-stu-id="ea272-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="ea272-108">Επιλέξτε " **Αποθήκευση**".</span><span class="sxs-lookup"><span data-stu-id="ea272-108">Choose **Save**.</span></span>

<span data-ttu-id="ea272-109">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Έλεγχος εξωτερικού ανταλλαγής μηνυμάτων στο δίκτυο Yammer με κανόνες μεταφοράς του Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="ea272-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  