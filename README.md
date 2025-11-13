# Hau-den-Maulwurf

Ein einfaches Whack-a-Mole Spiel, gebaut mit HTML, CSS und JavaScript.

## Features

- 4 Maulwürfe in Löchern
- Hammer-Cursor zum Treffen der Maulwürfe
- 5 Punkte pro Treffer (normale Maulwürfe)
- Maulwürfe mit Helm: Nicht treffen! Sonst -5 Punkte
- Sammle so viele Punkte wie möglich
- Highscore-System: Dein Rekord wird gespeichert und angezeigt
- 30 Sekunden Zeitlimit
- Maulwürfe erscheinen zufällig (alle 0.5-2 Sekunden)
- Hintergrundmusik während des Spiels
- Verloren-Sound bei Zeitablauf
- Countdown am Anfang (3, 2, 1, Start)
- Neustart und Beenden Buttons am Ende

## Lokale Entwicklung

1. Öffne `index.html` in einem modernen Webbrowser
2. Das Spiel startet automatisch mit einem Countdown

## Deployment auf Netlify

### Option 1: Drag & Drop

1. Gehe zu [Netlify Drop](https://app.netlify.com/drop)
2. Ziehe den gesamten Projektordner in das Drop-Fenster
3. Netlify erstellt automatisch eine URL für dein Spiel

### Option 2: Git Integration

1. Erstelle ein GitHub Repository
2. Lade deinen Code hoch:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin <deine-repo-url>
   git push -u origin main
   ```
3. Gehe zu [Netlify](https://www.netlify.com/)
4. Klicke auf "New site from Git"
5. Wähle dein Repository aus
6. Netlify erkennt automatisch, dass es eine statische Seite ist
7. Klicke auf "Deploy site"

### Option 3: Netlify CLI

1. Installiere die Netlify CLI:
   ```bash
   npm install -g netlify-cli
   ```
2. Logge dich ein:
   ```bash
   netlify login
   ```
3. Deploye das Projekt:
   ```bash
   netlify deploy
   ```
4. Für Production:
   ```bash
   netlify deploy --prod
   ```

## Audio-Dateien hinzufügen (optional)

Falls du eigene Musik und Soundeffekte verwenden möchtest:

1. Füge deine Audio-Dateien zum Projektordner hinzu (z.B. `background-music.mp3` und `lose-sound.mp3`)
2. Öffne `index.html`
3. Finde die Audio-Elemente im HTML:
   ```html
   <audio id="backgroundMusic" loop>
       <source src="background-music.mp3" type="audio/mpeg">
   </audio>
   
   <audio id="loseSound">
       <source src="lose-sound.mp3" type="audio/mpeg">
   </audio>
   ```
4. Entferne die Kommentare und passe die Dateinamen an

## Browser-Kompatibilität

Das Spiel funktioniert in allen modernen Browsern:
- Chrome
- Firefox
- Safari
- Edge

## Technologie

- HTML5
- CSS3 (mit Animationen)
- Vanilla JavaScript (keine Frameworks)

## Lizenz

Dieses Projekt ist für persönliche Zwecke erstellt.
