---
title: Μεγάλες λίστες του SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720133"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="2f0ad-102">Εργασία με μεγάλες λίστες και βιβλιοθήκες στο SharePoint</span><span class="sxs-lookup"><span data-stu-id="2f0ad-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="2f0ad-103">Οι λίστες και οι βιβλιοθήκες του SharePoint μπορούν να περιέχουν έως και στοιχεία του 30.000.000, αλλά όταν έχουν περισσότερα από 5.000 στοιχεία, ενδέχεται να δείτε ένα σφάλμα ορίου προβολής λίστας όταν προσπαθείτε να εργαστείτε μαζί τους.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="2f0ad-104">Αυτό το όριο έχει ισχύ για τη διατήρηση της απόδοσης της υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="2f0ad-105">Δεν μπορεί να αλλάξει.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-105">It can't be changed.</span></span> <span data-ttu-id="2f0ad-106">Για να αποφύγετε το πάτημα αυτού του ορίου:</span><span class="sxs-lookup"><span data-stu-id="2f0ad-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="2f0ad-107">**Χρήση σύγχρονων**</span><span class="sxs-lookup"><span data-stu-id="2f0ad-107">**Use modern**</span></span>

<span data-ttu-id="2f0ad-108">Οι προβολές που εμφανίζουν πολλά στοιχεία λειτουργούν καλύτερα στη σύγχρονη εμπειρία.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="2f0ad-109">[Χρησιμοποιήστε τη σύγχρονη εμπειρία](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) για να αποφύγετε σφάλματα που μπορεί να δείτε στην κλασική εμπειρία.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="2f0ad-110">**Προσθήκη ευρετηρίων**</span><span class="sxs-lookup"><span data-stu-id="2f0ad-110">**Add indexes**</span></span>

<span data-ttu-id="2f0ad-111">Όταν φιλτράρετε ή ταξινομήσετε κατά μια στήλη που δεν έχει ευρετήριο, ενδέχεται να εμφανιστεί ένα μήνυμα σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="2f0ad-112">[Προσθέστε ένα ευρετήριο](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) με μη αυτόματο τρόπο από τις **Ρυθμίσεις λίστας** στο μενού "Ρυθμίσεις" και, στη συνέχεια, στις **στήλες με ευρετήριο**.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="2f0ad-113">**Επεξεργασία της προβολής λίστας**</span><span class="sxs-lookup"><span data-stu-id="2f0ad-113">**Edit the list view**</span></span>

<span data-ttu-id="2f0ad-114">Εάν παρουσιαστεί σφάλμα κατά την εργασία με μια μεγάλη λίστα, [επεξεργαστείτε την προβολή λίστας](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="2f0ad-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="2f0ad-115">Οι παρακάτω τέσσερις αλλαγές θα αφαιρέσουν τα σφάλματα ορίου προβολής λίστας.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="2f0ad-116">Κάντε και τις τέσσερις αλλαγές για να καταργήσετε όλα τα σφάλματα.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="2f0ad-117">Εάν εξακολουθείτε να λαμβάνετε σφάλματα, επιλέξτε [Διαχείριση μεγάλων λιστών και βιβλιοθηκών](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="2f0ad-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="2f0ad-118">Επιλέξτε **κανένα** και από τα δύο **Πρώτα ταξινομήστε κατά τη στήλη** και **, στη συνέχεια, ταξινομήστε κατά τη στήλη**.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="2f0ad-119">Επιλέξτε **κανένα** και από τις δύο **πρώτες ομάδες κατά τη στήλη** και **, στη συνέχεια, ομαδοποίηση κατά τη στήλη**.</span><span class="sxs-lookup"><span data-stu-id="2f0ad-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="2f0ad-120">Επιλέξτε **κανένα** για όλες τις στήλες στην ενότητα **σύνολα** .</span><span class="sxs-lookup"><span data-stu-id="2f0ad-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="2f0ad-121">Καταργήστε την επιλογή όλων εκτός από μία στήλη για εμφάνιση από την ενότητα **στήλες** .</span><span class="sxs-lookup"><span data-stu-id="2f0ad-121">Deselect all but one column for display from the **Columns** section.</span></span>

