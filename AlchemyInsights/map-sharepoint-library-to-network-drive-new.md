---
title: Αντιστοιχίστε μια βιβλιοθήκη του SharePoint σε μια μονάδα δίσκου δικτύου
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: a545c2d9a395893bb089e1647944e9250e6d8df6
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802930"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="a493c-102">Αντιστοιχίστε μια βιβλιοθήκη του SharePoint σε μια μονάδα δίσκου δικτύου</span><span class="sxs-lookup"><span data-stu-id="a493c-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="a493c-103">Αντιστοίχιση μιας βιβλιοθήκης ως μια μονάδα δίσκου δικτύου είναι προσωρινή και υποστηρίζεται μόνο μέσω του Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="a493c-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="a493c-104">Περιστασιακά πρέπει να ανοίξετε την τοποθεσία SharePoint στον Internet Explorer και επιλέξτε " **Διατήρηση της σύνδεσης** " για να αποτρέψετε τη λήξη της περιόδου λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="a493c-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="a493c-105">Αντί για αυτό, [συγχρονισμό αρχείων του SharePoint με το νέο πελάτη συγχρονισμού OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> που παρέχει [Τα αρχεία On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="a493c-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="a493c-106">Πρόσβαση σε όλα τα αρχεία σας στο OneDrive χωρίς χρησιμοποιώντας τοπικό αποθηκευτικό χώρο.</span><span class="sxs-lookup"><span data-stu-id="a493c-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="a493c-107">Εάν θέλετε να αντιστοιχίσετε μια μονάδα δίσκου, αντί να [χρησιμοποιήσετε τον υπολογιστή-πελάτη συγχρονισμού νέα OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), βεβαιωθείτε ότι ακολουθείτε τα βήματα στο παρακάτω άρθρο.</span><span class="sxs-lookup"><span data-stu-id="a493c-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="a493c-108">**Τρόπος ρύθμισης παραμέτρων και αντιμετώπισης προβλημάτων αντιστοιχισμένες μονάδες δίσκων δικτύου**</span><span class="sxs-lookup"><span data-stu-id="a493c-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="a493c-109">Ανατρέξτε στην ενότητα [ρύθμισης παραμέτρων και αντιμετώπισης προβλημάτων αντιστοιχισμένες μονάδες δίσκων δικτύου](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="a493c-109">See [Configure and to troubleshoot mapped network drives](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

<span data-ttu-id="a493c-110">ΣΗΜΕΊΩΣΗ: Εάν χρησιμοποιείτε Internet Explorer 10 με Windows 8 ή Windows 7, και εμφανίζεται **η πρόσβαση** ή **η διαδρομή δεν είναι δεν είναι δυνατή η πρόσβαση** κατά την αντιστοίχιση μιας μονάδας δίσκου, να εγκαταστήσετε [αυτήν την επείγουσα επιδιόρθωση](https://support.microsoft.com/help/2846960) για να επιλύσετε αυτό το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="a493c-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
