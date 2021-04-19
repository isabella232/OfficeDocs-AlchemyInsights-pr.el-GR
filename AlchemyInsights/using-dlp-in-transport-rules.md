---
title: Χρήση DLP στους κανόνες μεταφοράς
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827216"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="2e47b-102">Χρήση DLP στους κανόνες μεταφοράς</span><span class="sxs-lookup"><span data-stu-id="2e47b-102">Using DLP in transport rules</span></span>

<span data-ttu-id="2e47b-103">Για να ενσωματώσετε την αποτροπή απώλειας δεδομένων (DLP) σε μια ήδη υπάρχουσα μεταφορά, εφαρμόστε τη συνθήκη "**Εάν το μήνυμα περιέχει...Ευαίσθητες πληροφορίες**" στη ρύθμιση κανόνα μεταφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e47b-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="2e47b-104">**Για περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα:**</span><span class="sxs-lookup"><span data-stu-id="2e47b-104">**For more details, see:**</span></span>

- <span data-ttu-id="2e47b-105">Ενσωματωμένοι τύποι ευαίσθητων στοιχείων DLP στους κανόνες μεταφοράς: [Ενσωμάτωση κανόνων ευαίσθητων πληροφοριών](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="2e47b-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="2e47b-106">Μπορείτε επίσης να ελέγξετε τον κανόνα, με ή χωρίς έλεγχο πολιτικής, κάνοντας χρήση της "λειτουργίας δοκιμής" στον κανόνα.</span><span class="sxs-lookup"><span data-stu-id="2e47b-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="2e47b-107">Θα πρέπει να περιμένετε 30 λεπτά μετά τη δημιουργία του κανόνα, για να τον ελέγξετε.</span><span class="sxs-lookup"><span data-stu-id="2e47b-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="2e47b-108">Ανατρέξτε στο θέμα [Έλεγχος ροής αλληλογραφίας/κανόνες μεταφοράς](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="2e47b-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="2e47b-109">**Σημείωση**: Εάν προσπαθείτε να εφαρμόσετε μια νέα πολιτική DLP με τους κανόνες μεταφοράς που εφαρμόζονται στην EAC, χρησιμοποιήστε αντί αυτού τις [Πολιτικές DLP του κέντρου ασφαλείας και συμμόρφωσης](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="2e47b-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
