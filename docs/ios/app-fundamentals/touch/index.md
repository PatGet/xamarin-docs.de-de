---
title: Behandlung von Touch Xamarin.iOS Apps
description: Dieses enthält Dokumentenlinks zu Anleitungen, die zum Arbeiten mit Touch, Multitouch-Gesten und 3D Touch in einer app Xamarin.iOS beschreiben.
ms.prod: xamarin
ms.assetid: E3904713-6018-4755-A315-EB045DFB3500
ms.technology: xamarin-ios
author: bradumbaugh
ms.author: brumbaug
ms.date: 01/23/2017
ms.openlocfilehash: eb8dce8b13345c13a6f95ae7784bd135e7d1f1f5
ms.sourcegitcommit: ea1dc12a3c2d7322f234997daacbfdb6ad542507
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2018
ms.locfileid: "34784161"
---
# <a name="handling-touch-in-xamarinios-apps"></a>Behandlung von Touch Xamarin.iOS Apps

Wie bei anderen mobilen Plattformen hat iOS vielfältige Weise Toucheingabe zu behandeln. Es kann Multi-Touch unterstützen – viele Kontaktpunkte auf dem Bildschirm – und komplexe Gesten. Dieses Handbuch enthält einige der Konzepte sowie den Besonderheiten des Touch- und Gesten auf iOS-Implementierung.

iOS kapselt Touch-Daten in der `UITouch` -Klasse, durch eine Reihe von Anwendungen zur Verfügung gestellt werden `UIResponder` Methoden. Anwendungen können diese Methoden in Unterklassen überschreiben `UIView` und `UIViewController`, beide erben von `UIResponder`.

Zusätzlich zum Erfassen der Touch-Daten, bietet iOS bedeutet, dass für das Muster der Fingereingaben in Gesten interpretieren. Diese Bewegung Prüfer können wiederum zum Interpretieren von anwendungsspezifischen Befehle, wie z. B. eine Drehung ein Bild oder eine Deaktivieren einer Seite verwendet werden. iOS bietet eine umfassende Sammlung von Klassen häufige Gesten mit minimalen hinzugefügten Code behandeln.

Die Wahl zwischen Fingereingaben sowie Geste Prüfer kann eine verwirrend sein. Es wird empfohlen, im Allgemeinen Voreinstellung für die Geste Prüfer gewährt werden soll. Prüfer Geste werden als diskrete Klassen implementiert, die wodurch die stärkere Trennung von Anliegen und eine bessere Kapselung bereitzustellen. Dies erleichtert die Logik zwischen verschiedenen Ansichten, minimieren die Menge an Code geschrieben freigeben.

Es gibt jedoch auch vorkommen, dass Sie auf niedriger Ebene Touch-Verarbeitung verwenden und sogar mehrere Finger, z. B. zum Erstellen eines Programms Finger-paint nachverfolgen müssen.

## <a name="sections"></a>Abschnitte

-  [Toucheingabe in iOS](touch-in-ios.md)
-  [Exemplarische Vorgehensweise: Verwenden von Touch in iOS](ios-touch-walkthrough.md)
-  [Nachverfolgen von Multitoucheingaben](touch-tracking.md)

Dieses Handbuch dient als Einführung in die Fingereingabe iOS. Weitere Informationen zur Verwendung von 3D Touch und Haptic Feedback in iOS wurden die in iOS 9 und 10, die bzw. der bestimmte Anleitungen unten finden Sie eingeführt:

* [3D Touch](~/ios/platform/3d-touch.md)
* [Übermitteln von haptischem Feedback](~/ios/user-interface/ios-ui/haptic-feedback.md)

## <a name="related-links"></a>Verwandte Links

- [iOS berühren starten (Beispiel)](https://developer.xamarin.com/samples/monotouch/ApplicationFundamentals/Touch_start)
- [iOS endgültigen berühren (Beispiel)](https://developer.xamarin.com/samples/monotouch/ApplicationFundamentals/Touch_final)
- [FingerPaint (Beispiel)](https://developer.xamarin.com/samples/monotouch/ApplicationFundamentals/FingerPaint)
