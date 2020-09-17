---
title: Αντιστοίχιση βιβλιοθήκης του SharePoint σε μονάδα δίσκου δικτύου
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 9115a3ab8d1234127a95628a9a49679ef06f6d39
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806183"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="deaf0-102">Αντιστοίχιση βιβλιοθήκης του SharePoint σε μονάδα δίσκου δικτύου</span><span class="sxs-lookup"><span data-stu-id="deaf0-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="deaf0-103">Η αντιστοίχιση μιας βιβλιοθήκης ως μονάδας δίσκου δικτύου είναι προσωρινή και υποστηρίζεται μόνο μέσω του Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="deaf0-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="deaf0-104">Πρέπει περιστασιακά να ανοίξετε την τοποθεσία του SharePoint στον Internet Explorer και να επιλέξετε **παραμείνετε συνδεδεμένοι** για να αποτρέψετε τη λήξη της περιόδου λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="deaf0-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="deaf0-105">Αντί για αυτό, [Συγχρονίστε αρχεία του SharePoint με το νέο πρόγραμμα-πελάτη συγχρονισμού του OneDrive, το](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> οποίο παρέχει [αρχεία κατ ' απαίτηση](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="deaf0-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="deaf0-106">Αποκτήστε πρόσβαση σε όλα τα αρχεία σας στο OneDrive χωρίς να χρησιμοποιήσετε τον τοπικό χώρο αποθήκευσης.</span><span class="sxs-lookup"><span data-stu-id="deaf0-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="deaf0-107">Εάν επιλέξετε να αντιστοιχίσετε μια μονάδα δίσκου αντί να [χρησιμοποιήσετε το νέο πρόγραμμα-πελάτη συγχρονισμού του OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), βεβαιωθείτε ότι ακολουθείτε τα βήματα στο παρακάτω άρθρο.</span><span class="sxs-lookup"><span data-stu-id="deaf0-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="deaf0-108">**Τρόπος ρύθμισης παραμέτρων και αντιμετώπισης προβλημάτων αντιστοιχισμένων μονάδων δίσκου δικτύου**</span><span class="sxs-lookup"><span data-stu-id="deaf0-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="deaf0-109">Ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων αντιστοιχισμένων μονάδων δίσκου δικτύου που συνδέονται με το SharePoint Online](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="deaf0-109">See [Troubleshoot mapped network drives that connect to SharePoint Onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>

<span data-ttu-id="deaf0-110">Σημείωση: Εάν χρησιμοποιείτε τον Internet Explorer 10 με Windows 8 ή Windows 7 και δεν **επιτρέπεται η πρόσβαση** ή η **διαδρομή δεν είναι προσβάσιμη** κατά την αντιστοίχιση μιας μονάδας δίσκου, εγκαταστήστε [αυτήν την επείγουσα επιδιόρθωση](https://support.microsoft.com/help/2846960) για να επιλύσετε αυτό το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="deaf0-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
