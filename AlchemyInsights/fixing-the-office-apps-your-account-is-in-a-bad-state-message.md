---
title: Καθορισμός των εφαρμογών του Office ο λογαριασμός σας βρίσκεται σε μήνυμα κακής κατάστασης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969473"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="fd56b-102">Επιδιόρθωση των εφαρμογών του Office "ο λογαριασμός σας είναι σε κακή κατάσταση" σφάλμα</span><span class="sxs-lookup"><span data-stu-id="fd56b-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="fd56b-103">Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τις ακόλουθες επιλογές στον υπολογιστή που επηρεάζεται:</span><span class="sxs-lookup"><span data-stu-id="fd56b-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="fd56b-104">Ανοίξτε μια εφαρμογή του Office, επιλέξτε υπογραφή**λογαριασμού** >  **αρχείου** > **από όλους τους λογαριασμούς**.</span><span class="sxs-lookup"><span data-stu-id="fd56b-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="fd56b-105">Συνδεθείτε ξανά χρησιμοποιώντας ένα λογαριασμό χρήστη με έγκυρη άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="fd56b-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="fd56b-106">Για λεπτομερείς πληροφορίες, ανατρέξτε [στο λογαριασμό λογαριασμοί στο Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="fd56b-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="fd56b-107">[Καταργήστε τις πιστοποιήσεις του Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.</span><span class="sxs-lookup"><span data-stu-id="fd56b-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="fd56b-108">**Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16,0.</span><span class="sxs-lookup"><span data-stu-id="fd56b-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="fd56b-109">Για παράδειγμα, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="fd56b-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="fd56b-110">Στον υπολογιστή που επηρεάζεται, ορίστε το EnableADAL = 0, ακολουθώντας τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="fd56b-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="fd56b-111">Κάντε δεξιό κλικ στο κουμπί των Windows και επιλέξτε **Εκτέλεση**.</span><span class="sxs-lookup"><span data-stu-id="fd56b-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="fd56b-112">Με το **Άνοιγμα** πλαίσιο, πληκτρολογήστε **regedit**, και στη συνέχεια επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="fd56b-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="fd56b-113">Επιλέξτε **Ναι** όταν σας ζητηθεί να επιτρέψετε στον επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.</span><span class="sxs-lookup"><span data-stu-id="fd56b-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="fd56b-114">Στον επεξεργαστή μητρώου, προσθέστε μια τιμή DWORD του EnableADAL με μια ρύθμιση 0 κάτω από HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="fd56b-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="fd56b-115">Εάν το σφάλμα παρουσιάζεται κατά τη σύνδεση με το Office 365 χρησιμοποιώντας το Office 2013, [ενεργοποιήστε τον σύγχρονο έλεγχο ταυτότητας](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) για το πρόγραμμα-πελάτη του Office.</span><span class="sxs-lookup"><span data-stu-id="fd56b-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="fd56b-116">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Τρόπος αντιμετώπισης προβλημάτων εφαρμογών που δεν είναι προγράμματα περιήγησης που δεν είναι δυνατό να εισέλθετε στο Office 365, Azure ή Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="fd56b-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

