---
title: Δημόσιος φάκελος με δυνατότητα αποστολής ως αλληλογραφίας στο EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052566"
---
# <a name="sendas-mail-enabled-public-folder"></a>Δημόσιος φάκελος με δυνατότητα αποστολής ως αλληλογραφίας

Το παρακάτω παράδειγμα εκχωρεί δικαιώματα "Αποστολή ως" για τον δημόσιο φάκελο Με δυνατότητα αλληλογραφίας NewPF1 στο χρήστη Jason.

Add-RecipientPermission -Identity "NewPF1" -Trustee "Jason" -AccessRights 'SendAs'

Για λεπτομερείς πληροφορίες σύνταξης και παραμέτρων, ανατρέξτε στο θέμα Εκχώρηση δικαιωμάτων "Αποστολή ως" ή "Αποστολή εκ [μέρους" για δημόσιους φακέλους με δυνατότητα αλληλογραφίας.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)

