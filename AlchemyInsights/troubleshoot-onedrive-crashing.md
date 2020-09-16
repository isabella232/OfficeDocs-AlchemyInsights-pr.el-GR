---
title: Αντιμετώπιση προβλημάτων σφαλμάτων του OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664998"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="c4208-102">Αντιμετώπιση προβλημάτων σφαλμάτων του OneDrive</span><span class="sxs-lookup"><span data-stu-id="c4208-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="c4208-103">Εάν το OneDrive παρουσιάσει επανειλημμένα σφάλμα, δοκιμάστε αυτά τα βήματα αντιμετώπισης προβλημάτων:</span><span class="sxs-lookup"><span data-stu-id="c4208-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="c4208-104">**Βεβαιωθείτε ότι δεν έχουν καθοριστεί τα κλειδιά μητρώου:**</span><span class="sxs-lookup"><span data-stu-id="c4208-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="c4208-105">Χρησιμοποιώντας τον επεξεργαστή μητρώου, μεταβείτε στο HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="c4208-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="c4208-106">Εάν το DisableFileSyncNGSC είναι παρόν και ορίστε το 1, ανοίξτε το κλειδί και αλλάξτε την τιμή σε 0.</span><span class="sxs-lookup"><span data-stu-id="c4208-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="c4208-107">Μη αυτόματη εκκίνηση του OneDrive με τη μετάβαση στην έναρξη</span><span class="sxs-lookup"><span data-stu-id="c4208-107">Manually launch OneDrive by going to Start</span></span> ![Πατήστε το πλήκτρο των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="c4208-109">, πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c4208-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="c4208-110">**Επαναφορά του OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="c4208-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="c4208-111">Σημειώσεις</span><span class="sxs-lookup"><span data-stu-id="c4208-111">Notes:</span></span>

- <span data-ttu-id="c4208-112">Η επαναφορά του OneDrive αποσυνδέει όλες τις υπάρχουσες συνδέσεις συγχρονισμού (συμπεριλαμβανομένου του προσωπικού σας OneDrive, εάν έχει ρυθμιστεί).</span><span class="sxs-lookup"><span data-stu-id="c4208-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="c4208-113">Δεν θα χάσετε αρχεία ή δεδομένα με την επαναφορά του OneDrive στον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="c4208-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="c4208-114">**Για να επαναφέρετε το OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="c4208-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="c4208-115">Ανοίξτε ένα παράθυρο διαλόγου "εκτέλεση" πατώντας το πλήκτρο Windows και το πλήκτρο R.</span><span class="sxs-lookup"><span data-stu-id="c4208-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="c4208-116">Πληκτρολογήστε% localappdata% \Microsoft\OneDrive\onedrive.exe/reset και πατήστε OK.</span><span class="sxs-lookup"><span data-stu-id="c4208-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="c4208-117">Ένα παράθυρο εντολών μπορεί να εμφανιστεί σύντομα.</span><span class="sxs-lookup"><span data-stu-id="c4208-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="c4208-118">Μη αυτόματη εκκίνηση του OneDrive με τη μετάβαση στην έναρξη</span><span class="sxs-lookup"><span data-stu-id="c4208-118">Manually launch OneDrive by going to Start</span></span> ![Πατήστε το πλήκτρο των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="c4208-120">, πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c4208-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="c4208-121">Σημειώσεις</span><span class="sxs-lookup"><span data-stu-id="c4208-121">Notes:</span></span>

- <span data-ttu-id="c4208-122">Εάν είχατε επιλέξει να συγχρονίσετε μόνο ορισμένους φακέλους πριν από την επαναφορά, θα πρέπει να το κάνετε ξανά όταν ολοκληρωθεί ο συγχρονισμός.</span><span class="sxs-lookup"><span data-stu-id="c4208-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="c4208-123">Διαβάστε το στοιχείο [επιλογή των φακέλων του OneDrive για συγχρονισμό με τον υπολογιστή σας](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="c4208-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="c4208-124">Θα πρέπει να το συμπληρώσετε αυτό για το προσωπικό σας OneDrive και το OneDrive για επιχείρηση.</span><span class="sxs-lookup"><span data-stu-id="c4208-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>