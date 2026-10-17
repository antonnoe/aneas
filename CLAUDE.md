# ANEAS (voorbeeldontwerp nieuwe website)

Trigger: Anton typt "Aneas" in een sessie op deze repo. Lees dit bestand en vat in enkele regels de stand samen, daarna vragen waar hij mee verder wil.

## Context
- Repo antonnoe/aneas, direct op main werken, GitHub Pages staat aan op main (verwachte URL https://antonnoe.github.io/aneas/, niet getest).
- Opdracht is pro deo voor ANEAS (Nederlandse Vereniging voor Onderlinge Hulpverlening, Association Néerlandaise d'Entr'Aide Sociale, sinds 1885). Geen vaste kosten opbouwen.
- Het huidige aneas.fr lijkt Joomla (pad /templates/aneas/). Anton wil geen Joomla.

## Stand (V08, losse index.html)
- index.html: één pagina, eigen CSS in de head, kleuren via :root (blauw #1f3a5f, oranje #d9692b).
- Mock-up-balk bovenaan (regel met class="mock"), verwijderen voor livegang.
- Header: tekstlogo ANEAS met ondertitel. Hero (blauw veld): tekst links, logo rechts.
- Logo's: aneas-transp.png (origineel, grijze letters), aneas-logo-licht.webp (afgeleid, witte letters, voor op blauw: grijs had te weinig contrast). Banner is verwijderd (staat in git-geschiedenis, commit f39aee4 voor het PNG-origineel).
- Mobiel getest op 360 px: menu breekt niet af, header niet sticky onder 760 px, knoppen volle breedte. Alleen in headless Chromium bekeken, niet op een echte telefoon.

## Gekozen richting voor V09 (nog niet gebouwd)
- Hele site bouwen, NL en FR.
- Beheerder moet eenvoudig kunnen toevoegen: titel + korte inleiding + pdf.
- Voorkeur Anton: Next.js. Advies: Next.js als statische export (output: 'export'), geen draaiende server. Inhoud als bestanden in de repo, formulier voor de beheerder via Pages CMS of Decap CMS (beheerder logt in met GitHub-account).
- Afgevallen: Supabase-beheerpagina (mogelijke kosten), Joomla (Anton wil het niet). Terugvaloptie als de beheerder geen GitHub wil: kleine PHP-beheerpagina op de hosting van aneas.fr met wachtwoord.
- Open vragen: lijst van pagina's en talen (sitemap aneas.fr), waar de site uiteindelijk staat (GitHub Pages of hosting aneas.fr, PHP-versie, schrijfbare map), aantal beheerders, of verwijderen en herordenen nodig is, of de beheerder GitHub-inlog accepteert. Vercel Hobby is bedoeld voor niet-commercieel gebruik, voor een vereniging nog nakijken.

## Beperkingen van de omgeving
- Netwerk geblokkeerd voor aneas.fr en chatgpt.com (proxy 403). Bestanden dus via de repo aanleveren.
- Preview kan met /opt/pw-browsers/chromium-1194/chrome-linux/chrome headless, mobiel nabootsen via een iframe van 360 px (headless gaat niet smaller dan ca. 500 px).

## Werkafspraken
- Model noemen: Sonnet voor bouw, Opus of Fable alleen voor architectuur, audit en beveiligingscontrole (uploads, CMS-rechten).
- Antwoorden zakelijk, Nederlands, geen lange streepjes, niet "ecosysteem" maar "netwerk van platforms".
