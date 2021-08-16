---
title: Intune Exchange σύνδεσης εσωτερικής εγκατάστασης
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013964"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange σύνδεσης εσωτερικής εγκατάστασης

Για λεπτομέρειες σχετικά με τη ρύθμιση της γραμμής σύνδεσης μεταξύ του Intune και Exchange που φιλοξενείται στην εσωτερική εγκατάσταση, ανατρέξτε στην παρακάτω τεκμηρίωση:

[Ρύθμιση της γραμμής σύνδεσης εσωτερικής εγκατάστασης του Intune Exchange στο Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Συνήθεις ερωτήσεις:**

Ε: Εμφανίζεται ένα σφάλμα όπως "Η έκδοση Exchange σύνδεσης δεν υποστηρίζεται" όταν επιχειρώ να ρυθμίσω τη Exchange σύνδεσης. Ποια μπορεί να είναι η αιτία;

Α: Ο λογαριασμός που χρησιμοποιείτε διαθέτει κατάλληλη άδεια χρήσης - πρέπει να έχει μια ενεργή άδεια χρήσης του Intune

Ε: Είναι δυνατό να έχετε πολλές Exchange σύνδεσης;

Α: Μπορείτε να ρυθμίσετε μόνο μία Exchange ανά μισθωτή Intune ανά Exchange οργανισμό. Η γραμμή σύνδεσης μπορεί να εγκατασταθεί μόνο σε έναν διακομιστή σε έναν οργανισμό ανταλλαγής διακομιστών πολλών διακομιστών.

Επίσης, δεν μπορείτε να ρυθμίσετε τις παραμέτρους των γραμμών σύνδεσης τόσο για Exchange εσωτερικής εγκατάστασης όσο και Exchange Online έχουν ρυθμιστεί στον ίδιο μισθωτή.

Ε: Μπορεί η γραμμή σύνδεσης να χρησιμοποιήσει έναν πίνακα CAS ως σύνδεση με Exchange;

Α: Ο καθορισμός ενός πίνακα CAS δεν είναι υποστηριζόμενη ρύθμιση παραμέτρων στη ρύθμιση της γραμμής σύνδεσης. Θα πρέπει να καθοριστεί μόνο ένας διακομιστής και θα πρέπει να κωδικοποιηθεί στο αρχείο ρύθμισης παραμέτρων της γραμμής σύνδεσης, το οποίο μπορείτε να βρείτε στο

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Εντοπίστε την ακόλουθη καταχώρηση ```<ExchangeWebServiceURL />``` και αντικαταστήστε τη διεύθυνση URL με το διακομιστή exchange.

**Παράδειγμα:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Ανατρέξτε στην παρακάτω τεκμηρίωση για πρόσθετη αντιμετώπιση προβλημάτων: Αντιμετώπιση προβλημάτων στη γραμμή σύνδεσης εσωτερικής [εγκατάστασης του Intune Exchange σύνδεσης](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Ενεργοποίηση λεπτομερής καταγραφής για τη Exchange σύνδεσης**

1. Ανοίξτε το αρχείο Exchange ανίχνευσης σύνδεσης για επεξεργασία.  
Το αρχείο βρίσκεται στη θέση : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Παράδειγμα:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Εντοπίστε την TraceSourceLine με το ακόλουθο κλειδί: OnPremisesExchangeConnectorService  
  
3. Αλλαγή της τιμής κόμβου SourceLevel από "Πληροφορίες activityTracing" (προεπιλογή) σε "Λεπτομερής activityTracing"  

**Παράδειγμα:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Επανεκκίνηση της Microsoft Intune Exchange Υπηρεσίας  
5. Πλήρης συγχρονισμός στην πύλη Intune μέχρι να ολοκληρωθεί και, στη συνέχεια, αλλάξτε ξανά την XML σε "Πληροφορίες ActivityTracing" και επανεκκινήστε την Microsoft Intune Exchange υπηρεσίας.  
6. Η θέση των αρχείων καταγραφής είναι: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`