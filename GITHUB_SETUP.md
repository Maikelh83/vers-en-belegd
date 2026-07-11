# Repo op GitHub zetten

Ik heb geen toegang tot je GitHub-account — dit doe je zelf, 5 minuten werk.

## 1. Nieuwe repository aanmaken

1. Ga naar https://github.com/new (inloggen indien nodig).
2. Repository name: `vers-en-belegd` (of `versenbelegd-website`).
3. Zichtbaarheid: Private (of Public als je gratis GitHub Pages wilt gebruiken).
4. Laat "Initialize with README" UIT (deze repo heeft er al een).
5. Klik "Create repository".

## 2. Lokale map koppelen en pushen

```bash
cd pad/naar/vers-en-belegd
git init
git add .
git commit -m "Initial commit: homepage en privacyverklaring"
git branch -M main
git remote add origin https://github.com/JOUW-GEBRUIKERSNAAM/vers-en-belegd.git
git push -u origin main
```

Vervang `JOUW-GEBRUIKERSNAAM` door je eigen GitHub-gebruikersnaam.

Vraagt git om inloggegevens: gebruik een Personal Access Token als wachtwoord (Settings → Developer settings → Personal access tokens), of `gh auth login` / GitHub Desktop.

## 3. Optioneel: GitHub Pages

Als de repo public is: Settings → Pages → Source: branch `main`, map `/ (root)` → Save. Site staat dan op `https://JOUW-GEBRUIKERSNAAM.github.io/vers-en-belegd/`. Voor het echte domein www.versenbelegd.nl blijft je huidige hosting leidend.
