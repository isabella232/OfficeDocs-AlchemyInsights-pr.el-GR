---
title: Προβλήματα κατά την εγκατάσταση του Microsoft Defender σε Mac ή Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713543"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="aa535-102">Προβλήματα κατά την εγκατάσταση του Microsoft Defender σε Mac ή Linux</span><span class="sxs-lookup"><span data-stu-id="aa535-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="aa535-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="aa535-103">**Mac**</span></span>

- <span data-ttu-id="aa535-104">Βεβαιωθείτε ότι πληρούνται οι απαιτήσεις συστήματος πριν από την εγκατάσταση του Microsoft Defender ATP για Mac.</span><span class="sxs-lookup"><span data-stu-id="aa535-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="aa535-105">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Πώς να εγκαταστήσετε το Microsoft Defender ATP για Mac".](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="aa535-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="aa535-106">Εξετάστε τις πληροφορίες στο αρχείο: "/Βιβλιοθήκη/Αρχεία καταγραφής/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="aa535-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="aa535-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="aa535-107">**Linux**</span></span>

- <span data-ttu-id="aa535-108">Βεβαιωθείτε ότι πληρούνται οι απαιτήσεις συστήματος πριν από την εγκατάσταση του Microsoft Defender ATP για Linux.</span><span class="sxs-lookup"><span data-stu-id="aa535-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="aa535-109">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Πώς να εγκαταστήσετε το Microsoft Defender ATP για Linux".](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="aa535-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="aa535-110">Για να επαληθεύσετε ότι εκτελείται η υπηρεσία MDATP, ανατρέξτε στο θέμα ["Η εγκατάσταση απέτυχε".](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="aa535-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="aa535-111">Για να αντιμετωπίσετε και να επιλύσετε προβλήματα εάν η υπηρεσία δεν εκτελείται, ανατρέξτε στα βήματα αντιμετώπισης προβλημάτων εάν δεν [εκτελείται η υπηρεσία mdatp.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="aa535-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="aa535-112">Για τα βήματα για να ελέγξετε τη ρύθμιση παραμέτρων του προγράμματος-πελάτη, το οποίο επαληθεύει την κατάσταση του προϊόντος και για να εκτελέσετε έναν έλεγχο εντοπισμού στο αρχείο κειμένου EICAR, ανατρέξτε στο θέμα "Ρύθμιση παραμέτρων [προγράμματος-πελάτη".](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="aa535-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="aa535-113">**Σημείωση** Για μια λίστα των υποστηριζόμενων συστημάτων αρχείων για δραστηριότητα κατά την πρόσβαση, ανατρέξτε [στο θέμα Microsoft Defender ATP για Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="aa535-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>