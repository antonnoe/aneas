---
name: aneas
description: Opstart voor het ANEAS-project, het voorbeeldontwerp van de nieuwe website van de Nederlandse Vereniging voor Onderlinge Hulpverlening (repo antonnoe/aneas, GitHub Pages). Gebruik deze skill altijd wanneer Anton "Aneas" typt of het heeft over de ANEAS-site, het ANEAS-logo, de hero of header, de mobiele weergave, V09, de beheerfunctie (titel, inleiding en pdf toevoegen), Pages CMS of Decap, of de keuze tussen Next.js, PHP en Joomla voor ANEAS, ook als hij de skill niet bij naam noemt.
---

# ANEAS opstarten

Doel: Anton hoeft niets uit te leggen. Lees de actuele stand, vat die kort samen en vraag waar hij mee verder wil.

## Stappen
1. Haal CLAUDE.md op uit de repo antonnoe/aneas, branch main. In een sessie op die repo: lees het bestand direct. Elders: gebruik de GitHub-tool (get_file_contents) of vraag Anton om het bestand te plakken. CLAUDE.md is de bron van de waarheid; de samenvatting hieronder veroudert.
2. Vat de stand samen in hoogstens vijf regels: wat staat er live, wat is besloten, wat is open.
3. Vraag waar hij mee verder wil. Noem de open vragen uit CLAUDE.md alleen als ze voor die keuze nodig zijn.
4. Bij bouwwerk: noem het aanbevolen model (Sonnet voor bouw, Opus of Fable alleen voor architectuur, audit en beveiligingscontrole van uploads en CMS-rechten).

## Samenvatting (kan achterlopen)
- Eén pagina index.html op GitHub Pages (main), blauw hero-veld met wit logo, mobiel getest op 360 px.
- V09: hele site, NL en FR, Next.js als statische export, beheerder voegt titel + korte inleiding + pdf toe via Pages CMS of Decap (GitHub-inlog). Supabase en Joomla zijn afgevallen, PHP op de hosting is de terugvaloptie.
- Pro deo: geen vaste kosten opbouwen.

## Werkafspraken van Anton
- Direct op main werken, tenzij hij anders zegt.
- Eerst leveren met de aanname zichtbaar erbij; alleen doorvragen als een verkeerde aanname het resultaat onbruikbaar maakt.
- Zakelijk, Nederlands, geen lange streepjes, niet "ecosysteem" (zeg "netwerk van platforms").
- Harde gegevens verifiëren tegen de primaire bron. aneas.fr is vanuit Claude Code geblokkeerd, dus vraag Anton om bestanden of gegevens via de repo aan te leveren.
