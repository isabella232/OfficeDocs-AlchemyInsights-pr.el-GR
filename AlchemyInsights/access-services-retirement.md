---
title: Πρόσβαση στις υπηρεσίες συνταξιοδότησης
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747784"
---
# <a name="access-services-retirement"></a><span data-ttu-id="4a205-102">Πρόσβαση στις υπηρεσίες συνταξιοδότησης</span><span class="sxs-lookup"><span data-stu-id="4a205-102">Access services retirement</span></span>

<span data-ttu-id="4a205-103">Όπως αρχικά ανακοινώθηκε το MC97576, τον Μάρτιο του 2017, και συνέχισε να επικοινωνεί κατά το παρελθόν έτος οι υπηρεσίες πρόσβασης συνταξιοδοτήθηκε από το Office 365.</span><span class="sxs-lookup"><span data-stu-id="4a205-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="4a205-104">Η επόμενη φάση σε αυτήν τη διεργασία θα είναι η κατάργηση των βάσεων δεδομένων Web της Access που χρησιμοποιούν λίστες του SharePoint ως υποκείμενη Αποθήκευση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="4a205-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="4a205-105">**Πώς με επηρεάζει αυτό;**</span><span class="sxs-lookup"><span data-stu-id="4a205-105">**How does this affect me?**</span></span>

<span data-ttu-id="4a205-106">Ξεκινώντας Ιουνίου 2019, θα σταματήσει τη δημιουργία νέων βάσεων δεδομένων της Access στο SharePoint Online και τερματίστε την υπηρεσία και τυχόν υπόλοιπες εφαρμογές μέχρι τον Απρίλιο 2020.</span><span class="sxs-lookup"><span data-stu-id="4a205-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="4a205-107">**Τι πρέπει να κάνω για να προετοιμαστώ γι ' αυτή την αλλαγή;**</span><span class="sxs-lookup"><span data-stu-id="4a205-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="4a205-108">Σας συνιστούμε να δημιουργήσετε ένα σχέδιο μετάβασης για τις βάσεις δεδομένων Web της εταιρείας σας στην Access.</span><span class="sxs-lookup"><span data-stu-id="4a205-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="4a205-109">Οι διαχειριστές μπορούν να χρησιμοποιήσουν το [σαρωτή εφαρμογών του SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) για να αποκτήσουν ένα απόθεμα των εφαρμογών της Access που χρησιμοποιούν οι ιστότοποι.</span><span class="sxs-lookup"><span data-stu-id="4a205-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="4a205-110">Υπάρχουν διάφοροι τρόποι για να μετεγκαταστήσετε δεδομένα βάσεων δεδομένων Web της Access:</span><span class="sxs-lookup"><span data-stu-id="4a205-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="4a205-111">Εισαγωγή σε μια τοπική βάση δεδομένων της Access (. ACCDB) ή σε ένα αρχείο του Excel.</span><span class="sxs-lookup"><span data-stu-id="4a205-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="4a205-112">Συνιστούμε επίσης να εξερευνήσετε το Microsoft PowerApps ως εναλλακτική πλατφόρμα για τη δημιουργία επιχειρηματικών λύσεων χωρίς κώδικα για διαδικτυακές και κινητές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="4a205-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>