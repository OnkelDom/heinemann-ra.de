# heinemann-ra.de

Statische Website fuer `heinemann-ra.de`.

## Architektur

- Quelle: GitHub Repository `OnkelDom/heinemann-ra.de`
- Branch: `main`
- Zielsystem: Hetzner Webspace per SFTP
- Zielpfad: Domain-Ordner `heinemann-ra.de`
- Deployment: `.github/workflows/deploy.yml`

## Bearbeitung

```bash
vim index.html
vim impressum.html
vim datenschutz.html
vim styles.css
```

Lokale Vorschau:

```bash
python3 -m http.server 8084
```

## Deployment

Automatisch bei Push auf `main`.

Erforderliche Secrets:

```text
HETZNER_HOST
HETZNER_PORT
HETZNER_USER
HETZNER_PASSWORD
HETZNER_TARGET_DIR
```

`HETZNER_TARGET_DIR` ist `heinemann-ra.de`.

## Offene Pruefpunkte

- Impressum berufsrechtlich final gegen Mandantendaten pruefen.
- Datenschutz final gegen tatsaechliche Hosting-/Kontaktprozesse pruefen.
- Telefonnummer, Fax und E-Mail vor Livegang vom Mandanten bestaetigen lassen.
