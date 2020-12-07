---
title: Τι πρέπει να κάνετε εάν οι δυνατότητες του Azure δεν λειτουργούν σωστά στο Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583462"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="e0f41-102">Τι πρέπει να κάνετε εάν οι δυνατότητες του Azure δεν λειτουργούν σωστά στο Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e0f41-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="e0f41-103">Το Microsoft Edge έχει [γνωστά προβλήματα](https://go.microsoft.com/fwlink/?linkid=2140608) που σχετίζονται με τις ζώνες ασφαλείας και μπορεί να επηρεάσει τον τρόπο με τον οποίο οι χρήστες του Azure συνδέονται στο κέντρο διαχείρισης των Windows.</span><span class="sxs-lookup"><span data-stu-id="e0f41-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="e0f41-104">Εάν αντιμετωπίζετε προβλήματα με τη χρήση των δυνατοτήτων του Azure με το Microsoft Edge, δοκιμάστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="e0f41-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="e0f41-105">Στο μενού **Έναρξη** , κάντε αναζήτηση για **Επιλογές Internet** και επιλέξτε την.</span><span class="sxs-lookup"><span data-stu-id="e0f41-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="e0f41-106">Στο παράθυρο διαλόγου **Ιδιότητες Internet** , μεταβείτε στην καρτέλα **ασφάλεια** .</span><span class="sxs-lookup"><span data-stu-id="e0f41-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="e0f41-107">Επιλέξτε τη ζώνη **αξιόπιστων τοποθεσιών** και, στη συνέχεια, επιλέξτε το κουμπί **τοποθεσίες** .</span><span class="sxs-lookup"><span data-stu-id="e0f41-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="e0f41-108">Στο παράθυρο διαλόγου **Αξιόπιστες τοποθεσίες** , προσθέστε τη διεύθυνση URL της πύλης σας καθώς [https://login.microsoftonline.com](https://login.microsoftonline.com) και και [https://login.live.com](https://login.live.com) , στη συνέχεια, επιλέξτε **Κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="e0f41-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="e0f41-109">Στο παράθυρο διαλόγου **Ιδιότητες Internet** , μεταβείτε στην καρτέλα **προστασία προσωπικών δεδομένων** .</span><span class="sxs-lookup"><span data-stu-id="e0f41-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="e0f41-110">Στην ενότητα **Αποκλεισμός αναδυόμενων** παραθύρων, επιλέξτε **Ρυθμίσεις**.</span><span class="sxs-lookup"><span data-stu-id="e0f41-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="e0f41-111">Στο παράθυρο διαλόγου που ανοίγει, προσθέστε τη διεύθυνση URL της πύλης σας καθώς [https://login.microsoftonline.com](https://login.microsoftonline.com) και και [https://login.live.com](https://login.live.com) , στη συνέχεια, επιλέξτε **Κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="e0f41-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
