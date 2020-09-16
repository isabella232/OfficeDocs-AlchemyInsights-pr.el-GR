---
title: Χρήση προφίλ ηλεκτρονικού ταχυδρομείου με το Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653288"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="291b5-102">Χρήση προφίλ ηλεκτρονικού ταχυδρομείου με το Intune</span><span class="sxs-lookup"><span data-stu-id="291b5-102">Using email profiles with Intune</span></span>

<span data-ttu-id="291b5-103">Το Intune μπορεί να χρησιμοποιηθεί για τη δημιουργία και την ανάπτυξη προφίλ ηλεκτρονικού ταχυδρομείου για το τοπικό (ενσωματωμένο) πρόγραμμα-πελάτη ηλεκτρονικού ταχυδρομείου σε πολλές πλατφόρμες συσκευών.</span><span class="sxs-lookup"><span data-stu-id="291b5-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="291b5-104">Για πληροφορίες σχετικά με ορισμένους από τους περιορισμούς που σχετίζονται με τα προφίλ ηλεκτρονικού ταχυδρομείου, συμπεριλαμβανομένου του τρόπου χειρισμού της παρουσίας των υπαρχόντων προφίλ και του τρόπου κατάργησης των προφίλ ηλεκτρονικού ταχυδρομείου, ανατρέξτε [στο θέμα Προσθήκη ρυθμίσεων ηλεκτρονικού ταχυδρομείου σε συσκευές με χρήση του Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="291b5-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="291b5-105">Για περισσότερες πληροφορίες σχετικά με τον τρόπο δημιουργίας προφίλ ηλεκτρονικού ταχυδρομείου για κάθε πλατφόρμα συσκευής, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="291b5-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="291b5-106">Ρυθμίσεις συσκευής Android για τη ρύθμιση παραμέτρων ηλεκτρονικού ταχυδρομείου, ελέγχου ταυτότητας και συγχρονισμού στο Intune</span><span class="sxs-lookup"><span data-stu-id="291b5-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="291b5-107">Προσθήκη ρυθμίσεων ηλεκτρονικού ταχυδρομείου για συσκευές iOS και iPadOS στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="291b5-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="291b5-108">Ρυθμίσεις προφίλ ηλεκτρονικού ταχυδρομείου στο Microsoft Intune για συσκευές που εκτελούν Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="291b5-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="291b5-109">Ρυθμίσεις προφίλ ηλεκτρονικού ταχυδρομείου για συσκευές που εκτελούν Windows 10 στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="291b5-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="291b5-110">**Κοινό πρόβλημα συγχρονισμού**</span><span class="sxs-lookup"><span data-stu-id="291b5-110">**Common syncing issue**</span></span>

<span data-ttu-id="291b5-111">**Ένα προφίλ ηλεκτρονικού ταχυδρομείου του KNOX στο Android αποτρέπει τις επαφές, το ημερολόγιο και τις εργασίες των χρηστών να συγχρονίζονται με συσκευές χρηστών.**</span><span class="sxs-lookup"><span data-stu-id="291b5-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="291b5-112">Το προφίλ ηλεκτρονικού ταχυδρομείου του KNOX στο Android KNOX προσφέρει στο διαχειριστή τη δυνατότητα να αποφασίζει για τους τύπους περιεχομένου που θα συγχρονίζονται με τη συσκευή, ορίζοντας τον καθένα σε ενεργοποιημένο.</span><span class="sxs-lookup"><span data-stu-id="291b5-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="291b5-113">Εάν η ρύθμιση για οποιονδήποτε από τους τύπους περιεχομένου έχει οριστεί σε **μη ρυθμισμένες παραμέτρους** (προεπιλογή), αυτός ο τύπος περιεχομένου δεν θα συγχρονιστεί αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="291b5-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="291b5-114">Ένας χρήστης μπορεί να ενεργοποιήσει τον τύπο περιεχομένου που θέλει απευθείας στη συσκευή με μη αυτόματο τρόπο, αλλά αυτή η ρύθμιση παραμέτρων αντιγράφεται από τη ρύθμιση πολιτικής του Intune και ο συγχρονισμός σταματά για αυτόν τον τύπο περιεχομένου.</span><span class="sxs-lookup"><span data-stu-id="291b5-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

