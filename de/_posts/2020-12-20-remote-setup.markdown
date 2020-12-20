---
layout: single
title: "rC3 Remote Streaming zu OIO/A:F"
date: 2020-12-19 13:37:00 +0100
lang: de
toc: true
classes: wide
ref: rc3-remote-streaming
---

Zum rC3 möchten wir die Möglichkeit bieten, euch so anzubinden, dass ihr eure Talks auch von zu Hause aus halten könnt.

Bitte lest euch diese Dokumentation durch und probiert die beschriebenen Werkzeuge aus. Kommt bei Fragen auf uns zu und lasst uns das Setup auch gemeinsam testen. Macht euch auch damit vertraut, falls euer Beitrag momentan noch live on stage geplant ist.

Die Auswahl der Werkzeuge basiert auf den Erfahrungen aus einigen durchgeführten Onlineveranstaltungen in diesem Jahr.

## Architektur

1. Übertragung Kamerabild/Ton und Folien/andere Form der Präsentation zum OIO: OBS-Ninja
2. Rückkanal und Notfall-Kommunkation bei Störungen: Jitsi

![](/images/rc3-remote-streaming/obs-ninja.png)

![](/images/rc3-remote-streaming/jitsi.png)

### Jitsi-Kanal
Jitsi ist eine quelloffene Software für Onlinemeetings. Es benötigt keine weitere Softwareinstallation und wird am besten in Chromium/Chrome benutzt.

### OBS-Ninja Desktop/Videoshare
Eurer Content zur Regie: OBS-Ninja ist ein Browser-Streaming, das keine Installation einer App benötigt sondern lediglich einen aktuellen Browser (Chromium/Chrome bevorzugt).

## Ablauf
Vor dem offiziellen Start des rC3 möchten wir mit jedem von euch das Setup einmal testen. Wir melden uns bei euch, um einen Termin zu vereinbaren.

Der Ablauf ist grundsätzlich so:

* ihr kommt 30 Minuten vor eurem Talk in einen definierten Jitsiraum, das Foyer. Die URL wird noch bekannt gegeben.
* ein Regieengel holt euch dort ab und "bringt" Euch "in einen Saal". Das wird ein spezieller Jitsiraum nur für diesen Talk sein.
* Vor eurem Talk bekommt ihr zwei URLs für Euren Browser
  * **URL für Camera-Share**: Diesem Browser gebt ihr Zugriff auf Webcam und Mikrofon. Das Browserfenster könnt ihr dann minimieren.
  * **URL für Slide/Desktop-Share**: Dort wählt ihr entweder das Fenster mit der Applikation aus, die ihr für Eure Präsentationsfolien nutzen wollt oder den Komplettbildschirm.
  * Falls ihr mehrere Vortragende seid oder mehrere Kameras habt, z.B. wenn noch was unter einer Dokumentenkamera gebastelt wird, gibt es so viele URLs bis alle Teilnehmenden und alle Kameras versorgt sind.
  * solltet ihr keine URLs bekommen haben können wir sie spätestens in den 30 Minuten vor dem Talk einrichten.
* Wenn die Technik richtig funktioniert
    * Wir warten gemeinsam auf den Beginn eures Talks laut Fahrplan.
    * Ein Herald wird Euren Talk anmoderieren, evtl. wechselt ihr auch dabei im Dialog schon ein paar Worte. Herald und Regie werden per Jitsi zu hören und ggf. zu sehen sein.
    * Ihr haltet einfach Euren Talk, die Bildmischung zwischen den Bildquellen (Folien/Speaker) macht die Regie
    * Bei jeweils 10min und 5min Restzeit bekommt ihr eine entsprechende kurze Ansage von der Regie über Jitsi
    * Im Anschluss an Euren Talk übernimmt der Herald wieder und wird das Q&A mit dem Signalangel machen. Mangels Publikum vor Ort werden die Fragen aus verschiedenen Kanälen im Internet kommen.
    * Es besteht die Möglichkeit, detaillierte Gespräche in einem eignenen Raum nach dem Ende des Talks fortzuführen.

### Ein paar Tipps an dieser Stelle

* Wenn ihr Folien mit "Video+Ton-Einspielern" habt: **Chrome/Chromium** ist der einzige Browser, der (unseres Wissens nach) derzeit zuverlässig Audio "vom Desktop" senden kann. Zudem ist es ein Browser, dem es zumindest teilweise gelingt, die Videokompression in vorhandene Hardware, wie z.B. CPU-Einheiten oder Grafikkarte, auszulagern. Das verbessert die Bildqualität erheblich
* Bitte **verzichtet auf GEMA-pflichtige Musik** in euren Beiträgen.
* Mikrofon & Audio Setup verdienen Eure Aufmerksamkeit: **Kopfhörer sind unbedingte Voraussetzung**, egal ob große Headsets oder kleine Ohrstecker
    *  ein **Ansteck-Mikrofon** verbessert den Sound, **Headsets sind noch besser**! Das Mikrofon im Laptop wird vermutlich keinen guten Dienst leisten, da beim Videostreaming oft die Lüfter hochdrehen und dieser Lärm im Audiostream landet
* **Licht ist wichtig**: Macht so viel Licht, dass ihr gerade noch Euren Laptop sehen könnt. Webcams sind, verglichen mit den in Telefonen üblichen Kameras, erstaunlich lichtschwach
* **Fingerabdrücke auf der Kameralinse** vorher beseitigen. Dabei hilft ein Brillenputztuch
* **Redshift** (oft in Verbindung mit "Nightmode") sieht in Präsentationen nicht gut aus
* Bitte schließt während eures Talks alle Programme, die nicht notwendig sind. Dadurch vermeidet ihr, dass Popups von Messengern oder Benachrichtigungen aus anderen Browserfenstern während eurer Präsentation erscheinen.
* Wenn möglich, nutzt zwei Monitore. Einen gebt ihr frei und zeigt eure Präsentation. Auf dem anderen Monitor können dann andere Fenster sein, z.B. das mit dem Rückkanal für Herald und Regie.
* Wenn ihr ein **ausgefeiltes Kamera-Setup** oder gar selbst ein Studio betreiben solltet: Im OBS-Ninja könnt ihr auch die Virtual-Webcam als Quelle angeben. Oder einen HDMI-Grabber, an dem eine Videokamera hängt.
* **Aufgezeichnete Talks** (Pre-Recording) und nur "Q&A-Live" ist durchaus eine Option, wenn ihr Euch nicht sicher seid, dass die Internet-Bandbreite ausreicht und stabil genug ist. Entweder als "Live on Tape"-Aufzeichnung vorab von einem Ort mit besserer Anbindung oder ihr nehmt selbst, z.B. mit OBS auf. Entsprechene Folienlayouts für Splitscreen-Ansichten wird es in den nächsten 2-3 Tagen geben.

# Details zu den eingesetzten Werkzeugen
## OBS NINJA
Um Euren Vortrag auf die OIO/A:F-Bühne zu bringen nutzen wir OBS Ninja. Dies ist eine Live-Streaming Software die rein im Browser funktioniert und somit keine zusätzliche Softwareinstallation benötigt. Ihr bekommt von uns zwei Links zugesendet. Die Kanäle werden passwortgeschützt sein, um ungebetenen Besuch zu vermeiden. Natürlich könnt ihr im Vorfeld auch schon selbst damit spielen und eigene Räume anlegen.

Bitte beachtet, dass ihr zwei Fenster, bzw. Tabs, von OBS-Ninja braucht, um sowohl die Webcam zu nutzen als auch den Bildschirm zu teilen. OBS-Ninja läuft aktuell am besten in Chromium/Chrome.

### Einen Invite-Link verwenden
Kopiert den Link in die Adresszeile eures Browsers und gebt das Passwort ein.

![](/images/rc3-remote-streaming/obs-ninja-invite.png)
Gebt Bildschirm und Webcam frei.

### Einen Raum eröffnen
Geht auf die VOC-OBS-Ninja-Seite [OBS-Ninja](https://ninja.c3voc.de/) und startet mit der Auswahl/Freigabe von Screenshare und Kamera.

![](/images/rc3-remote-streaming/obs-ninja-raum-oeffnen.png)

### Webcam einrichten
Um die Kamera freizugeben muss nun die korrekte Kamera ausgewählt und im Browser freigegeben werden.
![](/images/rc3-remote-streaming/obs-ninja-webcam1.png)

Nun gibt es ein kleines Vorschaubild in dem die Ansicht kontrolliert werden kann. Die sonstigen Einstellungen sollten den zuvor gewählten Einstellungen im Browser entsprechen.
![](/images/rc3-remote-streaming/obs-ninja-webcam2.png)

Beginnt den Stream mit einem Klick auf den Startbutton.
![](/images/rc3-remote-streaming/obs-ninja-webcam3.png)

### Bildschirm freigeben
Wählt den gewünschten Bildschirm aus und gebt diesen im Browser frei.

![](/images/rc3-remote-streaming/obs-ninja-screenshare1.png)

Bestätigt die Auswahl und startet die Übertragung mit dem Share Button.
![](/images/rc3-remote-streaming/obs-ninja-screenshare2.png)

Unter MacOS muss in Firefox die Bildschrimfreigabe erstmalig bestätigt werden.
![](/images/rc3-remote-streaming/obs-ninja-screenshare3.png)
Danach muss Firefox noch einmal neu gestartet werden.
![](/images/rc3-remote-streaming/obs-ninja-screenshare4.png)

### Bedienelemente
Es gibt unter dem Videobild Bedienelemente die die Übertragung steuern.

Links ist eine Sprechblase die ein Chatfenster öffnet. Der Chat ist für alle Teilnehmer sichtbar.

Daneben ist ein Lautsprechersysmbol, mit dem die Übertragung von Tönen aus anderen Programmen gestoppt werden kann.

Das 3. Symbol von links ist ein Mikrofon mit dem das eigene Mikro ausgeschaltet werden kann.

Daneben befindet sich ein Auge mit dem die Übertragung schwarz geschaltet wird, so dass der eigene Bildschrim bzw. die Webcam nicht mehr zu sehen sind.

Das Zahnrad öffnet die Streameinstellungen in denen z.B. andere Mikrofone ausgewählt werden können oder ein anderer Bildschrim zur Übertragung.

Ganz rechts ist ein rotes Telefon mit dem der Anruf/Stream beendet wird.

![](/images/rc3-remote-streaming/obs-ninja-buttons.png)

## Jitsi

Als Rückkanal zu euch verwenden wir einen Raum in Jitsi. Diesen öffnet ihr in einem anderen Tab eures Browsers. Über diesen Kanal werden ihr dann die Moderation des Heralds und gestellte Fragen hören oder Anweisungen aus der Regie.

Wir senden euch einen Link zu, über den ihr direkt den Raum betretet. Auch hier müsst ihr im ersten Schritt eure Freigabe für das Mikrofon und optional die Kamera erteilen.

Die wichtigsten Bedienelemente beinden sich hier in der Mitte. Links der Mitte kann man das Mikrofon an- oder ausschalten, rechts die Kamera und mit dem roten Knopf in der Mitte verlässt man den Raum wieder.

![](/images/rc3-remote-streaming/jitsi-bedienung.png)

# Selbst testen
Hier könnt ihr selbst Eure Bildqualität beurteilen, auch in Abhängigkeit von der gewählten Maximalauflösung und Eurer nutzbaren Internetbandbreite.
Probiert es selbst aus mit unterschiedlichen Settings, vorzugsweise mit zwei getrennten PCs an unterschiedlichen Internetanschlüssen, da das genutzte Protokoll webRTC sonst (idealerweise) gar nicht "durch's Internet" geht, sondern lokal bleibt, was Einflüsse von z.B. verfügbarer Upload-bandbreite nicht zeigt.

* Speaker-Kamera
    * Quell-PC: https://obs.ninja/?push=xJf8Mqs&room=test&hash=2e40&label=OIO_Test_Cam
        * (self-monitor/view: https://obs.ninja/?view=xJf8Mqs&scene&room=test&password=test123&label=OIO_Test_Cam)
* Speaker-Screenshare
    * Quell-PC: https://obs.ninja/?push=v2QAmBj&room=test&hash=2e40&label=OIO_Test_Screenshare
        * (self-monitor/view: https://obs.ninja/?view=v2QAmBj&scene&room=test&password=test123&label=OIO_Test_Screenshare)

nochmal als Tabelle, zum einfacheren Klicken

Funktion | Sender | Empfänger
---------|--------|----------
Speaker-Video |[Quelle](https://obs.ninja/?push=xJf8Mqs&room=test&hash=2e40&label=OIO_Test_Cam) | [Ziel/Monitor](https://obs.ninja/?view=xJf8Mqs&scene&room=test&password=test123&label=OIO_Test_Cam)
Speaker-Screenshare| [Quelle](https://obs.ninja/?push=v2QAmBj&room=test&hash=2e40&label=OIO_Test_Screenshare)| [Ziel/Monitor](https://obs.ninja/?view=v2QAmBj&scene&room=test&password=test123&label=OIO_Test_Screenshare)

## Test-Session / technische Stellprobe
Wir werden eure Setups im Vorfeld mit euch testen. Dazu bekommt ihr noch eine Email oder habt sie schon längst bekommen.

Dabei geht es vor allem um die optimalen Einstellungen von Bild- und Audioqualität. Euren Talk müsst ihr dafür also noch nicht fertig haben!

Solltet ihr Fragen haben oder Probleme mit den oben beschriebenen Werkzeugen aufreten, kontaktiert uns bitte schnellstmöglich.

# Für Eure Folien
## Layout
* keine wichtigen Details in die untere rechte Ecke, wenn möglich bitte.
(Beispielbild von 2019)
    *  Das Kamerabild wird die rechte untere Ecke möglicherweise überlappen.
    *  wenn Ihr ein Branding dort haben solltet, dann wäre es gut, wenn ihr es nach links oder oben verschieben könntet. Wenn das nicht geht, dann werden wir diese Ansicht nicht nutzen.
![](/images/rc3-remote-streaming/slides-example.png)
* Erstellt eure Präsentationen bitte im Format 16:9, da es sonst schwarze Streifen an den Rändern geben wird.

## Artwork and Fonts
Falls ihr Eure Folien noch nach dem Event-Motto optisch gestalten wollen solltet, könnt ihr euch den Styleguide ansehen: https://howto.rc3.world/styleguide.html

## Tipps & Tricks

Die meisten Betriebsysteme haben mindestens eine Möglichkeit die Aufnahmen eurer Webcam anzuzeigen. Schau dir also vor deinem Talk einmal das Bild deiner Kamera an und stell fest ob du damit zufrieden bist. Beachte die Lichtverhältnisse die zum Zeitpunkt deines Talks herschen werden.
Ein Kameracheck mittags um 12 Uhr mit Tageslicht ist nicht aussagekräftig, wenn dein Talk erst abends um 22 Uhr stattfindet. Eventuell lohnt es sich du noch eine Lampe umstellen um das Licht zu verbessern. Pass aber auf, dass du nicht überbelichtet bist und ein einfarbiger Fleck wirst.

Gestallte deinen Hintergrund möglichst neutral und vermeide persönliche Gegenstände wie deinen Geburtstagskalender, Passwörter oder eine freie Sichtlinie in das Fenster deiner Nachbarn.  Je langweiliger dein Hintergrund ist, desto besser.

Die Vortragsweise ist dieses Jahr deutlich anders als in den letzten Jahren. Es gibt keine direkten Zuschauer und auch kein sofortiges Feedback aus dem Publikum. Gestalte deinen Vortrag persönlicher indem du Wackelaugen, dein Lieblingsstofftier oder eine Quietscheente auf/an/um/hinter die Kamera setzt. Dadurch schaust du den Zuschauern im Stream öfters ins Gesicht und hast gleichzeitig "reale" Zuschauer, was häufig das Vortragen erleichtert.

<small>Vielen Dank an die [RheinRuhrStage](https://r3s.nrw), deren Dokumentation wir als Grundlage für diesen Beitrag genommen haben!</small>
