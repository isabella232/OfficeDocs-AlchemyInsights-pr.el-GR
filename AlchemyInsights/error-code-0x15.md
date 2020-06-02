---
title: Κωδικός σφάλματος 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Εάν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε αναπτύξεις υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), εξετάστε το ενδεχόμενο να ενεργοποιήσετε το ADAL με επεξεργασία του μητρώου.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506846"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="8152d-103">Σφάλμα κατά την ενεργοποίηση του Office 2013 στις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας</span><span class="sxs-lookup"><span data-stu-id="8152d-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="8152d-104">Εάν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε αναπτύξεις υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), εξετάστε το ενδεχόμενο να ενεργοποιήσετε το ADAL με επεξεργασία του μητρώου.</span><span class="sxs-lookup"><span data-stu-id="8152d-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="8152d-105">**Κλειδί μητρώου**</span><span class="sxs-lookup"><span data-stu-id="8152d-105">**Registry key**</span></span>|<span data-ttu-id="8152d-106">**Πληκτρολογήστε**</span><span class="sxs-lookup"><span data-stu-id="8152d-106">**Type**</span></span>|<span data-ttu-id="8152d-107">**Τιμή**</span><span class="sxs-lookup"><span data-stu-id="8152d-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8152d-108">HKEY_CURRENT_USER\Λογισμικό\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="8152d-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="8152d-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="8152d-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="8152d-110">1</span><span class="sxs-lookup"><span data-stu-id="8152d-110">1</span></span>  <br/> |

<span data-ttu-id="8152d-111">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση σύγχρονου ελέγχου ταυτότητας για το Office 2013 σε συσκευές Των Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="8152d-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="8152d-112">Το ADAL είναι ενεργοποιημένο από προεπιλογή στις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις και στο Office 2016.</span><span class="sxs-lookup"><span data-stu-id="8152d-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="8152d-113">Οι υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) είχαν ονομαστεί προηγουμένως υπηρεσίες τερματικού.</span><span class="sxs-lookup"><span data-stu-id="8152d-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  