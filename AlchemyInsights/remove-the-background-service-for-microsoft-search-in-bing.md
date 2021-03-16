---
title: Κατάργηση της υπηρεσίας φόντου για την Αναζήτηση της Microsoft στο Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816199"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="5a459-102">Κατάργηση της υπηρεσίας φόντου για την Αναζήτηση της Microsoft στο Bing</span><span class="sxs-lookup"><span data-stu-id="5a459-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="5a459-103">Για να καταργήσετε την υπηρεσία φόντου για την Αναζήτηση της Microsoft στο Bing, μπορείτε να δοκιμάσετε τις ακόλουθες λύσεις:</span><span class="sxs-lookup"><span data-stu-id="5a459-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="5a459-104">Για να επιστρέψετε στις αρχικές ρυθμίσεις του μηχανισμού αναζήτησης, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="5a459-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="5a459-105">a.</span><span class="sxs-lookup"><span data-stu-id="5a459-105">a.</span></span> <span data-ttu-id="5a459-106">Απενεργοποιήστε **την επιλογή "Χρήση του Bing ως προεπιλεγμένου [μηχανισμού αναζήτησης".](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**</span><span class="sxs-lookup"><span data-stu-id="5a459-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="5a459-107">b.</span><span class="sxs-lookup"><span data-stu-id="5a459-107">b.</span></span> <span data-ttu-id="5a459-108">[Μεταβείτε στο κέντρο διαχείρισης του Microsoft 365 και καταργήστε](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) τη ρύθμιση που επηρεάζει όλους τους χρήστες στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="5a459-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="5a459-109">Για να καταργήσετε την υπηρεσία φόντου από μια μεμονωμένη συσκευή, κάντε τις ακόλουθες εργασίες:</span><span class="sxs-lookup"><span data-stu-id="5a459-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="5a459-110">a.</span><span class="sxs-lookup"><span data-stu-id="5a459-110">a.</span></span> <span data-ttu-id="5a459-111">Επιλέξτε **"Πίνακας Ελέγχου" > "Προγράμματα" > "Προγράμματα και δυνατότητες".**</span><span class="sxs-lookup"><span data-stu-id="5a459-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="5a459-112">b.</span><span class="sxs-lookup"><span data-stu-id="5a459-112">b.</span></span> <span data-ttu-id="5a459-113">Κάντε δεξί κλικ στην **Αναζήτηση της Microsoft στο Bing κάτω από τη** λίστα των εγκατεστημένων προγραμμάτων και, στη συνέχεια, κάντε κλικ στην επιλογή "Κατάργηση **εγκατάστασης".**</span><span class="sxs-lookup"><span data-stu-id="5a459-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="5a459-114">Για να καταργήσετε την υπηρεσία φόντου από πολλές συσκευές στον οργανισμό σας, συνδεθείτε ως διαχειριστής και εκτελέστε την ακόλουθη εντολή σε μια δέσμη ενεργειών:</span><span class="sxs-lookup"><span data-stu-id="5a459-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
