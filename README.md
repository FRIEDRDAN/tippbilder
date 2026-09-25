# Tippbilder

Eine einzelne, komplett offline lauffähige HTML-Seite für Kleinkinder: Jeder
Tastendruck (oder Klick/Touch) lässt ein handgezeichnet wirkendes Piktogramm im
bunten Marker-Stil aufblühen – dazu ein kleiner Ton. Kein Internet, kein
Account, keine Werbung, keine Downloads außer der einen Datei.

## Loslegen

1. `tippbilder.html` herunterladen (oder dieses Repo klonen).
2. Datei per Doppelklick im Browser öffnen (Chrome oder Firefox empfohlen).
3. Modus auswählen und auf **"Los geht's"** klicken – der Browser fragt kurz
   nach Vollbild und Ton, das ist normal.
4. Ab jetzt: einfach drauflostippen!

Es gibt keine Installation, kein Build, keine Abhängigkeiten. Die Datei
funktioniert genauso gut offline auf einem Zug wie am heimischen Rechner.

## Die drei Spielmodi

- **🎈 Frei spielen** – jede Taste lässt irgendwo auf dem Bildschirm ein
  Bild aufblühen, kurz schweben und wieder verschwinden. Manche Bilder
  verwandeln sich unterwegs in ein anderes Motiv.
- **✉️ E-Mail schreiben** – für etwas ältere Kinder. Die Bilder bleiben wie
  Buchstaben nebeneinander stehen, `Enter` beginnt einen neuen Absatz, `-`
  einen Aufzählungspunkt. Ein Klick auf "Absenden" lässt den Brief sich zu
  einem Papierflieger falten und wegfliegen (es wird nichts wirklich
  verschickt oder gespeichert).
- **🌴 Abenteuer** – eine Dschungelkulisse zieht langsam vorbei, die Bilder
  erscheinen mitten im Blattwerk und verstecken sich teilweise dahinter.

Tastendruck-Bilder orientieren sich meistens am Anfangsbuchstaben der Taste
(z. B. `K` → eher Katze als Wolke) – aber nicht immer, damit auch beim
wiederholten Tippen derselben Taste mit der Zeit alle Bilder mal auftauchen.

## Für Eltern

- **Ton an/aus:** Knopf oben rechts.
- **Zurück zur Moduswahl:** Knopf oben links.
- **Vollbild beenden:** `Esc`.
- Die App blockt die meisten Tasten (F5, Tab, …), aber **nicht** die
  Windows-Taste, `Strg+W` oder `Alt+F4` – eine Webseite kann das technisch
  nicht verhindern. Für wirklich kindersicheres Tippen am eigenen
  Kinder-Account oder im Kiosk-Modus des Browsers öffnen.
- Alles läuft rein lokal im Browser: keine Daten werden gesendet oder
  gespeichert, nichts verlässt das Gerät.

## Eigene Zeichnungen einbinden

Wer möchte, kann eigene gescannte oder fotografierte Zeichnungen zusätzlich zu
den eingebauten Piktogrammen verwenden:

1. Eigene Zeichnungen scannen/fotografieren, als PNG oder JPG speichern (am
   besten mit transparentem Hintergrund).
2. Die Bilddateien in denselben Ordner wie `tippbilder.html` legen.
3. `tippbilder.html` in einem Texteditor öffnen und ganz oben im
   `<script>`-Bereich die Dateinamen eintragen, z. B.:
   ```js
   const EIGENE_BILDER = ["katze.png", "haus.png", "oma.jpg"];
   ```
   Sollen **nur** eigene Bilder erscheinen (keine eingebauten Piktogramme):
   direkt darunter `const NUR_EIGENE = true;` setzen.

Wer den Code selbst lesen oder erweitern möchte: `tippbilder.html` ist
durchgehend kommentiert (Architektur-Überblick ganz oben im `<style>`-Block).

## Lizenz

[MIT](LICENSE) © 2026 FRIEDRDAN
