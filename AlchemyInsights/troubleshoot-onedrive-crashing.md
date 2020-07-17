---
title: Αντιμετώπιση προβλημάτων σφαλμάτων στο OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748919"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="bfa3f-102">Αντιμετώπιση προβλημάτων σφαλμάτων στο OneDrive</span><span class="sxs-lookup"><span data-stu-id="bfa3f-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="bfa3f-103">Εάν το OneDrive διακοπεί επανειλημμένα, δοκιμάστε τα εξής βήματα αντιμετώπισης προβλημάτων:</span><span class="sxs-lookup"><span data-stu-id="bfa3f-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="bfa3f-104">**Βεβαιωθείτε ότι τα κλειδιά μητρώου δεν έχουν οριστεί:**</span><span class="sxs-lookup"><span data-stu-id="bfa3f-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="bfa3f-105">Χρήση του Επεξεργαστή Μητρώου( Registry Editor", μεταβείτε στην HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="bfa3f-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="bfa3f-106">Εάν υπάρχει το DisableFileSyncNGSC και οριστεί σε 1, ανοίξτε το κλειδί και αλλάξτε την τιμή σε 0.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="bfa3f-107">Μη αυτόματη εκκίνηση του OneDrive μεταβαίνοντας στην Έναρξη</span><span class="sxs-lookup"><span data-stu-id="bfa3f-107">Manually launch OneDrive by going to Start</span></span> ![Πάτημα του πλήκτρου των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="bfa3f-109">, πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="bfa3f-110">**Επαναφορά του OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="bfa3f-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="bfa3f-111">Σημειώσεις:</span><span class="sxs-lookup"><span data-stu-id="bfa3f-111">Notes:</span></span>

- <span data-ttu-id="bfa3f-112">Η επαναφορά του OneDrive αποσυνδέει όλες τις υπάρχουσες συνδέσεις συγχρονισμού (συμπεριλαμβανομένου του προσωπικού σας OneDrive, αν έχει ρυθμιστεί).</span><span class="sxs-lookup"><span data-stu-id="bfa3f-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="bfa3f-113">Δεν θα χάσετε αρχεία ή δεδομένα επαναφέροντας το OneDrive στον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="bfa3f-114">**Για να επαναφέρετε το OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="bfa3f-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="bfa3f-115">Ανοίξτε ένα παράθυρο διαλόγου Εκτέλεση πατώντας το πλήκτρο των Windows και το πλήκτρο R.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="bfa3f-116">Πληκτρολογήστε %localappdata%\Microsoft\OneDrive\onedrive.exe /reset και πατήστε OK.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="bfa3f-117">Ένα παράθυρο εντολών μπορεί να εμφανιστεί για λίγο.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="bfa3f-118">Μη αυτόματη εκκίνηση του OneDrive μεταβαίνοντας στην Έναρξη</span><span class="sxs-lookup"><span data-stu-id="bfa3f-118">Manually launch OneDrive by going to Start</span></span> ![Πάτημα του πλήκτρου των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="bfa3f-120">, πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="bfa3f-121">Σημειώσεις:</span><span class="sxs-lookup"><span data-stu-id="bfa3f-121">Notes:</span></span>

- <span data-ttu-id="bfa3f-122">Εάν είχατε επιλέξει να συγχρονίσετε μόνο ορισμένους φακέλους πριν από την επαναφορά, θα πρέπει να το κάνετε ξανά μόλις ολοκληρωθεί ο συγχρονισμός.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="bfa3f-123">Διαβάστε την ενότητα [Επιλέξτε τους φακέλους του OneDrive που θα συγχρονιστούν με τον υπολογιστή σας](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)για   περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="bfa3f-124">Θα χρειαστεί να το ολοκληρώσετε αυτό για το προσωπικό σας OneDrive και το OneDrive για επιχειρήσεις.</span><span class="sxs-lookup"><span data-stu-id="bfa3f-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>