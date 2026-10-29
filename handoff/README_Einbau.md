# SANNIS Pillar Page Bio-Leinöl · Einbau (Vorlage für Themenseiten)

Stand 29.10.2026 · Quelle: SANNIS Style Guide 2026, Kapitel 15 „Vorlage Pillar Page“. Ansprechpartner: Manuel Kössler (SANNIS Marketing).

## Was das ist
Die komplette Pillar Page „Bio-Leinöl“ (Prototyp v1.9) als **ein Elementor-HTML-Widget**: Markup, CSS und Skript in einer Datei.
CSS ist unter `.sn-pillar` gekapselt, Header und Footer von sannis.at bleiben unverändert. Aufbau = die Regel für jede SANNIS-Themenseite
(Hero-Statement, Kapitelfolge im Farbrhythmus, Zahlen-Kacheln ohne Preise, Love Breaks, Herkunft, FAQ, „Ein Lächeln…“, Weg in den Shop).

## Dateien
| Datei | Zweck |
|---|---|
| `SANNIS_PillarPage_Bio-Leinoel_Elementor.html` | Das Widget, komplett kopierbar (ca. 78 KB) |
| `assets/pillar/` | Alle Bilder, Video und OG-Bild der Seite (32 Referenzen im Code) |

## Einbau (ca. 30 Minuten)
1. **Bilder hochladen:** Ordner `assets/pillar/` so auf den Server legen, dass die Dateien unter `https://sannis.at/wp-content/uploads/sannis-brand/pillar/…` erreichbar sind
   (z. B. per FTP nach `wp-content/uploads/sannis-brand/pillar/`). Anderer Pfad? Dann im Code alle `https://sannis.at/wp-content/uploads/sannis-brand/pillar` ersetzen.
2. **Seite anlegen:** WordPress → Seiten → Neu. Typ **Seite** (kein Beitrag), Slug `/leinoel/`, Elementor-Template **Full Width**.
3. **Widget:** In Elementor EIN HTML-Widget auf die Seite ziehen, den Inhalt der Datei komplett hineinkopieren (Cmd+A/Cmd+V). Nichts weglassen, keine `on…`-Attribute ergänzen.
4. **Rank Math:** Title „Bio-Leinöl aus Vorarlberg: frisch gepresst in den Alpen | SANNIS“, Meta wie im Kommentar am Dateianfang, OG-Bild aus `assets/pillar/`.
5. **Cache:** WP Rocket Cache leeren.
6. **Prüfen (mobil zuerst):** iPhone 393 px ohne Überbreite, Hero-Statement, Love Breaks, FAQ-Akkordeon, Buttons in den Shop. Dann Desktop 1440 px.
7. **Go-live erst nach Freigabe** (Harald Klüh, Frank Nessler); bis dahin „noindex“ oder Entwurf.

## Schrift
Die Seite lädt die Schriften über Google Fonts (Link am Dateianfang). Headlines im Guide = ITC Avant Garde Gothic Pro (Lizenz vorhanden);
sobald die Webfont-Dateien da sind, Google-Fonts-Link gegen `@font-face` auf die eigenen Dateien tauschen (siehe Style Guide Kap. 03).

## Regeln
- Firewall-sicher: kein HTML in JS-Strings, keine `on…`-Attribute, keine externen Skripte außer dem Google-Fonts-Link, kein Base64.
- Keine Preise auf der Pillar (stehen im Shop), deutsche Sublines, keine englischen Echo-Zeilen.
- Neue Themenseite = Content-Brief nach dem Muster `CONTENT-BRIEF_Pillar_Bio-Leinoel_v1.md`, dann die Kapitelfolge aus Style Guide Kap. 08 füllen.
