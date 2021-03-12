---
title: Προβλήματα σύνδεσης σε εφαρμογές του Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709106"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="f93a0-102">Επιδιόρθωση των εφαρμογών του Microsoft 365 "Η λειτουργική μονάδα αξιόπιστης πλατφόρμας του υπολογιστή σας δεν λειτουργεί σωστά"</span><span class="sxs-lookup"><span data-stu-id="f93a0-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="f93a0-103">Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="f93a0-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="f93a0-104">Εγκαταστήστε τις πιο πρόσφατες ενημερώσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και [το Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="f93a0-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="f93a0-105">[Εκκαθαρίσω τα διαπιστευτήρια του Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.</span><span class="sxs-lookup"><span data-stu-id="f93a0-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="f93a0-106">**Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0.</span><span class="sxs-lookup"><span data-stu-id="f93a0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="f93a0-107">(Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="f93a0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="f93a0-108">Δοκιμάστε τη διαδικασία [ανάκτησης χρηστών για](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) να διορθώσετε αποτυχίες Λειτουργικής μονάδας αξιόπιστης πλατφόρμας (TPM).</span><span class="sxs-lookup"><span data-stu-id="f93a0-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="f93a0-109">Ορίστε το EnableADAL = 0 ακολουθώντας τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="f93a0-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="f93a0-110">Κάντε δεξί κλικ στο κουμπί "Έναρξη" των Windows, επιλέξτε **"Εκτέλεση",** **πληκτρολογήστε regedit** και, στη συνέχεια, επιλέξτε **OK.**</span><span class="sxs-lookup"><span data-stu-id="f93a0-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="f93a0-111">Επιλέξτε **"Ναι"** για να επιτρέψετε στον Επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.</span><span class="sxs-lookup"><span data-stu-id="f93a0-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="f93a0-112">Στον Επεξεργαστή Μητρώου, προσθέστε μια τιμή DWORD της **EnableADAL** με ρύθμιση **0 στην** περιοχή HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="f93a0-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="f93a0-113">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα "Προβλήματα σύνδεσης κατά την είσοδο μετά την ενημέρωση στο [Office 2016, έκδοση 16.0.7967 στα Windows 10".](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="f93a0-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>