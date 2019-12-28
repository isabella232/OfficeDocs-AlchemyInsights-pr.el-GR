---
title: Αποστολή προσαρμοσμένων ειδοποιήσεων με το Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886857"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="27280-102">Πώς να στείλετε προσαρμοσμένες ειδοποιήσεις στους χρήστες των διαχειριζόμενων συσκευών iOS και Android</span><span class="sxs-lookup"><span data-stu-id="27280-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="27280-103">Οι προσαρμοσμένες ειδοποιήσεις για το Intune υποβάλλονται σε επεξεργασία από την εφαρμογή πύλης εταιρείας στη συσκευή ενός χρήστη.</span><span class="sxs-lookup"><span data-stu-id="27280-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="27280-104">Στη συνέχεια, η εφαρμογή δημιουργεί την ειδοποίηση push σε αυτήν τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="27280-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="27280-105">Τα παρακάτω είναι προαπαιτούμενα συσκευών για την υποστήριξη παραλαβής προσαρμοσμένων ειδοποιήσεων και για την εφαρμογή στη συνέχεια να δημιουργήσετε την ειδοποίηση push:</span><span class="sxs-lookup"><span data-stu-id="27280-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="27280-106">Η συσκευή πρέπει να έχει εγκατεστημένη την εφαρμογή πύλης εταιρείας.</span><span class="sxs-lookup"><span data-stu-id="27280-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="27280-107">Η συσκευή πρέπει να επιτρέπει στην εφαρμογή πύλης εταιρείας να αποστέλλει ειδοποιήσεις push.</span><span class="sxs-lookup"><span data-stu-id="27280-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="27280-108">Όταν η εφαρμογή έχει εγκατασταθεί ή ενημερωθεί, θα ζητήσει από το χρήστη να επιτρέψει τις ειδοποιήσεις.</span><span class="sxs-lookup"><span data-stu-id="27280-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="27280-109">Οι συσκευές Android πρέπει να έχουν εγκατεστημένες τις υπηρεσίες Google Play.</span><span class="sxs-lookup"><span data-stu-id="27280-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="27280-110">Η συσκευή πρέπει να εγγραφεί στο Intune.</span><span class="sxs-lookup"><span data-stu-id="27280-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="27280-111">Για περισσότερες πληροφορίες, όπως πώς να στείλετε ένα μήνυμα, ανατρέξτε στην [τεκμηρίωση της δυνατότητας](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="27280-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
