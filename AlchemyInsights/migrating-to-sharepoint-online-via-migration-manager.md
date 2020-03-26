---
title: Μετεγκατάσταση στο SharePoint Online μέσω του Migration Manager
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932192"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="a6929-102">Μετεγκατάσταση στο SharePoint Online μέσω του Migration Manager</span><span class="sxs-lookup"><span data-stu-id="a6929-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="a6929-103">**Σημαντικό**: Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν σημαντικές επιχειρηματικές εφαρμογές με την υπηρεσία να εκτελείται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="a6929-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a6929-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="a6929-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a6929-105">Σε αυτούς τους πρωτόγνωρους καιρούς, λαμβάνουμε μέτρα για να εξασφαλίσουμε ότι οι υπηρεσίες του SharePoint Online και του OneDrive θα παραμείνουν διαθέσιμες και αξιόπιστες στον ύψιστο βαθμό για τους χρήστες σας, οι οποίοι εξαρτώνται από την υπηρεσία περισσότερο από ποτέ για απομακρυσμένες εργασίες.</span><span class="sxs-lookup"><span data-stu-id="a6929-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a6929-106">Για αυτόν τον στόχο, εφαρμόσαμε αυστηρότερα όρια περιορισμού σε εφαρμογές παρασκηνίου (μετεγκατάσταση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τη διάρκεια των πρωινών ωρών των εργάσιμων ημερών.</span><span class="sxs-lookup"><span data-stu-id="a6929-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a6929-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη απόδοση κατά τη διάρκεια αυτών των ωρών.</span><span class="sxs-lookup"><span data-stu-id="a6929-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a6929-108">Ωστόσο, κατά τις βραδινές ώρες της περιοχής σας και τα σαββατοκύριακα, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά μεγαλύτερο όγκο αιτήσεων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="a6929-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a6929-109">**Migration Manager**</span><span class="sxs-lookup"><span data-stu-id="a6929-109">**Migration Manager**</span></span>

<span data-ttu-id="a6929-110">Βρισκόμενη στο σύγχρονο κέντρο διαχείρισης του SharePoint, το Migration Manager σάς καθοδηγεί στη ρύθμιση των προγραμμάτων-πελατών σας και στη δημιουργία των εργασιών σας.</span><span class="sxs-lookup"><span data-stu-id="a6929-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="a6929-111">Μπορείτε να καθορίσετε καθολικές ρυθμίσεις ή ρυθμίσεις επιπέδου εργασιών, να προβάλετε την πρόοδο των εργασιών όλων των χρηστών και να κάνετε λήψη συγκεντρωτικών αναφορών σύνοψης και επιπέδου εργασιών.</span><span class="sxs-lookup"><span data-stu-id="a6929-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="a6929-112">Γρήγορα αποτελέσματα με το Migration Manager</span><span class="sxs-lookup"><span data-stu-id="a6929-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="a6929-113">Ρύθμιση προγραμμάτων-πελατών στο Migration Manager</span><span class="sxs-lookup"><span data-stu-id="a6929-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="a6929-114">Ρυθμίσεις του Migration Manager</span><span class="sxs-lookup"><span data-stu-id="a6929-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
