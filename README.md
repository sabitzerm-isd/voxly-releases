# Voxly — Releases

Voxly ist eine Windows-Tray-App für **Push-to-Talk Sprach-zu-Text-Diktat** —
hält den Hotkey, sprich, lass los, der transkribierte Text landet sofort
im fokussierten Fenster.

- Lokale Transkription via Whisper.net (kein Cloud-Upload des Audios)
- Optional KI-Polish über Anthropic Claude (Pro/Max Abo oder API-Key)
- Selection-Edit: markierten Text per Sprach-Anweisung umschreiben
- Voll lokalisiert (DE / EN / IT / FR)

---

## 📥 Direkt-Download (immer neueste Version)

**Stabiler Link — kannst du an Kollegen weitergeben:**

👉 **<https://github.com/sabitzerm-isd/voxly-releases/releases/latest/download/Voxly-Setup.exe>**

Dieser Link zeigt automatisch immer auf den aktuellsten Release. Beim Klick
wird `Voxly-Setup.exe` (~200 MB, self-contained mit .NET 8 + GPU-Runtimes)
heruntergeladen.

### Installation in 3 Schritten

1. **Voxly-Setup.exe** herunterladen (Link oben)
2. Doppelklick → Setup-Wizard. Bei „Whisper-Modell wählen" am besten
   **small (~470 MB)** mit aktivierter GPU — guter Sweet-Spot
3. Nach Install startet Voxly automatisch. Tray-Icon (blaues Mikrofon)
   rechts unten

### Erst-Konfiguration

- **Tray-Rechtsklick → Einstellungen → Hotkey** — Default ist `Links-Alt`,
  kannst du auf deine gewünschte Taste umstellen
- **STT-Tab:** Modell + GPU-Beschleunigung prüfen
- **LLM-Tab (optional):** für „KI-poliert" oder „Selection-Edit" einen
  Claude-Backend wählen (Claude Code Pro/Max-Abo ODER eigener Anthropic-API-Key)

---

## 🔄 Auto-Update

Voxly checkt automatisch ~10 Sekunden nach Start ob eine neue Version
verfügbar ist. Falls ja: Tray-Toast + persistenter Menü-Eintrag „Update verfügbar".
Du kannst auch manuell prüfen: Tray-Rechtsklick → „Auf Updates prüfen…".

Updates werden silent heruntergeladen, die App startet danach automatisch
neu — deine Einstellungen bleiben erhalten.

---

## 📚 Hilfe & Dokumentation

- **In-App-Hilfe:** Tray-Rechtsklick → „Hilfe / Anleitung…" öffnet eine
  interaktive HTML-Hilfe mit allen Features + FAQ + Lizenzen
- **Wunsch / Bug:** Tray-Rechtsklick → „Wunsch / Feedback schicken…"

---

## 📋 Versionierter Direkt-Link

Wenn du eine bestimmte Version verteilst (z. B. wenn du sicherstellen willst
dass alle die gleiche Version haben), dann:

```
https://github.com/sabitzerm-isd/voxly-releases/releases/download/v<version>/Voxly-Setup-<version>.exe
```

Beispiel: <https://github.com/sabitzerm-isd/voxly-releases/releases/download/v0.1.34/Voxly-Setup-0.1.34.exe>

---

## 🛡️ Systemanforderungen

- Windows 10 (Build 1809+) oder Windows 11
- 64-bit x64
- ~250 MB Disk-Space für die App (mit GPU-Runtimes), zusätzlich 75 MB–3 GB
  für das Whisper-Modell (je nach Größe)
- Mikrofon
- Optional: NVIDIA / AMD / Intel GPU für deutlich schnellere Transkription

---

## ⚖️ Lizenz

Voxly ist frei nutzbar inkl. kommerziell. Verwendet diverse Open-Source-
Komponenten (MIT / Apache 2.0 / CPOL für Hardcodet.NotifyIcon) — komplette
Lizenz-Übersicht in der In-App-Hilfe und in der mitgelieferten
`LICENSE.txt`.
