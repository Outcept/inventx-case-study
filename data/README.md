# Data package for builders

All synthetic calls of the case.

All calls are fictional. Names, companies and numbers are invented. There is no real customer or bank data.

| Folder | Content |
|---|---|
| `Audio/` | 60 recordings, WAV, mono, 16 kHz, 16-bit, Swiss German, synthetic voices |
| `Transkript/` | 30 scripts: the dialogue, turn by turn |
| `Skript_mit_Sollbewertung/` | the same 30 dialogues with the expected assessment, its reasoning and the supporting passages |
| `Stichwortliste.json` | preliminary keyword families |

## File names

- `Stufe1_...` level 1: direct keyword calls
- `Stufe2_...` level 2: context pairs, similar calls where only the context decides
- `Stufe3_...` level 3: open cases where the expected assessment is "review"
- Each script exists as two recordings: `K1`/`K3` clean, `K2`/`K4` with noise.

## Expected assessment ("Bearbeitung")

`alarm` = alert, `no_alert` = no alert, `review` = hand over to a human.

## Good to know

- The transcripts are the scripts the recordings were made from, not verified transcriptions.
- Keyword list and expected assessments are test conventions for the sprint, not official rules of Inventx.
- Do not feed file names, scripts or expected assessments into your audio pipeline as hidden hints.

The audio is about 500 MB, so the first clone takes a moment.
