---
title: Συνταξιοδότηση υπηρεσιών Access Services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698682"
---
# <a name="access-services-retirement"></a><span data-ttu-id="92014-102">Συνταξιοδότηση υπηρεσιών Access Services</span><span class="sxs-lookup"><span data-stu-id="92014-102">Access services retirement</span></span>

<span data-ttu-id="92014-103">Όπως ανακοινώθηκε αρχικά στο MC97576, τον Μάρτιο του 2017, και συνέχισε να επικοινωνεί κατά το παρελθόν έτος, οι υπηρεσίες πρόσβασης αποσύρονται.</span><span class="sxs-lookup"><span data-stu-id="92014-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="92014-104">Η επόμενη φάση σε αυτήν τη διαδικασία θα είναι η κατάργηση των βάσεων δεδομένων Web της Access που χρησιμοποιούν λίστες του SharePoint ως υποκείμενες Αποθήκευση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="92014-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="92014-105">**Πώς αυτό με επηρεάζει;**</span><span class="sxs-lookup"><span data-stu-id="92014-105">**How does this affect me?**</span></span>

<span data-ttu-id="92014-106">Ξεκινώντας από τον Ιούνιο του 2019, θα διακοπεί η δημιουργία νέων βάσεων δεδομένων της Access στο SharePoint Online και θα διακοπεί η λειτουργία της υπηρεσίας και τυχόν υπόλοιπων εφαρμογών μέχρι τον Απρίλιο του 2020.</span><span class="sxs-lookup"><span data-stu-id="92014-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="92014-107">**Τι πρέπει να κάνω για να προετοιμαστώ για αυτή την αλλαγή;**</span><span class="sxs-lookup"><span data-stu-id="92014-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="92014-108">Σας συνιστούμε να δημιουργήσετε ένα πρόγραμμα μετάβασης για τις βάσεις δεδομένων Web της εταιρείας σας στην Access.</span><span class="sxs-lookup"><span data-stu-id="92014-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="92014-109">Οι διαχειριστές μπορούν να χρησιμοποιήσουν το [πρόγραμμα σάρωσης εφαρμογών του SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) για να αποκτήσουν ένα απόθεμα των εφαρμογών της Access που χρησιμοποιούν οι τοποθεσίες.</span><span class="sxs-lookup"><span data-stu-id="92014-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="92014-110">Υπάρχουν διάφοροι τρόποι για τη μετεγκατάσταση δεδομένων βάσεων δεδομένων Web της Access:</span><span class="sxs-lookup"><span data-stu-id="92014-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="92014-111">Εισαγωγή σε μια τοπική βάση δεδομένων της Access (. ACCDB) ή σε ένα αρχείο του Excel.</span><span class="sxs-lookup"><span data-stu-id="92014-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="92014-112">Συνιστούμε επίσης να εξερευνήσετε το Microsoft PowerApps ως εναλλακτική πλατφόρμα για να δημιουργήσετε λύσεις χωρίς κώδικα για τις επιχειρηματικές λύσεις για το Web και τις κινητές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="92014-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>