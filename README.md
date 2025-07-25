# CSS Fonts & Animationen

## Teil 1: Fonts importieren

### Q&A Fragen

**1. Welche Methoden gibt es, um externe Fonts in CSS zu verwenden?**

**2. Was ist der Unterschied zwischen @import und Link-Tag für Fonts?**

**3. Warum sollte man Fallback-Fonts definieren?**

### Multiple Choice

**1. Welcher Code importiert korrekt einen Google Font?**
a) `@import url('https://fonts.google.com/roboto');`
b) `@import url('https://fonts.googleapis.com/css2?family=Roboto');`
c) `<link href="fonts.google.com/roboto" rel="stylesheet">`
d) `font-family: 'Roboto', google;`

**2. Was bedeutet font-display: swap?**
a) Der Font wird sofort ausgetauscht
b) Fallback-Text wird angezeigt bis der Font geladen ist
c) Der Font wird gespiegelt dargestellt
d) Der Font wechselt zwischen zwei Varianten

**3. Welche font-weight Werte sind Standard?**
a) light, normal, heavy
b) 100, 400, 700
c) thin, regular, bold
d) small, medium, large

### Code-Aufgaben Fonts

**Aufgabe 1:** Importiere den Font "Open Sans" von Google Fonts mit den Gewichten 300, 400 und 700.

**Aufgabe 2:** Definiere eine font-family mit Fallbacks für einen Titel.

```css
h1 {
    font-family: _______;
}
```

**Aufgabe 3:** Erstelle eine @font-face Regel für einen lokalen Font namens "MyFont".

## Teil 2: CSS Animationen

### Q&A Fragen

**1. Was ist der Unterschied zwischen transitions und animations?**

**2. Welche Eigenschaften sollte man für Performance nur animieren?**

**3. Was passiert bei animation-fill-mode: forwards?**

### Multiple Choice

**1. Welche transition-timing-function ist am smoothesten?**
a) linear
b) ease
c) ease-in-out
d) steps(5)

**2. Was bedeutet animation-iteration-count: infinite?**
a) Die Animation läuft einmal
b) Die Animation läuft unendlich oft
c) Die Animation läuft 5 mal
d) Die Animation läuft rückwärts

**3. Bei welchem Keyframe-Wert startet eine Animation?**
a) 0% oder from
b) 50%
c) 100% oder to
d) start

### Code-Aufgaben Animationen

**Aufgabe 4:** Erstelle eine einfache Hover-Transition für einen Button.

```css
.button {
    /* Normal state */
}

.button:hover {
    /* Hover state */
}
```

**Aufgabe 5:** Was macht dieser Keyframe-Code?

```css
@keyframes slideIn {
    0% {
        transform: translateX(-100%);
        opacity: 0;
    }
    100% {
        transform: translateX(0);
        opacity: 1;
    }
}
```

**Aufgabe 6:** Vervollständige diese Animation-Regel.

```css
.animated-box {
    animation: _____ _____ _____ _____ _____ _____;
}

/* Parameter: Name, Dauer, Timing, Verzögerung, Wiederholungen, Richtung */
```

**Aufgabe 7:** Erstelle eine Keyframe-Animation die ein Element rotiert und größer macht.

```css
@keyframes _____ {
    
}

.spinning-element {
    animation: _____;
}
```

**Aufgabe 8:** Was ist falsch an diesem Transition-Code?

```css
.box {
    width: 100px;
    height: 100px;
    transition: width 2s ease;
}

.box:hover {
    width: 200px;
    height: 200px;
    background-color: red;
}
```

### Erweiterte Aufgaben

**Aufgabe 9:** Erstelle eine Loading-Animation mit drei Punkten.

**Aufgabe 10:** Erkläre was animation-fill-mode macht und gib Beispiele.

**Aufgabe 11:** Erstelle eine Card die beim Hover umklappt (3D Flip).

**Aufgabe 12:** Performance-Frage: Welche dieser Animationen ist am smoothesten?

a) `transition: left 0.3s ease;`
b) `transition: margin-left 0.3s ease;`
c) `transition: transform 0.3s ease;`
d) `transition: width 0.3s ease;`

### Debugging-Aufgaben

**Aufgabe 13:** Warum funktioniert diese Animation nicht?

```css
.element {
    animation: fadeIn 2s ease-in-out;
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}
```

```html
<div class="element">Text</div>
```

**Aufgabe 14:** Optimiere diese langsame Animation.

```css
/* Langsam: */
@keyframes slideUp {
    0% { top: 100px; }
    100% { top: 0; }
}
```

**Aufgabe 15:** Erstelle eine komplexe Animation die mehrere Eigenschaften über verschiedene Zeitpunkte animiert.

```css
/* Erstelle eine Animation die:
   - 0-25%: Element fährt von links ein
   - 25-50%: Element wird größer
   - 50-75%: Element rotiert
   - 75-100%: Element wird transparent
*/
```

## Bonus: Kombinierte Aufgaben

**Aufgabe 16:** Erstelle eine Webseite mit einem Custom Font und animierten Elementen.

```html
<!DOCTYPE html>
<html>
<head>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* Dein CSS hier */
    </style>
</head>
<body>
    <h1>Animierte Überschrift</h1>
    <div class="card">Hover mich!</div>
</body>
</html>
```
