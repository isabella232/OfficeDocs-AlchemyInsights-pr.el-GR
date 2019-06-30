---
title: 1048 5.7.750 υπηρεσία δεν είναι διαθέσιμη. Υπολογιστής-πελάτης που στέλνετε από τομείς που δεν έχουν καταχωρηθεί
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: b94fcc697bb7ac065cef57f3e3eb0b515c3094a0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35352853"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="e9b2f-103">5.7.750 προγράμματος-πελάτη αποκλείστηκε από την αποστολή από μη καταχωρημένο τομέα</span><span class="sxs-lookup"><span data-stu-id="e9b2f-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="e9b2f-104">Το σφάλμα παρουσιάζεται όταν ένα μεγάλο όγκο των μηνυμάτων που αποστέλλονται από τομείς που δεν έχουν αποδοθεί στο Office 365 (προστεθεί ως αποδεκτή τομείς και επικύρωση).</span><span class="sxs-lookup"><span data-stu-id="e9b2f-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="e9b2f-105">Για να αποφύγετε αυτό το σφάλμα, μπορείτε να χρησιμοποιήσετε μια σύνδεση ροή αλληλογραφίας που βασίζεται σε πιστοποιητικό όταν το πιστοποιητικό τομέας είναι ένας τομέας που παρασχέθηκε ή να παράσχετε σε όλους τους τομείς αποστολής.</span><span class="sxs-lookup"><span data-stu-id="e9b2f-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
