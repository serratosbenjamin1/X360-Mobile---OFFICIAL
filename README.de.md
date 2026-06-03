# X360 Mobile - Xbox 360 Emulator für Android

<p align="center">
  <img src="https://x360mobile.com/logo.png" alt="X360 Mobile Logo" width="180" style="border-radius: 20%;"/>
</p>

<p align="center">
  <b>Ein experimenteller, nativer Xbox 360-Emulator für Android, der nativ auf Xenia Canary basiert.</b>
</p>

<p align="center">
  <a href="https://www.x360mobile.com"><b>Offizielle Website: www.x360mobile.com</b></a>
</p>

<p align="center">
  Choose Language / Scegli la lingua / Sprache wählen / Choisir la langue / Seleccionar idioma:
  <br>
  <a href="README.md">English</a> |
  <a href="README.it.md">Italiano</a> |
  <b>Deutsch</b> |
  <a href="README.fr.md">Français</a> |
  <a href="README.es.md">Español</a>
</p>

---

Willkommen im offiziellen Repository von **X360 Mobile**, einem experimentellen, nativen Xbox 360-Emulator, der speziell für die Android-Plattform entwickelt wurde. X360 Mobile wurde mit modernen ARM64- und Vulkan 1.3-Technologien entwickelt und ist der **Pionier bei der nativen Nutzung des hochgelobten Xenia Canary-Cores unter Android**. Er bringt fortschrittliche Optimierungen und Spitzenleistung direkt auf Ihre High-End-Mobilgeräte.

> [!NOTE]
> **Zweck des Repositories:** 
> Um die Codebasis zu schützen und proprietäre Leistungsverbesserungen beizubehalten, ist **X360 Mobile Closed-Source**. Dieses offizielle Repository enthält nicht den Quellcode des Emulators. Stattdessen dient es als **offizielles Versionsarchiv und primäre Vertriebsplattform** für die Veröffentlichung von APK-Builds, die Verwaltung von Kompatibilitätsproblemen (Issues) und die Bereitstellung von Benutzerhandbüchern.

---

## Hauptmerkmale

* **Native Xenia Canary-Basis:** Der allererste Android-Emulator, der von Anfang an nativ auf Xenia Canary ausgelegt war, anstatt nachträglich von Xenia Master zu migrieren, was eine überlegene Architektur und Leistung garantiert.
* **Modernes Vulkan-Backend:** Nutzt Vulkan 1.3, um eine optimale Hardwareauslastung, hohe Bildraten (FPS) und einen minimalen System-Overhead zu liefern.
* **Benutzerdefiniertes Touch-Overlay:** Vollständig anpassbare virtuelle Gamepads mit haptischem Feedback, flüssiger analoger Ansprache und maßgeschneiderten Layouts für jede Bildschirmgröße.
* **Unterstützung für physische Controller:** Nahtlose Plug-and-Play-Unterstützung für externe Controller über Bluetooth oder USB-OTG (einschließlich Xbox Series X|S, DualSense, DualShock 4 und gängigen mobilen Controllern).
* **Spielspezifische Profile:** Passen Sie Auflösungen, Shader-Kompilierungsoptionen und Speicherbeschränkungen für jedes Spiel einzeln an, um das Maximum aus Ihrem Gerät herauszuholen.
* **Optimierungen für Mobilgeräte:** Integrierte Übersetzung von PowerPC-Assembly in ARM64-Instruktionen mit spezifischen Mikrooptimierungen für Snapdragon- und Dimensity-Chipsätze.

---

## Systemanforderungen

Die Emulation der Xbox 360 ist ein experimenteller und rechenintensiver Prozess, der eine komplexe Hardwareübersetzung in Echtzeit erfordert. Bitte prüfen Sie die folgenden Anforderungen, um die erwartete Leistung Ihres Geräts einschätzen zu können.

| Spezifikation | Mindestanforderungen | Empfohlen (Für spielbare Geschwindigkeiten) |
| :--- | :--- | :--- |
| **Betriebssystem** | Android 11 (64-Bit) | Android 13 oder neuer (64-Bit) |
| **Prozessor & GPU** | Qualcomm Snapdragon mit Adreno-GPU (Serie 600/700/800) | High-End-Qualcomm Snapdragon (Snapdragon 8 Gen 1 oder neuer empfohlen) |
| **RAM (Arbeitsspeicher)**| 6 GB RAM | 8 GB - 12 GB RAM (oder mehr) |
| **Speicher (Geschwindigkeit)** | Schneller Speicher (UFS 3.1 oder besser empfohlen) | Ultraschneller UFS 3.1/4.0 Speicher |

> [!WARNING]
> Geräte mit Prozessoren, die über Mali-GPUs, Samsung Xclipse-GPUs (AMD RDNA-basiert), ältere Adreno-GPUs (vor der 600er-Serie) oder Einstiegs-Chipsätze verfügen, weisen erhebliche Leistungseinschränkungen, Grafikfehler, starkes Thermal Throttling oder Abstürze auf. Für optimale Ergebnisse wird ein moderner Qualcomm Snapdragon-Prozessor mit einer Adreno-GPU dringend empfohlen.

---

## Schnellstartanleitung

1. **APK herunterladen:** Gehen Sie zu unserem Bereich [Releases](https://github.com/Ashnar2602/X360-Mobile---OFFICIAL/releases) und laden Sie das neueste stabile `.apk`-Paket herunter.
2. **Unbekannte Quellen zulassen:** Erlauben Sie bei Aufforderung Ihrem Webbrowser oder Dateimanager in den Android-Sicherheitseinstellungen, Anwendungen aus unbekannten Quellen zu installieren.
3. **Installieren und Starten:** Installieren Sie die heruntergeladene APK-Datei und starten Sie **X360 Mobile**.
4. **Verzeichnisse konfigurieren:** Erstellen Sie ein eigenes Verzeichnis auf dem internen oder externen Speicher Ihres Geräts (z. B. `/Emulation/Xbox360/Games`) und kopieren Sie Ihre legal erworbenen Spieldateien dorthin.
5. **Spielformate:** Der Emulator unterstützt offiziell die Formate `.iso`, `.xex` und entpackte Ordnerstrukturen (unpacked).
6. **Laden & Spielen:** Richten Sie den Emulator auf Ihren Spieleordner aus, wählen Sie ein Spiel aus und starten Sie das Gameplay!

---

## Häufig gestellte Fragen (FAQ)

### Ist X360 Mobile kostenlos?
**Ja.** Der Download und die Nutzung von X360 Mobile sind völlig kostenlos. Wir verlangen keine Gebühren und schalten keine störende Werbung, die das Spielerlebnis beeinträchtigt.

### Warum ist das Projekt Closed-Source?
Wir haben uns dafür entschieden, X360 Mobile Closed-Source zu halten, um betrügerische Forks, schädliche Neuverpackungen (z. B. das Einschleusen von Adware/Spyware in unsere Builds) zu verhindern und unsere proprietäre ARM64-Konvertierungspipeline sowie Compiler-Optimierungen zu schützen. Wir möchten sicherstellen, dass Benutzer nur sichere, hochoptimierte und offiziell signierte Pakete direkt aus diesem Repository oder von unserer offiziellen Website erhalten.

### Steht X360 Mobile in Verbindung mit dem Desktop-Projekt Xenia?
X360 Mobile basiert auf der hervorragenden Codebasis von **Xenia Canary** (einem Open-Source-Projekt für PC). Wir haben die Kern-Rendering- und Ausführungs-Engines portiert, überarbeitet und optimiert, damit sie unter Android laufen. Wir haben größten Respekt vor den ursprünglichen Xenia-Entwicklern und möchten die gleiche hohe Qualität auf Mobilgeräten bieten.

### Welche Spiele kann ich im Moment spielen?
Die Kompatibilität wird kontinuierlich verbessert. Derzeit wurden **über 300 Titel getestet**, von denen etwa **40 % voll spielbar** sind.

Eine vollständige und aktuelle Kompatibilitätsliste finden Sie auf unserer offiziellen Website unter [www.x360mobile.com](https://www.x360mobile.com). Während klassische Arcade-Titel, Indie-Spiele und weniger anspruchsvolle 3D-Spiele sehr gut laufen, anspruchsvolle AAA-Titel (wie *Red Dead Redemption*, *Halo 3* oder *Gears of War*) startbar und können auf den neuesten Flaggschiff-Snapdragon-Prozessoren spielbare Geschwindigkeiten erreichen, weisen jedoch unter Umständen noch kleinere Grafikfehler oder Bildrateneinbrüche auf.

---

## Fehler melden

Wenn Sie auf Abstürze, Grafikfehler oder Kompatibilitätsprobleme stoßen:
1. Gehen Sie zu unserem Bereich [Issues](https://github.com/Ashnar2602/X360-Mobile---OFFICIAL/issues).
2. Prüfen Sie, ob das Problem bereits von einem anderen Benutzer gemeldet wurde.
3. Falls nicht, öffnen Sie ein neues Ticket mit unserer Vorlage und machen Sie folgende Angaben:
   * Ihr Gerätemodell und der verbaute Chipsatz (z. B. Samsung Galaxy S23, Snapdragon 8 Gen 2).
   * Die genaue Android-Version und der Arbeitsspeicher.
   * Der Spieletitel und das Dateiformat (.iso oder .xex).
   * Eine detaillierte Beschreibung des Fehlers und, falls möglich, Screenshots oder Videos.

---

## Rechtliche Hinweise & Haftungsausschluss

* **Xbox 360** ist eine eingetragene Marke der Microsoft Corporation. **X360 Mobile** steht in keinerlei Verbindung mit der Microsoft Corporation, ihren Tochtergesellschaften oder verbundenen Unternehmen und wird von diesen weder autorisiert, gesponsert noch unterstützt.
* Alle Spieletitel, Bilder und Markenwerte sind Marken ihrer jeweiligen Eigentümer.
* **X360 Mobile** enthält keine Spieldateien, Systemsoftware (Dashboard) oder urheberrechtlich geschützte ROMs. Benutzer sind gesetzlich verpflichtet, physische Kopien der Spiele zu besitzen und diese für den persönlichen, nicht-kommerziellen Gebrauch selbst zu sichern (Dump).
* Durch das Herunterladen und Nutzen dieser Software stimmen Sie unseren Nutzungsbedingungen zu und erkennen an, dass die Emulation eine experimentelle Technologie ist, die auf eigene Gefahr verwendet wird.

---

<p align="center">
  © 2026 X360 Mobile Team. Alle Rechte vorbehalten. <br>
  Für Neuigkeiten, Updates und mehr besuchen Sie <a href="https://www.x360mobile.com">www.x360mobile.com</a>.
</p>
