---
title: Συνταξιοδότηση υπηρεσιών πρόσβασης
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687258"
---
# <a name="access-services-retirement"></a><span data-ttu-id="959a9-102">Συνταξιοδότηση υπηρεσιών πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="959a9-102">Access services retirement</span></span>

<span data-ttu-id="959a9-103">Όπως αρχικά ανακοινώσαμε στο MC97576, τον Μάρτιο του 2017, και συνεχίσαμε να επικοινωνούμε κατά το παρελθόν έτος, οι Υπηρεσίες Πρόσβασης αποσύρονται.</span><span class="sxs-lookup"><span data-stu-id="959a9-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="959a9-104">Η επόμενη φάση αυτής της διαδικασίας θα είναι η κατάργηση των βάσεων δεδομένων Web της Access που χρησιμοποιούν λίστες του SharePoint ως υποκείμενο χώρο αποθήκευσης δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="959a9-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="959a9-105">**Πώς με επηρεάζει αυτό;**</span><span class="sxs-lookup"><span data-stu-id="959a9-105">**How does this affect me?**</span></span>

<span data-ttu-id="959a9-106">Από τον Ιούνιο του 2019, θα σταματήσουμε τη δημιουργία νέων βάσεων δεδομένων της Access στο SharePoint Online και θα τερματίσουμε την υπηρεσία και τυχόν υπόλοιπες εφαρμογές έως τον Απρίλιο του 2020.</span><span class="sxs-lookup"><span data-stu-id="959a9-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="959a9-107">**Τι πρέπει να κάνω για να προετοιμαστώ για αυτήν την αλλαγή;**</span><span class="sxs-lookup"><span data-stu-id="959a9-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="959a9-108">Σας συνιστούμε να δημιουργήσετε ένα σχέδιο μετάβασης για τις βάσεις δεδομένων Web της Access του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="959a9-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="959a9-109">Οι διαχειριστές μπορούν να χρησιμοποιήσουν το [σαρωτή εφαρμογών SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) για να αποκτήσουν ένα απόθεμα των εφαρμογών της Access που χρησιμοποιούν οι τοποθεσίες.</span><span class="sxs-lookup"><span data-stu-id="959a9-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="959a9-110">Υπάρχουν διάφοροι τρόποι μετεγκατάστασης δεδομένων βάσεων δεδομένων Web της Access:</span><span class="sxs-lookup"><span data-stu-id="959a9-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="959a9-111">Εισαγωγή σε τοπική βάση δεδομένων της Access (. ACCDB) ή σε ένα αρχείο του Excel.</span><span class="sxs-lookup"><span data-stu-id="959a9-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="959a9-112">Συνιστούμε επίσης να εξερευνήσετε το Microsoft PowerApps ως εναλλακτική πλατφόρμα για τη δημιουργία επιχειρηματικών λύσεων χωρίς κώδικα για συσκευές web και κινητές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="959a9-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>