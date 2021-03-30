---
title: Βοήθεια σχετικά με τη ρύθμιση εμφάνισης νυχτερινού φωτισμού
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404661"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="2fd4d-102">Βοήθεια σχετικά με τη ρύθμιση εμφάνισης νυχτερινού φωτισμού</span><span class="sxs-lookup"><span data-stu-id="2fd4d-102">Help with the night light display setting</span></span>

<span data-ttu-id="2fd4d-103">Για να μάθετε περισσότερα σχετικά με τις ρυθμίσεις νυχτερινής εμφάνισης, ανατρέξτε στο θέμα Ρύθμιση [της οθόνης σας για νυχτερινή ώρα στα Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="2fd4d-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="2fd4d-104">Εάν οι επιλογές νυχτερινού φωτισμού είναι γκρι στις "Ρυθμίσεις", ελέγξτε το πρόγραμμα οδήγησης οθόνης:</span><span class="sxs-lookup"><span data-stu-id="2fd4d-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="2fd4d-105">Κάντε κλικ στο πλαίσιο αναζήτησης στη γραμμή εργασιών και πληκτρολογήστε **"Διαχείριση συσκευών"** και, στη συνέχεια, επιλέξτε **"Διαχείριση συσκευών"** στα αποτελέσματα αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="2fd4d-106">Ανάπτυξη **προσαρμογέων οθόνης.**</span><span class="sxs-lookup"><span data-stu-id="2fd4d-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="2fd4d-107">Δυστυχώς, η δυνατότητα νυχτερινού φωτισμού δεν είναι διαθέσιμη εάν η συσκευή σας χρησιμοποιεί ένα πρόγραμμα οδήγησης DisplayLink ή ένα πρόγραμμα οδήγησης Βασικής οθόνης.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="2fd4d-108">Η δυνατότητα νυχτερινού φωτισμού χρησιμοποιεί την πρόσφατη τεχνολογία γραφικών, επομένως ίσως χρειαστεί να ενημερώσετε το πρόγραμμα οδήγησης οθόνης:</span><span class="sxs-lookup"><span data-stu-id="2fd4d-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="2fd4d-109">Ελέγξτε για ενημερώσεις, στη σελίδα **"Έναρξη**  >  **ενημέρωσης**  >  **ρυθμίσεων" & "Έλεγχος** ασφαλείας  >  **του Windows**  >  **Update" για ενημερώσεις.**</span><span class="sxs-lookup"><span data-stu-id="2fd4d-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="2fd4d-110">OR</span><span class="sxs-lookup"><span data-stu-id="2fd4d-110">OR</span></span>

- <span data-ttu-id="2fd4d-111">Επισκεφθείτε την τοποθεσία Web υποστήριξης του κατασκευαστή του υλικού σας για να κάνετε λήψη και εγκατάσταση των πιο πρόσφατων προγραμμάτων οδήγησης οθόνης με μη αυτόματο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="2fd4d-112">Επαναφορά νυχτερινού φωτισμού στο μητρώο</span><span class="sxs-lookup"><span data-stu-id="2fd4d-112">Reset night light in the registry</span></span>

<span data-ttu-id="2fd4d-113">Εάν η ενημέρωση του προγράμματος οδήγησης οθόνης δεν είχε αποτέλεσμα, ίσως χρειαστεί να επαναφέρετε το νυχτερινό φως στο μητρώο.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="2fd4d-114">**Προσοχή:** Αυτό το βήμα αντιμετώπισης προβλημάτων συνιστάται μόνο για προχωρημένους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="2fd4d-115">Εάν τροποποιήσετε εσφαλμένα το μητρώο, ενδέχεται να προκύψουν σοβαρά προβλήματα.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="2fd4d-116">Για πρόσθετη προστασία, κάντε αντίγραφα ασφαλείας του μητρώου πριν το τροποποιήσετε, ώστε να μπορείτε να το επαναφέρετε, εάν προκύψουν προβλήματα.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="2fd4d-117">Στο πλαίσιο αναζήτησης, πληκτρολογήστε **regedit και, στη** συνέχεια, επιλέξτε **"Επεξεργαστής μητρώου"** στα αποτελέσματα αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="2fd4d-118">Μεταβείτε στο ακόλουθο κλειδί μητρώου:</span><span class="sxs-lookup"><span data-stu-id="2fd4d-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="2fd4d-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="2fd4d-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="2fd4d-120">Εξαγάγετε και, στη συνέχεια, διαγράψτε το ακόλουθο δευτερεύον κλειδί:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="2fd4d-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="2fd4d-121">Εξαγάγετε και, στη συνέχεια, διαγράψτε το ακόλουθο δευτερεύον κλειδί:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="2fd4d-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="2fd4d-122">Επανεκκινήστε τα Windows και επαληθεύστε εάν είναι διαθέσιμες οι επιλογές νυχτερινού φωτισμού.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-122">Restart Windows and verify if the night light options are available.</span></span>


