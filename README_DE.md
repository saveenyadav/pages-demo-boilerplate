# DCI Boilerplate

Ein Projekt-Boilerplate mit Sass-Unterstützung

- Entwicklungs-Server betrieben von [parcel](https://parceljs.org/) mit Sass-Kompilierung und Auto-Reload.

## Los geht's

- [Einrichtung](#einrichtung)
- [Nützliche Befehle](#nützliche-befehle)
- [Projektstruktur](#projektstruktur)
- [Danksagungen](#danksagungen)

## Einrichtung

1. Klone dieses Repository in einen neuen Projektordner

2. Lösche die Git-Historie des Boilerplates, um sicherzustellen, dass die Projektgeschichte nur deine Commits enthält

   ```
   cd <Projektordner>
   rm -rf .git
   ```

3. Bearbeite `src/index.html`, vielleicht füge den Namen deines Projekts hinzu

4. Starte ein neues Git-Repository und mache einen initialen Commit. Das stellt sicher, dass du an deinem Projekt mit Git arbeiten kannst.

   ```
   git init
   git add . && git commit -m "Initial commit"
   ```

5. Installiere die Abhängigkeiten

   ```
   npm install
   ```

6. Viel Spaß beim Coden!

## Nützliche Befehle

### Entwicklung

Starte den **parcel-live-server** und fang an zu coden!

```
npm start
```

### Produktion

Kompiliere den Quellcode aus **src** und erstelle ein optimiertes Produktions-Bundle im **dist**-Ordner, bereit für das **Deployment**.

```
npm run build
```

## Projektstruktur

Jedes mit diesem Boilerplate erstellte Projekt wird der untenstehenden Struktur folgen:

```
Projekt
│   README.md
│   package.json
|   package-lock.json
└───src
│   │   index.html
│   |   sassy-css.scss
|   └───images
└───dist
```

### `README.md`

Das README sollte eine kurze Beschreibung deines Projekts enthalten, fühle dich frei, diese Anleitung zu löschen oder umzubenennen, um deine eigene Beschreibung hinzuzufügen.

### `package.json` & `package-lock.json`

Diese Dateien enthalten verschiedene Informationen über dein Projekt und seine Abhängigkeiten sowie nützliche Skripte, die dir im Entwicklungsprozess helfen.

### `src` & `index.html`

Der `src`-Ordner enthält alle Dateien, die du deiner Website hinzufügen möchtest. **Dies ist der Hauptordner, in dem du arbeiten wirst**.

`index.html` ist die Hauptseite deiner Website, an der du arbeiten wirst. Füge gerne direkt im `src`-Ordner neue `html`-Seiten hinzu, die du erstellst.

### `main.scss`

Die Datei `main.scss` wird jeglichen `scss`-Code enthalten, den du schreibst.

### `dist`

Der `dist`-Ordner wird automatisch generiert, wann immer du das Start- oder Build-Skript ausführst:

```bash
npm start
npm run build
```

`npm start` wird ein nicht optimiertes Bundle erstellen und `npm run build` wird ein optimiertes Produktions-Bundle erstellen, bereit zum Deployment. Es wird von der `git`-Verfolgung ausgeschlossen, da es nicht üblich ist, kompilierten Code in einem Entwicklungsprojekt einzuschließen.
