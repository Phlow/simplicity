---
layout: post
subheadline: Icon Fonts
title: Icon Fonts mit Font Custom erstellen
teaser: Mit der Open Source-Software Font Custom erstellt man sich maßgeschneiderte Icon Fonts, die man für eigene Webdesign-Projekte nutzen kann.
permalink: 
category:
    - webdesign
tags:
    - typography
    - icon font
    - icons
    - svg
image:
    homepage: icon-font-font-custom.png
    title: icon-font-font-custom.png
comments: true
---
Icon Fonts bieten eine großartige Möglichkeit Websites mit vektorbasierten Icons zu verschönern. Da es sich um einen Schriftdatei handelt, kann diese auch mit den üblichen CSS-Eigenschaften wie z.B. *hover*, *text-shadow*, *color* und ähnlichem gestaltet werden.

Zahlreiche Icon Fonts wie z.B. Font Awesome oder der von mir geschätzte Entypo-Icon-Satz bieten oft viel zu viele individuelle Icons. Oft reichen ein paar wenige. Manchmal möchte man aus verschiedenen SVG-Icons auch einen individuellen Icon Font für eigene Projekte erstellen.

Natürlich bietet das Web zahlreiche Online-Services wie z.B. [icomoon.io][4], [fontastic.me][2] oder [fontello.com][3] über welche man sich seine eigenen Icon Fonts im Browser zusammenklicken kann. Persönlich mag ich aber den direkten Zugriff auf die Dateien und genau das bietet [Font Custom][1].


## Font Custom installieren

Font Custom installiert man mit [Brew][5] in drei Schritten.

~~~
brew install fontforge --with-python
brew install eot-utils
gem install fontcustom
~~~

![Preview des Icon Fonts]({{ site.urlimg }}font-custom-preview.png)
<small class="sans text-right">Preview des Icon Fonts</small>

## Font Custom nutzen

Zu anfangs irritierte mich die Anleitung auf der Website von Font Custom ein wenig. Darum hier die eigentlich einfachen Schritte, um sich den eigenen Icon Font zusammenstricken zu lassen.

1. Terminal öffnen.
2. Verzeichnis mit `mkdir custom-font` erstellen
3. In das Verzeichnis mit `cd custom-font` wechseln.
4. Mit `fontcustom config`  die Standard YAML-Konfigurationsdatei erstellen.
5. Konfigurationsdatei `fontcustom.yml` öffnen, konfigurieren, speichern.
6. SVG-Dateien in das Verzeichnis *custom-font* kopieren.
7. Font Custom im Terminal mit `fontcustom watch` starten.
 
Dank des Watch-Vorgangs läuft jetzt Font Custom im Hintergrund und erzeugt eine neue Version des Fonts sobald man eine neue SVG-Vektor-Datei in das in `fontcustom.yml` definierte Verzeichnis wirft.

Sehr gut an Font Custom finde ich die zusätzlich erzeugte HTML und CSS-Datei, die den Font im Einsatz zeigt.



 [1]: http://fontcustom.com/
 [2]: http://fontastic.me/
 [3]: http://fontello.com/
 [4]: https://icomoon.io/app/
 [5]: http://brew.sh/
