---
title: Χρήση DLP στους κανόνες μεταφοράς
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915180"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="e00cf-102">Χρήση DLP στους κανόνες μεταφοράς</span><span class="sxs-lookup"><span data-stu-id="e00cf-102">Using DLP in transport rules</span></span>

<span data-ttu-id="e00cf-103">Για να ενσωματώσετε την αποτροπή απώλειας δεδομένων (DLP) σε μια ήδη υπάρχουσα μεταφορά, εφαρμόστε τη συνθήκη "**Εάν το μήνυμα περιέχει...Ευαίσθητες πληροφορίες**" στη ρύθμιση κανόνα μεταφοράς.</span><span class="sxs-lookup"><span data-stu-id="e00cf-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="e00cf-104">**Για περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα:**</span><span class="sxs-lookup"><span data-stu-id="e00cf-104">**For more details, see:**</span></span>

- <span data-ttu-id="e00cf-105">Ενσωματωμένοι τύποι ευαίσθητων στοιχείων DLP στους κανόνες μεταφοράς: [Ενσωμάτωση κανόνων ευαίσθητων πληροφοριών](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="e00cf-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="e00cf-106">Μπορείτε επίσης να ελέγξετε τον κανόνα, με ή χωρίς έλεγχο πολιτικής, κάνοντας χρήση της "λειτουργίας δοκιμής" στον κανόνα.</span><span class="sxs-lookup"><span data-stu-id="e00cf-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="e00cf-107">Θα πρέπει να περιμένετε 30 λεπτά μετά τη δημιουργία του κανόνα, για να τον ελέγξετε.</span><span class="sxs-lookup"><span data-stu-id="e00cf-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="e00cf-108">Ανατρέξτε στο θέμα [Έλεγχος ροής αλληλογραφίας/κανόνες μεταφοράς](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="e00cf-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="e00cf-109">**Σημείωση**: Εάν προσπαθείτε να εφαρμόσετε μια νέα πολιτική DLP με τους κανόνες μεταφοράς που εφαρμόζονται στην EAC, χρησιμοποιήστε αντί αυτού τις [Πολιτικές DLP του κέντρου ασφαλείας και συμμόρφωσης](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e00cf-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
