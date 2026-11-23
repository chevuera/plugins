# Che Lyric Studio

Een Claude Code-plugin met één skill, `lyrics`, die de **Che Elite Lyric Editor** en **De Apocalyptische Woordarchitect** samenvoegt. Je kiest zelf in welke stijl er geschreven wordt.

## Stijlen

| Stijl | Wat het is |
|---|---|
| `CHE` | Je eigen stem: autobiografisch, rauw, technisch multi-rijm, elk genre. |
| `APOCALYPS` | Duistere, dystopische underground-rap met kosmische en religieuze beeldtaal. |
| `PUNCHLINE` | Woordspel, dubbele bodems, setups en twists. |
| `LIED` | Beeldschrijvend: bachata, Cubaanse trova, liefdeslied, ballad. |
| Mix | Bv. `CHE + APOCALYPS`: de eerste stijl is de hoofdstijl. |

Noem je geen stijl, dan vraagt Claude eerst welke je wilt. De keuze blijft gelden tot je een andere noemt.

## Gebruik

```
/che-lyric-studio:lyrics apocalyps 16 bars over een stad die haar eigen naam vergeet
/che-lyric-studio:lyrics STIJL: CHE + APOCALYPS schrijf een track over ...
/che-lyric-studio:lyrics STIJL: LIED bachata over afscheid op het vliegveld
```

Of gewoon in gewone taal ("schrijf een hook in mijn eigen stijl"); de skill wordt dan automatisch geladen.

Commando's: `STIJL:`, `STIJLEN`, `GO`, `16 BARS`, `MAX N TEKENS`, `ALLEEN SONGTEKST`, `NIEUWE KENNIS:`, `TWEE ONAFHANKELIJKE TRACKS`, `CONTROLEER ZONDER HERSCHRIJVEN`, `TWEEDE MENING`, `FUCKING METAFOREN`, `EIGEN STIJL`, plus de modi STRENG en KANKERSTRENG.

## Stijlgeheugen

De skill leest en werkt `che-stijlgeheugen.md` bij: in je claude.ai-project (`claude/che-stijlgeheugen.md`) als dat beschikbaar is, anders als bestand in de werkmap. Sjabloon: `skills/lyrics/references/stijlgeheugen-sjabloon.md`.

## Installeren

```
/plugin marketplace add chevuera/plugins
/plugin install che-lyric-studio@cursor-plugins
```

## Inhoud

```
che-lyric-studio/
├── .claude-plugin/plugin.json
└── skills/lyrics/
    ├── SKILL.md                      stijlmenu, vaste regels, gedeeld vakmanschap
    └── references/
        ├── stijl-che.md              CHE
        ├── stijl-apocalyps.md        APOCALYPS
        ├── stijl-punchline.md        PUNCHLINE
        ├── stijl-beeldschrijvend.md  LIED (basis)
        ├── stijl-bachata.md          LIED: bachata
        ├── stijl-trova.md            LIED: trova
        ├── beeldbank-bachata.md
        ├── woordspel.md
        ├── rijm-en-flow.md
        ├── rijmbank.md
        ├── suno-v6-database.md
        ├── cross-model-review.md
        └── stijlgeheugen-sjabloon.md
```
