## Part 1: Fixed Film Decisions

**Historical period:** Denmark around 1600, the time the play was written. Kronborg Castle, the model for Elsinore, was rebuilt in Dutch Renaissance style between 1574 and 1585, and the film shows this castle.

- **Costume:** fitted doublets, padded trunk hose or breeches with woollen hose, ruffs or small linen collars, and wool cloaks. The queen wears a pearl-edged French hood. Guards wear leather jerkins and wool cloaks.
- **Weapons:** partisan spears and morion helmets for the guards, rapiers with swept steel hilts for the nobles, and full plate armour only for the ghost.
- **Architecture:** a sandstone castle with green copper roofs and spires, earthen and stone ramparts facing the sea, long halls with leaded windows, large wall tapestries, stone floors, and oak doors bound with iron.
- **Light sources:** tallow and wax candles, horn and oil lanterns, torches, fireplaces, the foundry furnace, moonlight, and overcast daylight through leaded windows.
- **Exceptions:** in the shots, the ghost is faintly translucent with a cold, sourceless glow. The flashbacks (the orchard and Yorick) have a soft golden, slightly faded light.

**Fixed style string:**

```
Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge
```

**Location Looks:**

|Location|Scenes|Base light|Palette|
|---|---|---|---|
|Castle ramparts at night|1, 3, end of 12|Cold moonlight through sea mist, flickering lantern light|`#0B1A2A` `#2E4A62` `#A9C1D3` `#E6EEF2`|
|Cannon foundry|1|Harsh orange furnace glow in a smoky space|`#120A06` `#7A2E0E` `#E8731C` `#FFC56B`|
|Ramparts at dawn|1, 3|Blue-hour dawn, thin mist, the first warm line on the horizon|`#1B2735` `#4F6A86` `#C9B79C` `#F2E6D0`|
|Great hall at the celebration|2|Warm torch and candelabra light on gold and red velvet|`#1A0F0A` `#6E2A1A` `#C99A4A` `#EEDFC2`|
|Royal orchard, memory|3, 11|Hazy golden afternoon, slightly faded like a memory|`#3E3A22` `#7D7A45` `#C9B57A` `#EFE3BF`|
|Galleries and great hall by day|4, 9, 12|Grey northern daylight through leaded windows, cold stone, dark oak|`#2B2B2E` `#5C5A55` `#A39E93` `#D9D3C7`|
|Players' hall by candlelight|4|Warm candle and torch light in a dark hall, amber shadows|`#140C07` `#5E3A1C` `#C98A3E` `#F4D9A6`|
|Quiet hall|5|Cool overcast light from one tall window, pale stone and faded tapestry|`#1F2226` `#4A4E52` `#8F948F` `#D6D2C4`|
|Soliloquy vision|5|Cold dreamlike darkness, soft mist, almost monochrome|`#0E1418` `#27353F` `#6B7C86` `#C5CCD0`|
|Play hall|6|Torchlight at night, warm amber on red tapestries|`#120806` `#5A1E14` `#C8742E` `#F5D7A0`|
|Chapel|7|A single altar candle in a cold stone chapel|`#0D0B0A` `#3B2A1E` `#9C6B3A` `#E8C88F`|
|Queen's chamber|8|Candle and firelight, red and gold; a cold light when the ghost appears|`#0F0807` `#4A1A1C` `#A8552E` `#EBC79A`|
|Churchyard|9, 11|Flat overcast light, wet earth and grey stone, muted colours|`#1A1C1D` `#45494A` `#8A8F8C` `#CFD3CF`|
|King's private room|10|A dark oak room at night, candles on the table, olive and brass tones|`#0B0D0B` `#2E3A2C` `#8A7A4A` `#D9C79A`|
|Sea and shore|9, 10|Stormy grey sea and cold dawn|`#0C1416` `#2C4246` `#6F8A86` `#D8E0D8`|
|Brook and willow|10|Green-gold morning, mist on the water, dreamlike calm|`#1F2A1C` `#4E6B3E` `#A8B77A` `#EEF0D8`|
|Hall after the deaths|12|The hall drained of warmth, cold blue-grey light like the night of scene 1|`#101418` `#2F3A44` `#7E8A92` `#D6DCE0`|

**Sheet format:** follows `Instructions/Instructions-Character-Sheet.md`. Every image has two rows: a front-facing close-up on top and a front-facing full body below. The character's name in English is written under each column.

- **Type A:** one character seen in several ages or costumes; all states in one image, one state per column. With more than three states, the states are split over several images, and the main state is repeated as the first column of each.
- **Type B:** three single-state characters in one image, one character per column.

**Image size in the node:** 1536 × 1024 for three columns, 1024 × 1024 for two columns. Set the size in the node, not in the prompt text.

**Prompt format:** every prompt uses exactly the fields of the node `Template/flux2-prompt-node-v2.html`: `prompt`, `style`, `camera` (with `angle`, `distance`, `lens`, `f-number`, `ISO`, `focus`), `lighting`, `colors` (with `palette` and `mood`) and `composition`. Each field can be pasted directly into the matching node field.

## Part 2: Type A Sheets, One Character in Several States

### Type A 1: Hamlet in Mourning Attire · Hamlet in Fencing Attire · Hamlet in Dishevelled Clothes; scenes 1–8 and 12

**Size in the node:** 1536 × 1024 · **File name:** `CHR_Hamlet_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Hamlet in Mourning Attire\": Hamlet, a slim man about thirty of medium height, pale complexion, angular face with high cheekbones, intense grey eyes with faint shadows beneath them, small straight nose, dark brown wavy hair falling just below the ears, short neatly trimmed dark beard and moustache, bare head, a fitted black velvet doublet with subtle black embroidery and a small white linen collar, black breeches and black hose, black leather shoes, a long black wool cloak, a thin silver chain with a small round silver locket on his chest, brooding melancholy expression. Middle column, captioned \"Hamlet in Fencing Attire\": the same man as in the other columns, with an identical face, bare head, without doublet or cloak, a loose white linen fencing shirt with full sleeves, black breeches, black hose, flat black leather shoes, the same thin silver chain with the small round silver locket, holding a slim rapier with a swept steel hilt pointing downward, its tip covered by a small round leather button, serene resigned expression. Right column, captioned \"Hamlet in Dishevelled Clothes\": the same man as in the other columns, with an identical face, tangled hair, bare head, the black velvet doublet hanging unbuttoned over a loose crumpled white linen shirt open at the neck, no cloak, black breeches, one black stocking slipped down to the ankle, the same thin silver chain with the small round silver locket, holding a small closed leather-bound book, distracted ironic expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#0A0A0A", "#EDEAE3", "#2A2A2E", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Hamlet in Mourning Attire\", \"Hamlet in Fencing Attire\", \"Hamlet in Dishevelled Clothes\""
}
```

**Identity lines:**

- Hamlet in Mourning Attire: `Hamlet, slim prince about thirty, pale angular face, intense grey eyes, slightly unkempt dark brown hair below the ears, short trimmed dark beard, black velvet mourning doublet with small white collar, long black cloak, thin silver chain with round pendant`
- Hamlet in Fencing Attire: `Hamlet, slim prince about thirty, pale angular face, intense grey eyes, slightly unkempt dark brown hair below the ears, short trimmed dark beard, loose white linen fencing shirt, black breeches, thin silver chain with round pendant, slim rapier`
- Hamlet in Dishevelled Clothes: `Hamlet, slim prince about thirty, pale angular face, intense grey eyes, tangled dark brown hair below the ears, short trimmed dark beard, black velvet doublet hanging unbuttoned over a loose white linen shirt, no cloak, one black stocking slipped down to the ankle, thin silver chain with round pendant`

**Note:** The columns match the three states in the sample image `Sample-Type-A.png`. The mourning clothes are seen in scenes 1–3 and 5–8, the dishevelled clothes in scene 4, and the fencing shirt in scene 12. The small round silver locket is the one that holds his father's portrait in scene 8.

---

### Type A 2: Hamlet in Mourning Attire · Hamlet in Travel Clothes; scenes 10 and 11

**Size in the node:** 1024 × 1024 · **File name:** `CHR_Hamlet_states_2.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Hamlet in Mourning Attire\": Hamlet, a slim man about thirty of medium height, pale complexion, angular face with high cheekbones, intense grey eyes with faint shadows beneath them, small straight nose, dark brown wavy hair falling just below the ears, short neatly trimmed dark beard and moustache, bare head, a fitted black velvet doublet with subtle black embroidery and a small white linen collar, black breeches and black hose, black leather shoes, a long black wool cloak, a thin silver chain with a small round silver locket on his chest, brooding melancholy expression. Right column, captioned \"Hamlet in Travel Clothes\": the same man as in the other columns, with an identical face, slightly weathered by a sea voyage, bare head, a plain dark charcoal wool travelling cloak over a worn black doublet, black breeches, scuffed knee-high black leather boots, a sword with a plain steel crossguard in a black leather scabbard at his left hip, the same thin silver chain with the small round silver locket, calm resolved expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#0A0A0A", "#4A4A4E", "#7A6A58", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Hamlet in Mourning Attire\", \"Hamlet in Travel Clothes\""
}
```

**Identity lines:**

- Hamlet in Travel Clothes: `Hamlet, slim prince about thirty, pale angular face, intense grey eyes, slightly unkempt dark brown hair below the ears, short trimmed dark beard, plain dark travelling cloak over a worn black doublet, scuffed black boots, sword at his hip, thin silver chain with round pendant`

**Note:** Hamlet has four states, so as the instructions require they are split over two images, and the main state, the mourning clothes, is repeated as the first column of both. The identity line for the mourning clothes is in Type A 1.

---

### Type A 3: Old Hamlet in Armour · Old Hamlet in Gown; scenes 1, 3 and 8

**Size in the node:** 1024 × 1024 · **File name:** `CHR_OldHamlet_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Old Hamlet in Armour\": Old Hamlet, a tall broad-shouldered man about sixty, gaunt face, sunken sorrowful dark eyes, strong straight nose, short dark beard and moustache heavily streaked with silver, pale skin, complete late sixteenth-century plate armour from head to foot in dark polished steel with thin gilded borders, a plain steel close helmet with a smooth rounded skull and the visor raised to show the whole face, steel gorget, rounded pauldrons, articulated gauntlets, a deep crimson sash across the breastplate from right shoulder to left hip, holding a short dark marshal's baton in the right hand, rendered as a solid fully opaque figure, solemn grieving expression. Right column, captioned \"Old Hamlet in Gown\": the same man as in the other columns, with an identical face, alive and healthy with natural skin colour, short greying dark hair, bare head, a loose dark crimson velvet gown with a brown fur collar over a white linen shirt, soft black velvet slippers, a heavy gold ring on his right hand, gentle tired expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#2B2F33", "#B8963E", "#6B1E22", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Old Hamlet in Armour\", \"Old Hamlet in Gown\""
}
```

**Identity lines:**

- Old Hamlet in Armour: `ghost of an old warrior about sixty, gaunt pale face, sorrowful dark eyes, short dark beard streaked with silver, full dark steel plate armour with thin gilded borders, plain steel close helmet with the visor raised, crimson sash, short marshal's baton in right hand`
- Old Hamlet in Gown: `the old man about sixty, gaunt face, short dark beard streaked with silver, short greying hair, bare head, loose dark crimson velvet gown with brown fur collar`

**Note:** The armour is for the ghost in scenes 1, 3 and 8; the gown is for the orchard flashback in scene 3 and the locket portrait in scene 8. In the sheet the ghost is deliberately solid. In the shots, add to the identity line: `faintly translucent, glowing pale`. The caption and description use Old Hamlet and old warrior instead of king, because the word king gave the ghost a crown in shot 6.

---

### Type A 4: Ophelia · Ophelia in Madness; scenes 4–6 and 9–11

**Size in the node:** 1024 × 1024 · **File name:** `CHR_Ophelia_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Ophelia\": Ophelia, a young noblewoman about eighteen, slender and of medium height, delicate oval face, pale skin, large hazel eyes, small straight nose, soft full lips, long straight light golden-brown hair parted in the centre and gathered in a loose braid down her back, bare head, a pale blue silk gown with a fitted bodice, long sleeves and a small white lace collar, a thin silver girdle at the waist, holding a small closed prayer book with a dark leather cover and brass clasp in both hands, gentle shy expression. Right column, captioned \"Ophelia in Madness\": the same woman as in the other columns, with an identical face, thinner and paler, faint shadows under red-rimmed eyes, long light golden-brown hair worn loose and tangled to the waist with small wildflowers and stems caught in it, a modest loose white linen gown with long sleeves and a high gathered neckline, crumpled, the hem grey with dust and torn in one place, barefoot, holding a loose bunch of rosemary sprigs, purple and yellow pansies, small white daisies and a few faded violets against her chest, distant dreamy half-smile. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#9DB4CC", "#EDE8DE", "#B8875A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Ophelia\", \"Ophelia in Madness\""
}
```

**Identity lines:**

- Ophelia: `Ophelia, young noblewoman about eighteen, delicate oval face, pale skin, large hazel eyes, long straight light golden-brown hair in a loose braid down her back, pale blue silk gown with a fitted bodice and small white lace collar, holding a small closed prayer book with a dark leather cover and brass clasp`
- Ophelia in Madness: `Ophelia after her madness, young noblewoman about eighteen, delicate oval face, pale skin, large hazel eyes with red rims, long loose tangled light golden-brown hair with wildflowers caught in it, modest loose white linen gown with long sleeves, crumpled and dusty at the hem, barefoot, holding a bunch of rosemary, pansies, daisies and faded violets`

**Note:** The second state is for scenes 9 and 10. For scene 10, add a crown of wildflowers in the shot prompt.

---

### Type A 5: Laertes in Travel Clothes · Laertes in Fencing Attire; scenes 9–12

**Size in the node:** 1024 × 1024 · **File name:** `CHR_Laertes_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Laertes in Travel Clothes\": Laertes, son of Polonius, an athletic young man about twenty-two, tall with broad shoulders, handsome square face, fair complexion, strong straight brows, light grey-green eyes, short light golden-brown hair brushed back, short clipped golden-brown beard along the jaw and a light moustache, bare head, a fashionable French-cut slate-grey travelling doublet with a row of small silver buttons and a narrow white linen collar, dark grey breeches, a dark charcoal wool cloak over one shoulder, brown leather riding gloves, high brown leather riding boots, a rapier with a swept steel hilt in a dark leather scabbard on his left hip, serious proud expression. Right column, captioned \"Laertes in Fencing Attire\": the same man as in the other columns, with an identical face, bare head, without doublet or cloak, a loose white linen fencing shirt, dark grey breeches, grey hose, flat black leather shoes, a brown leather fencing glove on the right hand, holding a slim rapier with a swept steel hilt pointing downward, guarded unreadable expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#5B646B", "#EDEAE3", "#8A6A45", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Laertes in Travel Clothes\", \"Laertes in Fencing Attire\""
}
```

**Identity lines:**

- Laertes in Travel Clothes: `Laertes, son of Polonius, athletic young man about twenty-two, handsome square face, fair complexion, short light golden-brown hair, light grey-green eyes, short clipped golden-brown beard along the jaw, fashionable French-cut slate-grey travelling doublet with silver buttons, dark cloak, high leather riding boots, rapier at his hip`
- Laertes in Fencing Attire: `Laertes, athletic young man about twenty-two, handsome square face, short light golden-brown hair, short clipped golden-brown beard, loose white linen fencing shirt, dark grey breeches, brown leather fencing glove, slim rapier`

**Note:** The travel clothes are for scenes 9–11 and the fencing shirt for scene 12. His hair and beard deliberately share Ophelia's hair colour to show that they are brother and sister.

---

## Part 3: Type B Sheets, Three Single-State Characters per Image

### Type B 1: Horatio · Gertrude · Claudius; scenes 1–12

**Size in the node:** 1536 × 1024 · **File name:** `CHR_Group_Horatio_Gertrude_Claudius.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Horatio\": Horatio, a slim young scholar about twenty-five, medium height, oval face, clean-shaven, short wavy dark brown hair, dark brown eyes, straight nose, bare head, a plain black wool doublet buttoned to the neck with a small white linen falling collar, black wool breeches and black hose, low black leather shoes, a long black wool cloak fastened at the right shoulder, a narrow leather belt with a small leather pouch, thoughtful sceptical expression. Middle column, captioned \"Gertrude\": Gertrude, a handsome woman about forty-five, upright and graceful, fair skin, composed face with fine lines at the eyes, high forehead, grey-green eyes, auburn hair parted in the centre and drawn back, her only headwear a small dark velvet French hood edged with a single row of pearls that leaves the front of her hair visible, a deep blue velvet gown with gold embroidered bands, a square neckline and full sleeves with slashed cuffs, a pearl necklace with a small oval gold locket, a gold ring on her right hand, hands folded at her waist, calm reserved expression. Right column, captioned \"Claudius\": Claudius, a robust man about fifty, broad face with full cheeks, well-groomed short dark beard and moustache with a little grey at the chin, heavy-lidded calculating dark eyes, dark hair cut short, a gold crown set with dark red stones, a deep red velvet robe with gold embroidered bands and a wide ermine collar over a black satin doublet, a heavy gold chain, gold rings on both hands, controlled polite expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#111111", "#1E2F5C", "#7A1F24", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Horatio\", \"Gertrude\", \"Claudius\""
}
```

**Identity lines:**

- Horatio: `Horatio, slim young scholar about twenty-five, clean-shaven oval face, short wavy dark brown hair, dark brown eyes, plain black wool doublet with small white linen collar, long black wool cloak`
- Gertrude: `Gertrude, handsome woman about forty-five, fair skin, composed face with fine lines, grey-green eyes, auburn hair under a small pearl-edged French hood, deep blue velvet gown with gold embroidery and a square neckline, pearl necklace`
- Claudius: `Claudius, robust man about fifty, well-groomed short dark beard, heavy-lidded calculating eyes, deep red velvet robe with gold embroidery and ermine collar, gold crown`

**Note:** In the sample image `Sample-Type-B.png`, Gertrude got a crown and a veil because the caption was "Queen of Denmark". The caption is now only "Gertrude", and the small French hood is described explicitly. In scene 11, Claudius and Gertrude wear black mourning cloaks over these clothes; write this in the shot prompt. Gertrude's small oval gold locket is the one that holds Claudius's portrait in scene 8.

---

### Type B 2: Bernardo · Marcellus · Fortinbras; scenes 1–3 and 12

**Size in the node:** 1536 × 1024 · **File name:** `CHR_Group_Bernardo_Marcellus_Fortinbras.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Bernardo\": Bernardo, a stocky castle guard about forty, weathered ruddy face, heavy brow, deep-set brown eyes, broad nose, short dark brown beard with a few grey hairs, a steel morion helmet with a raised comb and curved brim, a dark brown wool cloak over a buff leather jerkin with padded sleeves, brown wool breeches, worn knee-high leather boots, a small horn lantern hanging from a leather belt on the left hip, holding a tall partisan spear upright in the right hand, calm tired expression. Middle column, captioned \"Marcellus\": Marcellus, a lean castle guard about thirty, narrow face, high cheekbones, sharp nose, alert light blue eyes, short reddish-blond beard and moustache, a steel morion helmet with a raised comb and curved brim, a grey-blue wool cloak over a buff leather jerkin with padded sleeves, dark grey wool breeches, knee-high leather boots, holding a tall partisan spear upright in the left hand, slightly wary expression. Right column, captioned \"Fortinbras\": Fortinbras, a tall commanding young man about twenty-eight, weathered lean face, sharp blue eyes, long reddish-blond hair tied back, close-cropped reddish-blond beard, bare head, a polished steel breastplate over a dark blue padded doublet, a grey wolf-fur mantle on his shoulders, dark blue breeches, tall black riding boots, a sword with a plain steel hilt at his hip, one hand on the sword hilt, grave composed expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#5A3E2B", "#4F6475", "#1E2F4A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Bernardo\", \"Marcellus\", \"Fortinbras\""
}
```

**Identity lines:**

- Bernardo: `Bernardo, stocky Danish guard about forty, weathered ruddy face, short dark brown beard with grey hairs, steel morion helmet, dark brown wool cloak over buff leather jerkin, horn lantern on left hip, partisan spear`
- Marcellus: `Marcellus, lean Danish guard about thirty, narrow face, sharp nose, light blue eyes, short reddish-blond beard, steel morion helmet, grey-blue wool cloak over buff leather jerkin, partisan spear`
- Fortinbras: `Fortinbras, tall commanding young man about twenty-eight, weathered lean face, sharp blue eyes, long reddish-blond hair tied back, close-cropped reddish-blond beard, polished steel breastplate over a dark blue padded doublet, grey wolf-fur mantle, sword at his hip`

**Note:** The three armed men are placed together so their differences are clear: Bernardo is stocky with a brown beard and brown cloak, Marcellus is lean with a reddish beard and grey-blue cloak, and Fortinbras is tall with a breastplate and wolf fur. Fortinbras's caption deliberately leaves out the title Prince.

---

### Type B 3: Polonius · Rosencrantz · Guildenstern; scenes 2, 4, 5, 6 and 8

**Size in the node:** 1536 × 1024 · **File name:** `CHR_Group_Polonius_Rosencrantz_Guildenstern.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Polonius\": Polonius, an elderly court counsellor about sixty-five, slightly stooped, thin face, bald on top with wispy white hair at the sides, neat pointed white beard, small shrewd pale eyes, a long dark green wool gown with grey fur trim, a small white ruff, a black doublet beneath, dark green velvet slippers, a heavy gold chain of office, one finger raised, self-satisfied knowing expression. Middle column, captioned \"Rosencrantz\": Rosencrantz, a young courtier about thirty, of medium height and slightly plump, round face, curly light brown hair, small moustache and no beard, light brown eyes, bare head, a mustard-yellow slashed doublet with a small white ruff, mustard and brown paned trunk hose, yellow hose, brown leather shoes, a short brown cape, hands clasped in front, ingratiating smile. Right column, captioned \"Guildenstern\": Guildenstern, a young courtier about thirty, tall and thin, long thin face, straight black hair to the jaw, clean-shaven, narrow dark eyes, bare head, a plum-purple doublet with a small white ruff, plum and black paned trunk hose, black hose, black leather shoes, a short black cape, arms at his sides, cautious closed expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#2F4A35", "#C9A23A", "#5A2A4A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Polonius\", \"Rosencrantz\", \"Guildenstern\""
}
```

**Identity lines:**

- Polonius: `Polonius, elderly counsellor about sixty-five, thin face, bald on top with wispy white hair at the sides, neat pointed white beard, small shrewd pale eyes, long dark green wool gown with grey fur trim, small white ruff, heavy gold chain of office`
- Rosencrantz: `Rosencrantz, young courtier about thirty, round face, curly light brown hair, small moustache, mustard-yellow slashed doublet with a small white ruff`
- Guildenstern: `Guildenstern, young courtier about thirty, long thin face, straight black hair to the jaw, clean-shaven, plum-purple doublet with a small white ruff`

**Note:** Rosencrantz and Guildenstern deliberately differ in costume colour, face shape, hair and height. Polonius's identity line uses "bald on top" instead of "bald crown" so the model does not read it as a crown.

---

### Type B 4: First Player · Boy Player · Yorick; scenes 4, 6 and 11

**Size in the node:** 1536 × 1024 · **File name:** `CHR_Group_FirstPlayer_BoyPlayer_Yorick.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"First Player\": First Player, a middle-aged travelling actor about fifty, weathered expressive face with deep laugh lines, grey-flecked brown beard, long greying brown hair tied back, warm brown eyes, bare head, a faded crimson stage cloak with a frayed gold border over a worn brown doublet, patched brown breeches, scuffed boots, holding a painted wooden crown with chipped gilt and glass jewels in one hand, theatrical warm expression. Middle column, captioned \"Boy Player\": a slim beardless youth about sixteen dressed to play a woman on stage, narrow boyish face with a slightly square jaw beneath the makeup, thick white powder on the face, round rouged cheeks, darkened eyebrows, reddened lips, light brown eyes, a long pale blonde stage wig with a slightly artificial sheen topped by a small painted wooden crown, a stiff old-fashioned gold-and-rose brocade gown that is a little too broad at the shoulders, with worn patches and a frayed hem, a lace ruff yellowed with age, hands clasped in front in a theatrical ladylike manner. Right column, captioned \"Yorick\": Yorick, a lively court jester about forty, lean and agile, thin expressive face with a wide grin, merry dark eyes, clean-shaven, a soft red and green cap with small brass bells, a two-coloured motley tunic in faded red and green, matching parti-coloured hose, soft leather shoes, holding a short jester's stick with a small carved head, laughing. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#8A2A22", "#C9A35A", "#3E6A3A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"First Player\", \"Boy Player\", \"Yorick\""
}
```

**Identity lines:**

- First Player: `First Player, a middle-aged actor about fifty, weathered expressive face, grey-flecked brown beard, long greying hair tied back, faded crimson stage cloak over a worn brown doublet`
- Boy Player: `Boy Player, a slim beardless youth about sixteen playing a woman, powdered face, rouged cheeks, long pale wig, stiff old-fashioned brocade gown`
- Yorick: `Yorick, a lively jester about forty, thin expressive face with a wide grin, merry dark eyes, a two-coloured motley tunic in faded red and green, a soft cap with small bells`

**Note:** The three performers are grouped together. The caption of the boy who plays the Player Queen is deliberately "Boy Player", not "Player Queen", so the word queen does not make the costume royal. In Shakespeare's theatre, women's roles were played by boys. The First Player wears the wooden crown in scene 6.

---

### Type B 5: First Gravedigger · Second Gravedigger; scene 11

**Size in the node:** 1024 × 1024 · **File name:** `CHR_Group_Gravediggers.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"First Gravedigger\": a stout weathered peasant about sixty, ruddy cheerful face, bushy grey eyebrows, grey stubble, a few missing teeth, small twinkling blue eyes, a brown woollen cap, a rough brown wool tunic with rolled sleeves, a stained leather apron, coarse grey breeches, mud-caked boots, holding a long-handled iron spade, gap-toothed grin. Right column, captioned \"Second Gravedigger\": a lanky young labourer about twenty, tall and thin, thin face, pale freckled skin, wide pale eyes, straw-coloured hair sticking out from under a grey cap, a grey wool tunic, patched brown breeches tied below the knee, rough wooden-soled shoes, holding a short iron spade, slow simple expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, straight-on front view in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "f-number": "f/8",
    "ISO": 100,
    "focus": "deep focus, everything sharp in every panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows",
  "colors": {
    "palette": ["#5A4632", "#7A7A72", "#C8B07A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"First Gravedigger\", \"Second Gravedigger\""
}
```

**Identity lines:**

- First Gravedigger: `First Gravedigger, a stout weathered peasant about sixty, ruddy cheerful face, bushy grey eyebrows, grey stubble, a few missing teeth, rough brown wool tunic, stained leather apron, brown woollen cap, mud-caked boots`
- Second Gravedigger: `Second Gravedigger, a lanky young labourer about twenty, thin face, straw-coloured hair, grey wool tunic`

**Note:** The two remaining characters are placed in a two-column image.

---

## Part 4: Notes

- **Image list:** ten images for 22 character states. Type A: Hamlet (two images), Old Hamlet, Ophelia, Laertes. Type B: Horatio, Gertrude and Claudius; Bernardo, Marcellus and Fortinbras; Polonius, Rosencrantz and Guildenstern; First Player, Boy Player and Yorick; the two gravediggers.
- **Characters without a sheet:** these are seen only once, from behind, in silhouette, or as part of a body: Francisco, Lucianus (the player who pours the poison), the child Hamlet in Yorick's memory, the priest at the burial, Osric, servants, courtiers, rebels and Norwegian soldiers. If a shot list needs a close view of any of them, write a sheet for that character.
- **Captions:** captions are personal names, not titles. "Queen of Denmark" was changed to "Gertrude" because it gave her a crown and veil in the sample image. For the same reason, no caption uses King, Queen or Prince.
- **Before use as a reference:** crop the caption strip off the image so the text does not leak into the shots. In each shot, pass only the column of the state the shot needs.
- **Keeping the face consistent in Type A:** if the face differs slightly between the columns of one image, pass the first column's close-up as a reference and generate the image again.
- **Changes from the previous version:** the six-panel sheets (front, three-quarter and profile) were converted to the new front-view format with captions; 24 separate sheets were merged into ten images; every character's headwear is now described explicitly and positively; the identity lines of Bernardo and Marcellus now include their names.