# BooBeats

Een muziekbibliotheek voor DJ's die op je eigen computer draait. Geen
account, geen cloud, geen abonnement.

> BooBeats heette eerst **MuziekHub**. Na het installeren zie je die naam
> hier en daar nog terug, zoals in de map waar hij staat; het is dezelfde app.

- **Overzicht:** al je muziek op één plek, met BPM, toonsoort (Camelot),
  genres, labels en sterren.
- **Opschonen:** dubbele nummers vinden, slechte kwaliteit verbeteren en
  nep-lossless herkennen.
- **Playlists en sets:** playlists maken, harmonische mix-tips krijgen en een
  set laten samenstellen.
- **Rekordbox:** een koppeling die je bibliotheek naar Rekordbox stuurt.
- **Binnenhalen:** muziek ophalen van je eigen mappen en USB-sticks, of met je
  eigen account van YouTube, SoundCloud en Soulseek.
- **Volglijsten:** de Spotify-lijst van iemand anders volgen. Je luistert
  eerst het fragment en houdt alleen wat je goed vindt.

## Downloaden

Ga naar **[de nieuwste versie](../../releases/latest)** en kies het bestand
voor jouw computer:

| Jouw computer | Bestand |
|---|---|
| Windows | `BooBeats-…-setup.exe` |
| Mac met Apple Silicon (M1, M2, M3, M4) | `BooBeats-…-mac.dmg` |
| Mac met Intel (grofweg 2020 en eerder) | `BooBeats-…-mac-intel.dmg` |

Liever geen installer op Windows? `BooBeats-…-windows.zip` werkt ook, zie
hieronder. Staat de versie voor jouw computer er nog niet bij, dan komt die
eraan. De bestanden `…-update.zip` en `update.json` heb je niet nodig; die
gebruikt BooBeats zelf om bij te werken.

Je hoeft niets anders te installeren: Python, ffmpeg en de rest zitten al in
de download.

## Installeren op Windows

1. Download `BooBeats-…-setup.exe` en dubbelklik erop. Zegt je browser dat
   het bestand *"niet vaak wordt gedownload"*, kies dan **Behouden** (in Edge
   onder de drie puntjes **⋯**, daarna **Meer weergeven** en
   **Toch behouden**).
2. Zegt Windows *"Windows heeft uw pc beveiligd"*? Klik op
   **Meer informatie** en daarna op **Toch uitvoeren**.
3. Klik op **Volgende** en **Installeren**. Een beheerderswachtwoord is niet
   nodig. BooBeats en BooBeats Mini komen in het Startmenu en, als je dat
   aanvinkt, op je bureaublad.

Verwijderen gaat via **Instellingen > Apps**. Je bibliotheek, playlists en
downloads blijven dan staan.

**Liever de zip?** Rechtsklik hem, kies **Alles uitpakken** naar een vaste
plek (niet de map Downloads) en dubbelklik in de uitgepakte map op
**MuziekHub.vbs**. Laat Verkenner de extensies niet zien, neem dan de
"MuziekHub" met het blauwe pictogram.

## Installeren op de Mac

> Tot en met versie 1.5.0 heet de app op de Mac nog **MuziekHub**. Heb je
> zo'n versie, lees dan MuziekHub waar hieronder BooBeats staat.

1. Dubbelklik op het `.dmg`-bestand en sleep **BooBeats** op het mapje
   **Programma's** dat ernaast staat. Staat daar nog een oude **MuziekHub**?
   Gooi die weg: dat is dezelfde app onder zijn oude naam. Je muziek en
   instellingen blijven bewaard.
2. Open **Programma's** en dubbelklik daar BooBeats. De eerste keer zegt je
   Mac dat Apple niet kon controleren of BooBeats vrij is van malware. Klik op
   **Gereed** (Engels: *Done*; op een oudere Mac: *OK*). Niet op
   **Verplaats naar prullenmand**, dan gooi je de app weg.
3. Open **Systeeminstellingen > Privacy en beveiliging**. Stond
   Systeeminstellingen al open? Sluit het dan eerst helemaal af met **Cmd+Q**
   en open het opnieuw, anders staat de knop er nog niet.
4. Scroll naar het kopje **Beveiliging**. Daar staat *"BooBeats is
   geblokkeerd om je Mac te beschermen"*. Klik ernaast op **Open toch**
   (Engels: *Open Anyway*). Die knop blijft ongeveer een uur staan; is hij
   weg, dubbelklik BooBeats dan nog een keer.
5. Je Mac vraagt nog een keer of je het zeker weet. Kies weer **Open toch** en
   bevestig met Touch ID of je wachtwoord. Daarna onthoudt je Mac het.

Zegt je Mac *"BooBeats is beschadigd en kan niet worden geopend"*? Dat is
dezelfde beveiliging, strenger afgesteld. Open **Terminal** (Spotlight, typ
"Terminal"), plak deze regel en druk op Enter:

```
xattr -dr com.apple.quarantine /Applications/BooBeats.app
```

## Waarom die waarschuwing?

BooBeats is niet digitaal ondertekend. Zo'n handtekening kost per jaar geld
bij Microsoft en Apple. Daarom vragen je browser en je computer één keer of je
het vertrouwt.

## De eerste keer

Een welkomstscherm helpt je in drie stappen: je muziekmap kiezen, Soulseek
koppelen (mag je overslaan) en de koppeling met Rekordbox. Daarna bepaalt
BooBeats op de achtergrond van elk nummer de BPM en de toonsoort.

### Tip: maak een Soulseek-account

Het werkt zonder, maar met een Soulseek-account haal je veel meer uit
BooBeats. Op Soulseek vind je de meeste nummers in goede kwaliteit (lossless
of 320 kbps), en alleen dan kan BooBeats slechte versies in je bibliotheek
vanzelf door betere vervangen.

Aanmelden hoeft niet apart: verzin in het welkomstscherm een gebruikersnaam
en wachtwoord. Is de naam nog vrij, dan wordt hij bij de eerste keer inloggen
jouw account. Onthoud het wachtwoord goed, want opvragen kan niet. Gebruik je
SoulseekQt al, vul dan dat account in en sluit SoulseekQt af: een account kan
maar op één plek tegelijk online zijn.

## Bijwerken

Je hoeft hier niet terug te komen. BooBeats kijkt bij elke start, en daarna
elke paar uur, of er een nieuwe versie is. Dan staat onderin de zijbalk **↑ Versie … is er**, en
één klik werkt hem bij. Je muziek, bibliotheek en instellingen blijven
gewoon staan. Had je nog MuziekHub, dan word je met dezelfde knop BooBeats.

## Goed om te weten

BooBeats levert zelf geen muziek en heeft geen eigen account. Het is
gereedschap voor je eigen bibliotheek, net als Rekordbox. Wat je ermee
downloadt, is je eigen verantwoordelijkheid. Spotify-links gebruik je alleen
om een tracklijst over te nemen.

In de download zitten ffmpeg, yt-dlp en slskd, met hun licenties in de map
`LICENTIES`.
