# @marcelxwilhelm – Link-in-Bio Seite

Eigene Linktree-Alternative, keine externen Abhängigkeiten, kein Build nötig.

## Ordnerstruktur

```
├── index.html      Seiteninhalt (Links, Texte)
├── css/
│   └── style.css   Design (Farben, Layout, Animationen)
└── README.md       diese Anleitung
```

Beim Hochladen zu GitHub genau diese Struktur beibehalten (den `css`-Ordner mit hochladen), sonst findet `index.html` das Stylesheet nicht.

## So bringst du die Seite auf GitHub Pages live

1. Neues Repository auf GitHub anlegen, z. B. `marcelxwilhelm-links` (öffentlich, sonst braucht GitHub Pages einen bezahlten Plan).
2. `index.html` und den kompletten `css`-Ordner ins Repo hochladen (per Weboberfläche: **Add file → Upload files** – Ordner können per Drag & Drop mit hochgeladen werden – oder per Git).
3. Im Repo zu **Settings → Pages** gehen.
4. Unter **Source** die Option **Deploy from a branch** wählen, Branch `main` und Ordner `/ (root)` auswählen, dann **Save**.
5. Nach ca. 1–2 Minuten ist die Seite erreichbar unter:
   `https://<dein-github-username>.github.io/<repo-name>/`

## Eigene Domain (optional)

Falls du z. B. `links.deinedomain.de` nutzen willst:
1. Im Repo eine Datei `CNAME` mit genau der gewünschten Domain als Inhalt anlegen (eine Zeile, ohne `https://`).
2. Beim Domain-Anbieter einen `CNAME`-Eintrag anlegen, der auf `<dein-github-username>.github.io` zeigt.
3. In **Settings → Pages** die Custom Domain eintragen und "Enforce HTTPS" aktivieren, sobald verfügbar.

## Links später ändern

Links/Texte → `index.html` bearbeiten. Farben/Design → `css/style.css` bearbeiten. Beides direkt in der GitHub-Weboberfläche möglich – nach dem Commit aktualisiert sich die Seite automatisch nach kurzer Zeit.
