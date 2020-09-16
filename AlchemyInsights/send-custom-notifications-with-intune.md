---
title: Αποστολή προσαρμοσμένων ειδοποιήσεων με το Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720646"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="46409-102">Πώς μπορείτε να στείλετε προσαρμοσμένες ειδοποιήσεις στους χρήστες διαχειριζόμενων συσκευών iOS και Android</span><span class="sxs-lookup"><span data-stu-id="46409-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="46409-103">Οι προσαρμοσμένες ειδοποιήσεις για το Intune υποβάλλονται σε επεξεργασία από την εφαρμογή εταιρεία πύλης στη συσκευή ενός χρήστη.</span><span class="sxs-lookup"><span data-stu-id="46409-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="46409-104">Στη συνέχεια, η εφαρμογή δημιουργεί την ειδοποίηση push σε αυτήν τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="46409-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="46409-105">Ακολουθούν οι προϋποθέσεις συσκευής για την υποστήριξη της παραλαβής προσαρμοσμένων ειδοποιήσεων και, στη συνέχεια, η εφαρμογή θα δημιουργήσει την ειδοποίηση push:</span><span class="sxs-lookup"><span data-stu-id="46409-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="46409-106">Η συσκευή πρέπει να έχει εγκατεστημένη την εφαρμογή εταιρεία πύλης.</span><span class="sxs-lookup"><span data-stu-id="46409-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="46409-107">Η συσκευή πρέπει να επιτρέπει στην εφαρμογή πύλης εταιρείας να στέλνει ειδοποιήσεις push.</span><span class="sxs-lookup"><span data-stu-id="46409-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="46409-108">Κατά την εγκατάσταση ή την ενημέρωση της εφαρμογής, θα ζητηθεί από το χρήστη να επιτρέψει τις ειδοποιήσεις.</span><span class="sxs-lookup"><span data-stu-id="46409-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="46409-109">Οι συσκευές Android πρέπει να έχουν εγκατεστημένο το Google Play Services.</span><span class="sxs-lookup"><span data-stu-id="46409-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="46409-110">Η συσκευή πρέπει να είναι εγγεγραμμένη με το Intune.</span><span class="sxs-lookup"><span data-stu-id="46409-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="46409-111">Για περισσότερες πληροφορίες, όπως πώς μπορείτε να στείλετε ένα μήνυμα, ανατρέξτε στην [τεκμηρίωση της δυνατότητας](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="46409-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
