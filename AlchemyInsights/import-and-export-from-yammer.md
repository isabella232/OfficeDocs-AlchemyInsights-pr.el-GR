---
title: Εισαγωγή και εξαγωγή από Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036126"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="d8308-102">Εισαγωγή και εξαγωγή από Yammer</span><span class="sxs-lookup"><span data-stu-id="d8308-102">Import and export from Yammer</span></span>

<span data-ttu-id="d8308-103">**Εισαγωγή**</span><span class="sxs-lookup"><span data-stu-id="d8308-103">**Import**</span></span>

<span data-ttu-id="d8308-104">Οι επιλογές εισαγωγής χρήστη διαφέρουν ανάλογα με το εάν το Yammer σας βρίσκεται σε [εγγενή λειτουργία για το Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ή όχι.</span><span class="sxs-lookup"><span data-stu-id="d8308-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="d8308-105">**Μη εγγενής λειτουργία:** Οι χρήστες μπορούν να εισαχθούν σε ομάδες χρησιμοποιώντας την επιλογή ["Προσθήκη](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) από βιβλίο διευθύνσεων" (όριο σε 100 χρήστες) στις ρυθμίσεις ομάδας ή στο δίκτυο χρησιμοποιώντας [τη Μαζική ενημέρωση](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) μέσα από το διαχειριστή δικτύου.</span><span class="sxs-lookup"><span data-stu-id="d8308-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="d8308-106">**Εγγενής λειτουργία:** Οι λειτουργίες ιδιότητας μέλους ομάδας και μέλους δικτύου θα πρέπει να εκτελούνται από την πύλη διαχείρισης [Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/add-users)την πύλη [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ή χρησιμοποιώντας μια άλλη επιλογή Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d8308-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="d8308-107">Τα δίκτυα στην εγγενή λειτουργία δεν έχουν πλέον πρόσβαση στη Μαζική ενημέρωση και σε άλλες δυνατότητες παλαιού τύπου.</span><span class="sxs-lookup"><span data-stu-id="d8308-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d8308-108">Yammer υποστηρίζεται η εισαγωγή περιεχομένου από το διαχειριστή δικτύου, ακόμα και όταν η δυνατότητα εξαγωγής δεδομένων χρησιμοποιήθηκε σε άλλο δίκτυο.</span><span class="sxs-lookup"><span data-stu-id="d8308-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="d8308-109">Το περιεχόμενο μπορεί να δημοσιευτεί εκ Yammer λύσεων συνεργατών.</span><span class="sxs-lookup"><span data-stu-id="d8308-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="d8308-110">**Εξαγωγή**</span><span class="sxs-lookup"><span data-stu-id="d8308-110">**Export**</span></span>

<span data-ttu-id="d8308-111">[Η εξαγωγή δεδομένων δικτύου μέσα από το διαχειριστή](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) δικτύου επιτρέπει την εξαγωγή περιεχομένου από Yammer δίκτυα, συμπεριλαμβανομένων των μηνυμάτων και των αρχείων.</span><span class="sxs-lookup"><span data-stu-id="d8308-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="d8308-112">Τα συνημμένα μπορεί να είναι εξαιρετικά μεγάλα και θα προκαλέσουν την ολοκλήρωση των εξαγωγών.</span><span class="sxs-lookup"><span data-stu-id="d8308-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="d8308-113">Συνιστάται η εξαγωγή ενεργών δικτύων με χρήση του [API εξαγωγής δεδομένων](https://developer.yammer.com/docs/data-export-api) σε μπλοκ ανά ημέρα ή εβδομάδα.</span><span class="sxs-lookup"><span data-stu-id="d8308-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="d8308-114">Η Υποστήριξη της Microsoft δεν παρέχει προσαρμοσμένες δέσμες ενεργειών για το σκοπό αυτό.</span><span class="sxs-lookup"><span data-stu-id="d8308-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="d8308-115">Μια ξεχωριστή [εξαγωγή ΓΚΠΔ](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) υπάρχει για την εξαγωγή περιεχομένου για έναν μεμονωμένο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="d8308-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>