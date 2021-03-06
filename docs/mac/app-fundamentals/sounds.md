---
title: Die Wiedergabe von sound mit AVAudioPlayer xamarin.Mac
description: Dieses Dokument beschreibt, wie Sie die Wiedergabe von sound mit AVAudioPlayer in einer Xamarin.Mac-app. Es wird erläutert, AVAudioPlayer zu einem hohen und Links zu weiteren Informationen, die sie genauer untersucht.
ms.prod: xamarin
ms.assetid: 4A683A94-F75D-4EAF-8497-E9443653250B
ms.technology: xamarin-mac
author: bradumbaugh
ms.author: brumbaug
ms.date: 10/19/2016
ms.openlocfilehash: 03a0207ce8c742f0ca98ab6c75ed3e7b2f37d09e
ms.sourcegitcommit: b56b3f906d2c05a3f1be219ef41be8b79e519b8e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/25/2018
ms.locfileid: "39241353"
---
# <a name="playing-sound-with-avaudioplayer-in-xamarinmac"></a>Die Wiedergabe von sound mit AVAudioPlayer xamarin.Mac

## <a name="about-the-avaudioplayer"></a>Informationen zu den AVAudioPlayer

Die `AVAudioPlayer` Klasse wird zum Wiedergeben von Audiodaten aus entweder im Arbeitsspeicher oder eine Datei. Apple empfiehlt die Verwendung dieser Klasse, die audio in Ihrer app wiedergeben, es sei denn, Sie machen die streaming-Netzwerk oder mit geringer Latenz audio-e/a erfordern.

Sie können die `AVAudioPlayer` Klasse, um die folgenden Aktionen ausführen:

- Wiedergeben von Sound beliebiger Dauer mit optionalen Schleifen.
- Mehrere Sound zur gleichen Zeit mit optionalen Synchronisierung.
- Steuern Sie Volumes, Playback-Geschwindigkeit und Stereo-Positionierung für jede Sounds wiedergeben.
- Unterstützung von Funktionen wie ein Zeitsprung oder Rewind.
- Wiedergabe-Ebene, die Verwendungsdaten zu erhalten.

`AVAudioPlayer` unterstützt die Sounds in einem beliebigen audio Format, das von iOS, TvOS und MacOS wie z. B. .aif, WAV- oder MP3 bereitgestellt.

## <a name="playing-sounds-in-macos"></a>Wiedergabe von Sound in macOS

Da MacOS über die gleichen Audio Toolbox-Klassen als iOS unterstützt, finden Sie unserem iOS [spielen Sound mit AVAudioPlayer](https://github.com/xamarin/recipes/tree/master/Recipes/ios/media/sound/avaudioplayer) Dokumentation für die vollständigen Details der Audiowiedergabe in einer Xamarin.Mac-app.

## <a name="related-links"></a>Verwandte Links

- [AVAudioPlayer-Referenz](https://developer.apple.com/documentation/avfoundation/avaudioplayer)
