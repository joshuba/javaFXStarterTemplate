# JavaFX Starter Template

Dieses JavaFX Starter Template nutzt das Build-System [Gradle](https://gradle.org), um einfach ein Java Projekt mit Java 17 und JavaFX zu starten.


## Anleitung
1. Diesen Projektordner kopieren und beliebig benennen
2. (optional) in `settings.gradle` Eintrag `rootProject.name` an App-Namen anpassen
3. Projekt in beliebiger IDE/Text-Editor öffnen:
   1. Eclipse: `File/Import/Gradle/Existing Gradle Project`
   	1. Run Configuration anpassen
   2. IntelliJ `File/Open` (dann ggf. `Import as Gradle Project`)
4. Gradle Dependencies installieren
   1. Terminal Linux/MacOS: `./gradlew install`\
   2. Terminal Windows: `gradlew.bat install`
   3. Mit Eclipse: Rechtsklick auf das Projekt, dann `Gradle/Refresh Gradle Project`
   4. In IntelliJ: Rechts in der vertikalen Toolbar auf den Gradle-Elefanten klicken und dann auf das Reload Symbol
5. Sicherstellen, dass Project SDK korrekt gesetzt ist
   1. In Eclipse unter `File/Properties/Java Build Path/Libraries` nachsehen
   2. In IntellIJ unter `File/Project Structure/Project/SDK` nachsehen
6.  JavaFX App starten:
    1. Terminal Linux/MacOS: `./gradlew run`
    2. Terminal Windows: `gradlew.bat run`
    3. Eclipse: 
      1. Rechtsklick aufs Projekt `/Run as/Run Configurations`
      2. Doppelklick auf `Gradle Task` um einen neuen Gradle Task zu erstellen
      3. Gradle Task hinzufügen und `run` nennen
      4. Bei `Working Directory` das aktuelle Projekt auswählen
      5. run
    4. IntelliJ: Im Gradle-Menü rechts auf `<app name>/Tasks/application/run`

## Wenn eine andere Java Version genutzt wird
1. In `build.gradle` den Eintrag `JavaLanguageVersion.of(17)` die Java Version eintragen. Kompatiblität beachten.
