# Praktikumsbericht – Julius Lindenlaub

Statische One-Pager Website als Abgabe für den Praktikumsbericht.

## Deployment (GitHub Pages)

1. Erstelle ein neues GitHub Repository: github.com → New → Name: `praktikumsbericht` → **Public** → Create
2. Füge das Remote hinzu und pushe:
   ```bash
   git remote add origin https://github.com/DEIN-USERNAME/praktikumsbericht.git
   git branch -M main
   git push -u origin main
   ```
3. Aktiviere GitHub Pages: Repository → Settings → Pages → Source: `Deploy from a branch` → Branch: `main`, Folder: `/(root)` → Save
4. Nach 1–2 Minuten erreichbar unter: `https://DEIN-USERNAME.github.io/praktikumsbericht`

## Inhalt befüllen

### YouTube Video-IDs
In `main.html` die Platzhalter `[VIDEO_ID_X]` ersetzen:
- Woche 1–4 (Zeile ~79): `[VIDEO_ID_1]` → YouTube-URL: `youtube.com/watch?v=XXXXX` → ID = `XXXXX`
- Woche 5–8 (Zeile ~95): `[VIDEO_ID_2]` → ID eintragen
- Woche 9–12 (Zeile ~111): `[VIDEO_ID_3]` → ID eintragen

Ersetze den ganzen `<div class="video-embed">` Platzhalter-Block mit:
```html
<div class="video-embed">
  <iframe
    src="https://www.youtube.com/embed/DEINE_VIDEO_ID"
    title="Recap Woche X–X"
    loading="lazy"
    allowfullscreen
  ></iframe>
</div>
```

### Optionale zusätzliche Videos (max. 2)
In `main.html` die auskommentierten `<!-- ... -->` Blöcke einkommentieren und `[DEMO_VIDEO_ID]` bzw. `[FAZIT_VIDEO_ID]` ersetzen.

### Screenshots
- Screenshots in `assets/screenshots/` ablegen (z.B. `w1-gramenz-briefing.png`)
- In `main.html` die `<img>`-Tags in den `.screenshot-row` Divs einkommentieren und Pfade anpassen

### Texte
- Alle `<!-- Eigene ... -->` Kommentare in `main.html` durch echten Inhalt ersetzen
- `[Studiengang]` im Footer ersetzen

## Checkliste vor Abgabe
- [ ] Alle `<!-- ... -->` Textkommentare durch echten Inhalt ersetzt
- [ ] Alle 3 YouTube Recap-Video-IDs eingesetzt (Woche 1–4, 5–8, 9–12)
- [ ] Optional: Demo- und/oder Fazit-Video eingebaut (max. 2)
- [ ] Screenshots hochgeladen und verlinkt
- [ ] `[Studiengang]` im Footer eingetragen
- [ ] Zugangscode geändert (falls gewünscht)
- [ ] Abgabe-URL + Code an Betreuer weitergegeben
