# TR4C3R Props Creator

Ein professionelles Script zum Platzieren, Bearbeiten und Verwalten von Custom Props auf deinem FiveM Server.

## Features

- Einfache Platzierung von Props mit Freecam-System
- Visuelles Gizmo-System (wie CodeWalker) für präzise Positionierung
- Rotation und Skalierung in Echtzeit
- Automatisches Speichern und Laden von Props
- ESX-Menu Integration
- Sehr gute Performance (0.00ms)
- Props sind über die ganze Map sichtbar

## Installation

1. Lade das Script in deinen `resources` Ordner
2. Füge es zu deiner `server.cfg` hinzu:
   ```
   ensure tr4c3r_propscreator
   ```
3. Stelle sicher, dass ESX installiert ist
4. Starte den Server neu

## Verwendung

### Props erstellen

1. Öffne das Menu mit dem Befehl: `/propsmenu`
2. Wähle "Props erstellen"
3. Wähle ein Prop aus der Liste
4. Du wirst automatisch in den Freecam-Modus versetzt

### Freecam-Steuerung

#### Bewegung
- **W/A/S/D** - Prop vor/zurück/links/rechts bewegen
- **Q/Z** - Prop hoch/runter bewegen

#### Rotation
- **Pfeiltasten** - Prop drehen (Pitch/Yaw)
- **NUM4/NUM6** - Prop rollen (Roll)

#### Größe
- **PageUp/PageDown** - Prop größer/kleiner machen

#### Kamera
- **Maus** - Kamera drehen
- **Mausrad** - Zoom rein/raus
- **Shift** - Alle Bewegungen schneller ausführen

#### Platzierung
- **ENTER** - Prop platzen und speichern
- **X** - Platzierung abbrechen

### Props verwalten

1. Öffne das Menu mit `/propsmenu`
2. Wähle "Props löschen"
3. Wähle ein Prop aus der Liste zum Löschen
   - Oder wähle "Alle löschen" (mit doppelter Bestätigung)

## Props hinzufügen

Um neue Props zum Script hinzuzufügen, bearbeite die `config.lua`:

```lua
Config.Props = {
    {
        name = 'TR4C3R Logo',
        model = 'tr4c3r_logo',
        label = 'TR4C3R Logo'
    },
    {
        name = 'Dein Prop',
        model = 'dein_prop_model',
        label = 'Anzeigename'
    },
}
```

**Wichtig:** Das Prop-Model muss im Spiel verfügbar sein (als Resource oder Map).

## Performance

Das Script ist sehr optimiert und hat eine Performance von **0.00ms**. Props werden mit optimierten LOD-Distanzen geladen, sodass sie über die ganze Map sichtbar sind, ohne Performance-Probleme zu verursachen.

## Technische Details

- Props werden in einer JSON-Datei gespeichert
- Automatisches Laden beim Server-Start
- Synchronisierung mit allen Spielern
- Freecam-System mit präziser Steuerung
- Visuelles Gizmo für bessere Übersicht

## Support

Bei Fragen oder Problemen wende dich an den TR4C3R SERVICE.

