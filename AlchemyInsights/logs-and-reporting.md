---
title: Αρχεία καταγραφής και αναφορές
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035915"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="c4154-102">Αρχεία καταγραφής και αναφορές</span><span class="sxs-lookup"><span data-stu-id="c4154-102">Logs and Reporting</span></span>

<span data-ttu-id="c4154-103">[Συνήθεις ερωτήσεις για τις αναφορές του Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) απαντήσεις σε συνήθεις ερωτήσεις σχετικά με την αναφορά του Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c4154-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="c4154-104">Για περισσότερες πληροφορίες, ανατρέξτε στην [αναφορά του Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="c4154-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="c4154-105">**Αντιμετώπιση προβλημάτων με τον έλεγχο**</span><span class="sxs-lookup"><span data-stu-id="c4154-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="c4154-106">Αν αντιμετωπίζετε προβλήματα με την βλέπουν ορισμένες δραστηριότητες ελέγχου και η δραστηριότητα που λείπει βρίσκεται σε αυτή [τη λίστα,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)στείλτε ένα δελτίο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="c4154-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="c4154-107">Εάν αντιμετωπίζετε προβλήματα με την βλέπουν οποιαδήποτε αρχεία καταγραφής ελέγχου στο μισθωτή σας, στείλτε ένα δελτίο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="c4154-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="c4154-108">Εάν οι δραστηριότητες ελέγχου δεν εμφανίζονται αμέσως στην [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) πύλη Azure, ελέγξτε τις πληροφορίες λανθάνοντα χρόνου μας και κάντε ένα δελτίο υποστήριξης εάν η καθυστέρηση υπερβεί τον τεκμηριωμένο λανθάνοντα χρόνο.</span><span class="sxs-lookup"><span data-stu-id="c4154-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="c4154-109">Διατήρηση αρχείων καταγραφής δραστηριότητας του Azure AD</span><span class="sxs-lookup"><span data-stu-id="c4154-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="c4154-110">Εάν δεν βλέπετε όλο τον έλεγχο για το εύρος ημερομηνιών που επιλέξατε, μπορείτε να κάνετε λήψη έως και 250 γραμμώνK (ταξινομημένες κατά την πιο πρόσφατη) είσοδο από την πύλη Azure.</span><span class="sxs-lookup"><span data-stu-id="c4154-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="c4154-111">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Λήψη δραστηριοτήτων ελέγχου".](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="c4154-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="c4154-112">**Αντιμετώπιση προβλημάτων με τις είσοδοι**</span><span class="sxs-lookup"><span data-stu-id="c4154-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="c4154-113">Μπορείτε να δείτε τα δεδομένα των τελευταίων 30 ημερών μόνο εάν έχετε μια άδεια χρήσης Azure AD Premium (P1 ή P2) για το μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="c4154-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="c4154-114">Οι είσοδοι είναι διαθέσιμες μόνο για τους μισθωτές Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="c4154-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="c4154-115">Δεν είναι διαθέσιμη για μισθωτές δωρεάν ή βασικής άδειας χρήσης.</span><span class="sxs-lookup"><span data-stu-id="c4154-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="c4154-116">Εάν ο μισθωτής σας έχει άδεια χρήσης Premium P1 και δεν [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) μπορείτε να δείτε τις εισόδους, ελέγξτε τις πληροφορίες λανθάνοντα χρόνου μας και υπογράφετε ένα δελτίο υποστήριξης εάν η καθυστέρηση υπερβεί τον τεκμηριωμένο λανθάνοντα χρόνο.</span><span class="sxs-lookup"><span data-stu-id="c4154-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="c4154-117">Εάν δεν βλέπετε όλες τις είσοδο για το εύρος ημερομηνιών που επιλέξατε, λάβετε υπόψη ότι μπορείτε να κάνετε λήψη έως 250K γραμμών (ταξινομημένες κατά την πιο πρόσφατη) των εισέλθεων από την πύλη Azure.</span><span class="sxs-lookup"><span data-stu-id="c4154-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="c4154-118">Για περισσότερες πληροφορίες, ανατρέξτε [στη λήψη των δραστηριοτήτων είσοδοι.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="c4154-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="c4154-119">**Αντιμετώπιση προβλημάτων με αναφορές ασφαλείας (χρήστες με σημαία κινδύνου, επικίνδυνη είσοδος)**</span><span class="sxs-lookup"><span data-stu-id="c4154-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="c4154-120">Χρήστες με σημαία για αναφορά ασφαλείας κινδύνου</span><span class="sxs-lookup"><span data-stu-id="c4154-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="c4154-121">Αναφορά κινδύνων για τις είσοδο στην πύλη του Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c4154-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="c4154-122">Συμβάντα κινδύνου του Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c4154-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
