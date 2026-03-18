# 🔐 Login UI Prototype

Responsiver mehrseitiger Login- und Registrierungs-Prototype, gebaut mit purem HTML5 und CSS3. Zeigt einen vollständigen Auth-Flow mit Login, Passwort-Reset und dreistufigem Registrierungsprozess.

---

## 📁 Projektstruktur

```
/
├── index.html              ← Login
├── css/
│   └── stylesheet.css
├── html/
│   ├── forgotpassword.html ← Passwort vergessen
│   ├── register1.html      ← Registrierung Schritt 1: Zugangsdaten
│   ├── register2.html      ← Registrierung Schritt 2: Verifizierung
│   └── register3.html      ← Registrierung Schritt 3: Abschluss
└── images/
```

---

## 🧩 Seitenaufbau

**Login (`index.html`)** – Username, Passwort, „Login speichern"-Checkbox, Submit- und Reset-Button, Links zu Passwort-Reset und Registrierung. Fixierter Aside-Button für Kontakt und Hilfe.

**Passwort vergessen (`forgotpassword.html`)** – Einfaches Formular zur Eingabe des Usernames mit Zurück-Link.

**Registrierung Schritt 1 (`register1.html`)** – Username, Passwort, Geburtstag, Lieblingsfarbe. Fortschrittsbalken bei 30%.

**Registrierung Schritt 2 (`register2.html`)** – Ausweis-Verifizierung via Radio-Buttons (`<fieldset>` + `<legend>`), Foto-Auswahl, Datei-Upload, Nationalitäts-Dropdown. Fortschrittsbalken bei 60%.

**Registrierung Schritt 3 (`register3.html`)** – Herkunfts-Dropdown, AGB-Checkbox, Abschluss-Button mit Bestätigungs-Alert. Fortschrittsbalken bei 100%.

---

## 📱 Responsive

| Breakpoint | Änderungen |
|---|---|
| `≤ 540px` | Padding reduziert, Box nutzt volle Breite, Aside ausgeblendet |

Das Layout ist durch `max-width: 500px` + `margin: auto` auf dem Main-Container grundsätzlich mobile-tauglich.

---

## 🛠️ Technologien

- **HTML5** – semantisches Markup, `<fieldset>`, `<legend>`, `<progress>`, `autocomplete`-Attribute
- **CSS3** – Custom Properties, `:focus-visible`, `:valid`/`:invalid`, `accent-color`, `@media (prefers-reduced-motion)`
- **Kein Framework**, kein npm

---

## 📌 Hinweise

Dieser Prototype ist ein reines UI/UX-Demo ohne Backend-Anbindung. Formulare senden keine echten Daten – der Abschluss-Button in Schritt 3 zeigt einen Browser-Alert als Platzhalter.
