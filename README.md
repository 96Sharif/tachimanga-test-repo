# My Tachimanga Test Repo

Ein minimales Extension-Repository zum Testen mit Tachimanga / Mihon / Tachiyomi-kompatiblen Apps.
Es hostet eine `repo/index.min.json` mit einem Beispiel-Eintrag, damit du den kompletten Ablauf
(GitHub hosten → Raw-URL → in Tachimanga eintragen) einmal sauber nachvollziehen kannst.

## Was ist das hier?

Ein Extension-Repository ist im Kern eine einzelne JSON-Datei (`index.min.json`), die als Array
beschreibt, welche Extensions verfügbar sind. Tachimanga lädt diese Datei über eine URL und zeigt
die darin gelisteten Extensions an. Die eigentlichen `.apk`-Dateien werden separat referenziert.

## GitHub: Schritt für Schritt

1. Auf https://github.com einloggen und oben rechts auf **New repository** klicken.
2. Repository-Namen vergeben, z. B. `my-tachimanga-repo`. Sichtbarkeit **Public** wählen
   (sonst ist die Raw-URL nicht ohne Token erreichbar). Mit **Create repository** bestätigen.
3. Im neuen Repo auf **Add file → Create new file** klicken.
4. Als Dateinamen `repo/index.min.json` eingeben. Durch das `/` legt GitHub automatisch den
   Ordner `repo` an. Den JSON-Inhalt (siehe unten) einfügen und unten **Commit changes** klicken.
5. Optional denselben Schritt für `apks/comick-test-v1.apk` wiederholen, falls du eine echte
   APK hochladen willst (per **Add file → Upload files**).
6. Diese README ebenfalls als `README.md` im Hauptverzeichnis anlegen.

## Die Raw-URL ermitteln

1. Im Repo zur Datei `repo/index.min.json` navigieren.
2. Oben rechts den Button **Raw** anklicken.
3. Die URL aus der Adresszeile kopieren. Sie hat dieses Muster:
