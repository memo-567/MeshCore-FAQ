# MeshCore-FAQ
Eine Liste häufig gestellter Fragen und Antworten zu MeshCore

Die aktuelle Version dieser MeshCore-FAQ findest du unter https://github.com/ripplebiz/MeshCore/blob/main/docs/faq.md.

Diese MeshCore-FAQ ist auch unter https://github.com/LitBomb/MeshCore-FAQ abrufbar und kann aktualisiert werden, falls Pull Requests für Scotts MeshCore-Repo noch nicht genehmigt wurden.

Autor: https://github.com/LitBomb
---

## F: Was ist MeshCore?

**A:** MeshCore ist kostenlos und Open Source.
* MeshCore umfasst das Routing, die Firmware usw. und ist auf GitHub unter der MIT-Lizenz verfügbar.
* Es gibt von der Community entwickelte Clients, wie z. B. die Web-Clients. Diese sind kostenlos nutzbar, einige davon sind ebenfalls Open Source.
* Die plattformübergreifende mobile App von [Liam Cottle](https://liamcottle.net) für Android/iOS/PC usw. kann kostenlos heruntergeladen und genutzt werden.
* Die T-Deck-Firmware wurde von Scott von Ripple Radios, dem Entwickler von MeshCore, entwickelt und kann ebenfalls kostenlos auf deine Geräte geflasht und genutzt werden.

Einige erweiterte, aber optionale Funktionen sind auf T-Deck verfügbar, wenn du dein Gerät für einen Entsperrschlüssel registrierst. Auf den MeshCore-Smartphone-Clients für Android und iOS/iPadOS kannst du die Wartezeit für die Fernverwaltung von Repeatern und Raumservern über Funk abschalten.

Diese Funktionen sind völlig optional und für das grundlegende Messaging-Erlebnis nicht erforderlich. Diese Funktionen sind wie tolle Bonusfunktionen. Um die Entwickler bei der Weiterentwicklung dieser fantastischen Funktionen zu unterstützen, erheben sie möglicherweise eine geringe Gebühr für einen Freischaltcode zur Nutzung der erweiterten Funktionen.

Jeder kann auf MeshCore kostenlos beliebige Software erstellen.

## F: Was benötigst du für MeshCore?
**A:** Alles, was du für MeshCore benötigst, findest du hier:

Hauptwebsite: [https://meshcore.co.uk/](https://meshcore.co.uk/)

Firmware-Flasher: https://flasher.meshcore.co.uk/

Telefon-Client-Anwendungen: https://meshcore.co.uk/apps.html

MeshCore Firmware Github: https://github.com/ripplebiz/MeshCore

HINWEIS: Andy Kirby bietet ein sehr nützliches [Einführungsvideo](https://www.youtube.com/watch?v=t1qne8uJBAc) für Anfänger an.

Du benötigst LoRa-Hardware, um MeshCore-Firmware als Client oder Server (Repeater und Raumserver) auszuführen.

### Hardware
Um MeshCore ohne ein Telefon als Client-Schnittstelle zu nutzen, kannst due MeshCore auf einem T-Deck oder T-Deck Plus ausführen. Es ist eine umfassende, sichere Kommunikationslösung für netzunabhängige Anwendungen.

MeshCore ist auch auf verschiedenen 868-MHz- und 915-MHz-LoRa-Geräten verfügbar. Zum Beispiel RAK4631-Geräte (19003, 19007, 19026), Heltec V3, Xiao S3 WIO, Xiao C3, Heltec T114, Station G2 und Seeed Studio T1000-E. Weitere Geräte werden später unterstützt.

### Firmware
MeshCore bietet vier Firmware-Typen, die auf anderen LoRa-Systemen so nicht verfügbar sind. MeshCore bietet Folgendes:

#### Companion Radio Firmware
Companion Radios dienen zur Verbindung mit der Android-App oder Web-App als Messenger-Client. Es gibt zwei verschiedene Firmware-Versionen:

1. **BLE Companion**
Die BLE Companion-Firmware läuft auf einem unterstützten LoRa-Gerät und verbindet sich über BLE mit einem Smartgerät, auf dem der Android MeshCore-Client läuft (der iOS MeshCore-Client ist in Kürze verfügbar).
<https://meshcore.co.uk/apps.html>

2. **USB Serial Companion**
Die USB Serial Companion-Firmware läuft auf einem unterstützten LoRa-Gerät und verbindet sich über USB Serial mit einem Smartgerät oder Computer, auf dem der MeshCore-Webclient läuft.
<https://meshcore.liamcottle.net/#/>
<https://client.meshcore.co.uk/tabs/devices>

#### Repeater
Repeater dienen zur Erweiterung der Reichweite eines MeshCore-Netzwerks. Die Repeater-Firmware läuft auf denselben Geräten wie die Client-Firmware. Die Aufgabe eines Repeaters besteht darin, MeshCore-Pakete an das Zielgerät weiterzuleiten. Im Gegensatz zu anderen LoRa-Mesh-Systemen leitet er **nicht** jedes empfangene Paket weiter oder sendet es erneut. Ein Repeater kann über ein T-Deck mit MeshCore-Firmware und freigeschalteten Fernverwaltungsfunktionen oder über einen BLE Companion-Client, der mit einem Smartphone mit MeshCore-App verbunden ist, ferngesteuert werden.

#### Raumserver
Ein Raumserver ist ein einfacher BBS-Server zum Teilen von Beiträgen. T-Deck-Geräte mit MeshCore-Firmware oder ein BLE Companion-Client, der mit einem Smartphone mit MeshCore-App verbunden ist, können sich mit einem Raumserver verbinden.

Raumserver speichern den Nachrichtenverlauf und senden ihn an Nutzer. Nutzer, die sich im Raum befinden, können später auf den Nachrichtenverlauf zugreifen. Im Gegensatz zu Kanälen werden Nachrichten entweder empfangen, wenn sie gesendet werden, oder nicht empfangen und verpasst, wenn sich ein Nutzer außerhalb der Reichweite befindet. Raumserver können Sie sich wie E-Mail-Server vorstellen, auf denen Sie später Ihre E-Mails abrufen können.

Ein Raumserver kann per Fernzugriff über ein T-Deck mit MeshCore-Firmware und freigeschalteten Fernverwaltungsfunktionen oder über einen BLE Companion Client, der mit einem Smartphone mit MeshCore-App verbunden ist, verwaltet werden.

Wenn sich ein Client bei einem Raumserver anmeldet, erhält er die zuvor nicht angezeigten 16 Nachrichten.

Ein Raumserver kann auch die Repeater-Funktion übernehmen. Um die Repeater-Funktion auf einem Raumserver zu aktivieren, verwenden Sie diese
