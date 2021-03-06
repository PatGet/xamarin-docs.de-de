---
title: 'Xamarin.Essentials: e-Mail-Adresse'
description: Die E-Mail-Klasse in Xamarin.Essentials ermöglicht eine Anwendung, um die Standard-e-Mail-Anwendung mit einer angegebenen Informationen, einschließlich Betreff, Nachrichtentext und Empfänger (TO, CC, BCC) zu öffnen.
ms.assetid: 5FBB6FF0-0E7B-4C29-8F06-91642AF12629
author: jamesmontemagno
ms.author: jamont
ms.date: 05/04/2018
ms.openlocfilehash: f113cebfebf4238fd4b75ad8ab248e2abf61efea
ms.sourcegitcommit: 51c274f37369d8965b68ff587e1c2d9865f85da7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/30/2018
ms.locfileid: "39353905"
---
# <a name="xamarinessentials-email"></a>Xamarin.Essentials: e-Mail-Adresse

![Vorabversionen von NuGet](~/media/shared/pre-release.png)

Die **-e-Mail** Klasse ermöglicht einer Anwendung, die Standard-e-Mail-Anwendung mit einer angegebenen Informationen, einschließlich Betreff, Nachrichtentext und Empfänger (TO, CC, BCC) zu öffnen.

## <a name="using-email"></a>Mit e-Mail-Adresse

Fügen Sie einen Verweis auf Xamarin.Essentials in Ihrer Klasse hinzu:

```csharp
using Xamarin.Essentials;
```

Die e-Mail-Funktion erfolgt durch Aufrufen der `ComposeAsync` Methode eine `EmailMessage` , Informationen über die e-Mail-Adresse enthält:

```csharp
public class EmailTest
{
    public async Task SendEmail(string subject, string body, List<string> recipients)
    {
        try
        {
            var message = new EmailMessage
            {
                Subject = subject,
                Body = body,
                To = recipients,
                //Cc = ccRecipients,
                //Bcc = bccRecipients
            };
            await Email.ComposeAsync(message);
        }
        catch (FeatureNotSupportedException fbsEx)
        {
            // Email is not supported on this device
        }
        catch (Exception ex)
        {
            // Some other exception occurred
        }
    }
}
```

## <a name="api"></a>API

- [Quellcode-e-Mail](https://github.com/xamarin/Essentials/tree/master/Xamarin.Essentials/Email)
- [E-Mail-API-Dokumentation](xref:Xamarin.Essentials.Email)
