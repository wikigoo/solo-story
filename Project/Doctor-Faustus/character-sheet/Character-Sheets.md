# Doctor Faustus: Character Sheets

## Part 1: Fixed Film Decisions

**Historical period:** the Holy Roman Empire around 1535. This is the German Renaissance: the time of Charles the Fifth, and Wittenberg in the age of Luther.

- **Costume:** the Schaube (a long gown with a wide fur collar), slashed doublets, wide flat caps and woollen hose.
- **Weapons:** the Landsknecht short sword, early slender rapiers and halberds.
- **Architecture:** in Wittenberg, half-timbered houses and late Gothic vaulted rooms; in Rome, a Renaissance hall with frescoes and marble; at the Emperor's court, a stone hall with leaded windows and wall tapestries.
- **Light sources:** tallow and wax candles, oil lamps, torches, braziers, horn lanterns, and daylight through leaded windows.
- **Exceptions:** Alexander, his paramour and Helen wear ancient Greek dress. The angels, the devils and the Seven Deadly Sins are supernatural and theatrical.

**Fixed style string:**

```
Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge
```

**Location Looks:**

|Location|Scenes|Base light|Palette|
|---|---|---|---|
|Faustus's study|1, 5, 7|Amber candle and brazier light with deep shadows; blue moonlight from the window|`#2A1E16` `#8B5A2B` `#D9A441` `#3B4A5A`|
|In front of Faustus's house|2|Soft overcast late-afternoon light turning toward dusk|`#6F6A62` `#A9926E` `#4A3A2E` `#B7BEC4`|
|Solitary grove at night|3|Cold moonlight through bare trees, mist, flickering orange torchlight by the circle|`#0F1A24` `#2F4A3A` `#9FB3C8` `#E0752D`|
|A street in Wittenberg|4|A shadowed street with one sharp band of morning sun|`#5C4B3B` `#8A7A63` `#E2C48E` `#3E4A3F`|
|Inn stable|6|Dusty shafts of sunlight between the boards, warm straw|`#4B3621` `#C9A15B` `#E8C987` `#6B5B4E`|
|The Pope's banquet hall, Rome|8|The golden light of dozens of wax candles in silver candlesticks on marble and fresco|`#7A1F24` `#C9A44C` `#E9DFC8` `#3A2B22`|
|Outside the tavern|9|Blue dusk, warm window light and a lantern above the door|`#1E2A3A` `#D88C3A` `#5A4636` `#6B1E2E`|
|The Emperor's court|10|Cool bright daylight through tall leaded windows|`#2E3B4E` `#B08D57` `#D8D2C4` `#6B4B35`|
|The road to Wittenberg and the pond|10|Flat overcast midday light, muted greens, grey water|`#6E7A5A` `#8C8F86` `#A89F7E` `#4A5A5E`|
|The hall of Faustus's house|11, 12|Dying candles and a brazier, cold moonlight from the window|`#1A1410` `#C27C2C` `#6E2B1E` `#4D5D73`|

**Sheet format:** follows `Instructions/Instructions-Character-Sheet.md`. Every image has two rows: a front-facing close-up on top and a front-facing full body below. The character's name in English is written under each column.

- **Type A:** one character seen in several ages, costumes or forms; all states in one image, one state per column.
- **Type B:** three single-state characters in one image, one character per column. Two-column images are used for the last characters.

**Image size in the node:** 1536 × 1280 for three columns, 1024 × 1536 for two columns. Set the size in the node, not in the prompt text.

**Prompt format:** every prompt uses exactly the fields of the node `Template/flux2-prompt-node-v2.html`: `prompt`, `style`, `camera` (with `angle`, `distance`, `lens`, `f-number`, `ISO`, `focus`), `lighting`, `colors` (with `palette` and `mood`) and `composition`. Each field can be pasted directly into the matching node field.

## Part 2: Type A Sheets, One Character in Several States

### Type A 1: Faustus in Scholar's Gown · Faustus in Court Dress · Faustus in Old Age; scenes 1–12

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Faustus_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Faustus in Scholar's Gown\": Doctor Faustus about forty, tall and lean, long narrow face, high forehead, deep-set grey-green eyes, thin straight nose, dark brown hair to the shoulders, full dark brown beard trimmed to a point, a black wool doctor's flat cap, a long black wool scholar's gown with a wide dark brown marten fur collar, black wool doublet and black hose beneath, black leather shoes, a plain leather belt with a small iron key ring, holding a thick closed leather-bound book with brass clasps against his chest, intense restless expression. Middle column, captioned \"Faustus in Court Dress\": the same man as in the other columns, with the same bone structure, eyes and nose, now about fifty-two, his face lightly lined, first grey at the temples, the pointed dark brown beard greying at the chin, a black velvet flat cap with a small white ostrich feather, a crimson velvet slashed doublet with gold silk puffs, a long dark crimson velvet gown with a wide sable fur collar, black hose, black velvet shoes, a heavy gold chain across the shoulders, gold rings on both hands, confident amused expression. Right column, captioned \"Faustus in Old Age\": the same man as in the other columns, with the same bone structure, eyes and nose, now about sixty-four, slightly stooped and gaunt, the face deeply lined with hollow cheeks, red-rimmed haunted eyes, thinning long grey-white hair, an untrimmed grey beard that has lost its point, bare head, a faded black wool gown with a worn patchy brown fur collar, a loosened off-white linen shirt at the neck, the black doublet open, black hose, scuffed black shoes, exhausted fearful expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#111111", "#6E1A1F", "#C9A44C", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Faustus in Scholar's Gown\", \"Faustus in Court Dress\", \"Faustus in Old Age\""
}
```

**Identity lines:**

- Faustus in Scholar's Gown: `Doctor Faustus, tall lean scholar about forty, long narrow face, deep-set grey-green eyes, dark brown shoulder-length hair, pointed dark brown beard, black flat cap, long black gown with dark brown fur collar, closed leather book with brass clasps`
- Faustus in Court Dress: `Doctor Faustus about fifty-two, lean, long narrow face lightly lined, grey-green eyes, pointed dark brown beard greying at the chin, black velvet cap with white feather, crimson slashed doublet, dark crimson gown with sable collar, heavy gold chain`
- Faustus in Old Age: `aged Doctor Faustus about sixty-four, gaunt and slightly stooped, deeply lined narrow face, haunted red-rimmed grey-green eyes, thinning grey-white hair, untrimmed grey beard, bare head, faded black gown with worn brown fur collar`

**Note:** The three columns are one face at three ages: the scholar's gown for scenes 1–7, the court dress for scenes 8–10, and old age for scenes 11 and 12. In every shot, use the identity line of the right age.

---

### Type A 2: Wagner in Youth · Wagner in Middle Age; scenes 1, 2, 4 and 11

**Size in the node:** 1024 × 1536 · **File name:** `CHR_Wagner_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Wagner in Youth\": Wagner, a short wiry young man about twenty, round freckled face, upturned nose, quick sly light blue eyes, sandy blond hair cut in a straight fringe, clean-shaven, a brown felt cap, a short dark green wool coat over a brown wool doublet, an off-white linen shirt collar, brown hose, worn brown leather shoes, a leather satchel on a strap across the body, cheeky knowing half smile. Right column, captioned \"Wagner in Middle Age\": the same man as in the other columns, with the same bone structure, eyes and nose, now about forty-four and thickset, the round freckled face fuller and lined, receding sandy blond hair mixed with grey, a short sandy-grey beard, bare head, an old long black wool gown with a dark brown marten fur collar that is slightly too long for him, a brown wool doublet beneath, brown hose, brown leather shoes, holding a small iron key ring, thoughtful uneasy expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#2F4A33", "#6B4A2E", "#151515", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Wagner in Youth\", \"Wagner in Middle Age\""
}
```

**Identity lines:**

- Wagner in Youth: `Wagner, short wiry servant about twenty, round freckled face, upturned nose, sly light blue eyes, sandy blond fringe, clean-shaven, brown felt cap, short dark green wool coat over brown doublet, leather satchel`
- Wagner in Middle Age: `Wagner about forty-four, short and thickset, round freckled lined face, light blue eyes, receding sandy-grey hair, short sandy-grey beard, oversized old black gown with dark brown fur collar, iron key ring`

**Note:** Wagner in middle age wears Faustus's old gown, which Faustus leaves to him in scene 11, so it is the same gown as in Type A 1, slightly too long for him.

---

### Type A 3: Mephistopheles in Demon Form · Mephistopheles as a Friar; scenes 3–12

**Size in the node:** 1024 × 1536 · **File name:** `CHR_Mephistopheles_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Mephistopheles in Demon Form\": Mephistopheles in his first demonic form, a very tall gaunt humanoid demon, hairless head with a long skull, two long ridged ram horns curling back from the temples, ash-black skin with fine cracks like burnt wood showing a dull ember-orange beneath, glowing ember-orange eyes, gaunt cheeks, a thin lipless mouth, long bony fingers with dark claws, a bare sinewy torso, ragged dark grey cloth wrapped around the hips to the knees, long bony legs ending in dark cloven hooves, rendered as a solid fully opaque figure, cold sorrowful expression. Right column, captioned \"Mephistopheles as a Friar\": the same tall gaunt figure in human disguise as an old friar appearing about fifty-five, sallow pale skin, sunken cheeks, a long hooked nose, thin pale lips, piercing pale amber eyes, a shaved tonsure with a thin ring of black hair streaked with grey, clean-shaven, a coarse grey-brown wool habit to the ankles with the hood down on the shoulders, a white rope belt with three knots hanging at the left side, plain dark wooden prayer beads at the belt, worn leather sandals on bare feet, long pale fingers with the hands folded inside the sleeves, cold melancholy watchful expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#1A1716", "#C4561E", "#6A5E50", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Mephistopheles in Demon Form\", \"Mephistopheles as a Friar\""
}
```

**Identity lines:**

- Mephistopheles in Demon Form: `Mephistopheles demon form, very tall gaunt hairless demon, long curling ram horns, ash-black cracked skin with ember-orange glow beneath, glowing ember-orange eyes, clawed bony fingers, ragged dark grey hip cloth, cloven hooves`
- Mephistopheles as a Friar: `Mephistopheles as Franciscan friar, very tall gaunt man, sallow sunken face, hooked nose, piercing pale amber eyes, black-grey tonsure, clean-shaven, coarse grey-brown habit with hood down, white three-knot rope belt, dark wooden beads, sandals`

**Note:** The demon form appears only at the start of scene 3. From then to the end of the film, Mephistopheles keeps the friar's disguise. The same height and gaunt build link the two forms.

---

### Type A 4: Robin · Robin as an Ape; scenes 6 and 9

**Size in the node:** 1024 × 1536 · **File name:** `CHR_Robin_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Robin\": Robin the ostler, a short sturdy man about twenty-five, ruddy round face, small bright brown eyes, a broad grin, shaggy chestnut hair with bits of straw in it, two days of chestnut stubble, bare head, a rust-red cloth neckerchief, a scuffed brown leather jerkin over a grimy off-white linen shirt with rolled sleeves, a stained leather apron, brown hose, muddy ankle boots, holding a thick closed leather-bound book with brass clasps under his arm, delighted scheming expression. Right column, captioned \"Robin as an Ape\": Robin transformed into an animal, a stocky Barbary macaque with thick shaggy chestnut-brown fur the colour of his hair, a pinkish bare face, the same small bright brown eyes, a short stub tail, the same crumpled rust-red cloth neckerchief tied around its neck, standing on all fours, startled indignant expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#9C3A24", "#6B4A2E", "#7A5634", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Robin\", \"Robin as an Ape\""
}
```

**Identity lines:**

- Robin: `Robin the ostler, short sturdy man about twenty-five, ruddy round face, small bright brown eyes, shaggy chestnut hair with straw, stubble, rust-red neckerchief, brown leather jerkin and stained apron, stolen closed leather book with brass clasps`
- Robin as an Ape: `Robin as an ape, stocky Barbary macaque with shaggy chestnut-brown fur, pinkish face, small bright brown eyes, crumpled rust-red neckerchief`

**Note:** Robin's book is deliberately the same book that Faustus holds in Type A 1, so the viewer sees that it was stolen. The rust-red neckerchief and the chestnut colour link the man to the ape.

---

### Type A 5: Rafe · Rafe as a Dog; scenes 6 and 9

**Size in the node:** 1024 × 1536 · **File name:** `CHR_Rafe_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Rafe\": Rafe, a tall lanky young man about twenty-two, long horse-like face, drooping eyelids, dim gentle pale blue eyes, a slack open mouth, lank straight black hair to the jaw, clean-shaven, a faded blue knitted cap, a long faded blue linen smock belted with a cord, brown wool hose, worn brown shoes, slouched relaxed stance, simple bewildered expression. Right column, captioned \"Rafe as a Dog\": Rafe transformed into an animal, a tall lanky scruffy black mongrel with long thin legs, a long narrow muzzle, droopy ears, the same droopy-lidded pale eyes, a rough lank black coat, a thin tail, the same faded blue knitted cap tied loosely under its chin, standing on all fours, confused mournful expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#5C7690", "#1A1A1A", "#6B4A2E", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Rafe\", \"Rafe as a Dog\""
}
```

**Identity lines:**

- Rafe: `Rafe, tall lanky young man about twenty-two, long horse-like face, drooping eyelids, dim pale blue eyes, lank black jaw-length hair, clean-shaven, faded blue knitted cap, faded blue linen smock`
- Rafe as a Dog: `Rafe as a dog, lanky scruffy black mongrel, long narrow muzzle, droopy ears, droopy-lidded pale eyes, faded blue knitted cap tied under its chin`

**Note:** Robin and Rafe are deliberately different: short, ruddy and brown against tall, pale and blue. The blue cap and the lank black hair link Rafe to the dog.

---

### Type A 6: The Knight · Knight with Antlers; scene 10

**Size in the node:** 1024 × 1536 · **File name:** `CHR_Knight_states.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"The Knight\": a burly courtier about forty, square heavy face, a crooked once-broken nose, a sneering mouth, mocking brown eyes, cropped black hair, a short black spade beard, a black velvet flat cap with a red feather, a maroon velvet doublet slashed with black silk, black hose, black leather shoes, a short broad sword in a black leather scabbard on a sword belt at the left hip, swaggering stance, scornful mocking expression. Right column, captioned \"Knight with Antlers\": the same man as in the other columns, with an identical face, now bareheaded with a large pair of branching brown stag antlers growing from the top of his head, a flushed ashamed face, wide pleading eyes, the same maroon velvet doublet slashed with black silk now slightly disordered, black hose, black leather shoes, the same short sword at the left hip, standing stiffly, humiliated pleading expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#5A1A22", "#141414", "#7A5A3A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"The Knight\", \"Knight with Antlers\""
}
```

**Identity lines:**

- The Knight: `the Knight, burly man about forty, square face, crooked broken nose, sneering mouth, cropped black hair, short black spade beard, maroon velvet doublet slashed with black, black cap with red feather, short sword at left hip`
- Knight with Antlers: `the Knight with stag antlers, burly man about forty, square flushed face, crooked nose, short black spade beard, bareheaded with large branching brown stag antlers, maroon doublet slashed with black, short sword at left hip`

**Note:** The word knight may pull the model toward armour, so the description calls him a courtier and states his velvet court clothes explicitly. If armour still appears, regenerate.

---

## Part 3: Type B Sheets, Three Single-State Characters per Image

### Type B 1: Good Angel · Bad Angel · Old Man; scenes 1, 5, 7 and 11

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Group_GoodAngel_BadAngel_OldMan.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Good Angel\": a tall graceful youthful figure appearing about twenty-five, gentle oval face, fair skin, clear calm blue eyes, golden-blond shoulder-length curls, beardless, bare head, a long ivory-white linen robe falling to the feet with a narrow gold-embroidered hem, a plain gold cord at the waist, bare feet, large white feathered wings folded behind the shoulders, hands softly clasped at the chest, rendered as a solid fully opaque figure, compassionate pleading expression. Middle column, captioned \"Bad Angel\": a tall lithe youthful figure appearing about twenty-five, sharp angular face with a narrow chin, olive skin, dark glittering eyes under arched black brows, short cropped black hair, beardless, bare head, a long wine-red robe darkening to black at the hem, a black silk sash, bare feet, large charcoal-black feathered wings folded behind the shoulders, holding a small heap of gold coins in an open right palm, rendered as a solid fully opaque figure, sly tempting smile. Right column, captioned \"Old Man\": a small frail man about seventy-five, thin kind face deeply wrinkled, bright clear pale blue eyes, a long full white beard reaching the chest, long thin white hair, bare head, a simple undyed grey-brown wool robe to the ankles, a plain rope belt, worn leather sandals, a small plain wooden cross on a cord around his neck, both hands resting on a plain wooden walking staff, gentle compassionate expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#F2EDE3", "#5A1424", "#8A7E6A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Good Angel\", \"Bad Angel\", \"Old Man\""
}
```

**Identity lines:**

- Good Angel: `Good Angel, tall youthful figure, gentle oval face, calm blue eyes, golden-blond shoulder-length curls, ivory-white linen robe with gold hem, large white feathered wings, hands clasped`
- Bad Angel: `Bad Angel, tall lithe youthful figure, sharp angular olive face, dark glittering eyes, short cropped black hair, sly smile, wine-red robe darkening to black, large charcoal-black feathered wings, gold coins in open palm`
- Old Man: `the Old Man, small frail man about seventy-five, kind deeply wrinkled face, bright pale blue eyes, long full white beard, long thin white hair, undyed grey-brown wool robe, rope belt, wooden walking staff, small wooden cross`

**Note:** The three voices of conscience are grouped together. The two angels are deliberately opposite: golden hair against black, white robe against wine-red, white wings against black.

---

### Type B 2: Valdes · Cornelius · First Scholar; scenes 1 and 2

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Group_Valdes_Cornelius_FirstScholar.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Valdes\": Valdes, a heavy-set magician about forty-five, broad florid face, thick black eyebrows, dark brown eyes, black curly hair, a full thick black beard, a black felt hat with a narrow brim, a dark blue velvet doublet with tight sleeves, a short black wool cape over one shoulder, black hose, black leather boots to the calf, a gold ring with a large dark red stone, holding a dark carved walnut staff, knowing persuasive expression. Middle column, captioned \"Cornelius\": Cornelius, a thin small man about fifty-five, sharp hawk-like face, a hooked nose, pale green eyes under heavy lids, bald on top with short grey hair at the sides, a short pointed grey goatee, a black skullcap, a long ochre-brown wool gown lined with grey squirrel fur, a brown leather belt with a small brass-bound pouch, brown leather shoes, holding two rolled parchments tied shut with cord, sly calculating expression. Right column, captioned \"First Scholar\": a tall gangly student about twenty-two, long thin face, prominent nose, grey eyes, light brown hair falling to the jaw, a sparse wispy light brown beard, a black wool student's flat cap, a knee-length black wool student gown open at the front, a grey wool doublet beneath, grey hose, black leather shoes, anxious frowning expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#1F2A44", "#8A6A3A", "#161616", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Valdes\", \"Cornelius\", \"First Scholar\""
}
```

**Identity lines:**

- Valdes: `Valdes, heavy-set magician about forty-five, broad florid face, black curly hair, full thick black beard, black narrow-brim hat, dark blue velvet doublet, short black cape, red-stone gold ring, carved walnut staff`
- Cornelius: `Cornelius, thin small man about fifty-five, sharp hawk-like face, hooked nose, pale green eyes, bald on top with grey sides, pointed grey goatee, black skullcap, ochre-brown gown lined with grey fur, rolled tied parchments`
- First Scholar: `First Scholar, tall gangly student about twenty-two, long thin face, prominent nose, grey eyes, jaw-length light brown hair, wispy beard, black student cap and knee-length black gown over grey doublet`

**Note:** Valdes and Cornelius are deliberately different: one heavy with a thick black beard in blue and black, the other thin and bald with a grey goatee in ochre. Cornelius's "bald crown" was changed to "bald on top" so the model does not read it as a crown.

---

### Type B 3: Second Scholar · Third Scholar · Fourth Scholar; scenes 2, 11 and 12

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Group_Scholars.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Second Scholar\": a short stocky student about twenty, round broad face, small snub nose, warm brown eyes, cropped dark red hair, clean-shaven, bare head, a knee-length dark brown wool student gown, a blue-grey wool doublet beneath, dark brown hose, brown leather shoes, holding a small closed book with a plain leather cover, earnest determined expression. Middle column, captioned \"Third Scholar\": a slim student about twenty-four, fine-boned pale face, pale blue eyes, long straight blond hair to the shoulders, a thin blond moustache, bare head, a knee-length deep blue wool student gown trimmed with black velvet, a black doublet beneath, dark grey hose, black shoes, holding a small closed prayer book with a dark leather cover, gentle troubled expression. Right column, captioned \"Fourth Scholar\": a broad-shouldered student about twenty-six, olive complexion, strong square face, thick dark eyebrows, dark brown eyes, short black curly hair, clean-shaven with a dark stubble shadow, a black student flat cap, a knee-length maroon-brown wool student gown, a mustard-yellow wool doublet beneath, brown hose, brown leather shoes, serious alarmed expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#4A3426", "#22365A", "#5A2A24", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Second Scholar\", \"Third Scholar\", \"Fourth Scholar\""
}
```

**Identity lines:**

- Second Scholar: `Second Scholar, short stocky student about twenty, round broad face, snub nose, warm brown eyes, cropped dark red hair, clean-shaven, bareheaded, dark brown knee-length gown over blue-grey doublet, small closed book`
- Third Scholar: `Third Scholar, slim student about twenty-four, fine-boned pale face, pale blue eyes, long straight blond hair, thin blond moustache, deep blue knee-length gown trimmed with black velvet, small closed prayer book`
- Fourth Scholar: `Fourth Scholar, broad-shouldered student about twenty-six, olive square face, thick dark eyebrows, dark brown eyes, short black curly hair, dark stubble, black student cap, maroon-brown gown over mustard-yellow doublet`

**Note:** The students of scene 2 differ from those of scenes 11 and 12, because twenty-four years pass between them. Grouping the students together makes it easy to check that all four look clearly different.

---

### Type B 4: The Clown · Baliol · Belcher; scene 4

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Group_Clown_Baliol_Belcher.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"The Clown\": a scrawny peasant boy about sixteen, hollow cheeks, a smudged dirty face, large protruding ears, wide frightened brown eyes, unruly straw-blond hair sticking up, beardless, bare head, a ragged patched grey-brown wool tunic with holes at the elbows, frayed brown hose torn at one knee, a rope tied as a belt, bare dirty feet, hungry wary expression. Middle column, captioned \"Baliol\": a squat pot-bellied imp about the height of a child, mottled dark green-grey warty skin, a wide flat toad-like head, two short stubby horns, bulging yellow eyes, a very wide grinning mouth with small pointed teeth, large pointed bat-like ears, short thick arms with three-fingered clawed hands, short bowed legs with clawed feet, a thin whip-like tail, a scrap of dark leather around the waist, rendered as a solid fully opaque figure, crouched playful pose, gleeful menacing grin. Right column, captioned \"Belcher\": a tall thin demon with goat features, rust-red leathery skin, a long narrow face, a long scraggly black goat beard, two backward-curving black goat horns, small glittering black eyes, long pointed ears, wiry arms with long clawed fingers, furry black goat legs from the hips down ending in cloven hooves, a long thin tail with a black tuft, rendered as a solid fully opaque figure, loose mocking pose, leering expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#6B5E4E", "#3E4A3A", "#8A3A24", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"The Clown\", \"Baliol\", \"Belcher\""
}
```

**Identity lines:**

- The Clown: `the Clown, scrawny peasant boy about sixteen, hollow smudged face, big ears, wide frightened brown eyes, unruly straw-blond hair, ragged patched grey-brown tunic, rope belt, bare feet`
- Baliol: `Baliol, squat pot-bellied toad-like imp, mottled dark green-grey warty skin, short stubby horns, bulging yellow eyes, wide toothy grin, bat-like ears, whip-like tail`
- Belcher: `Belcher, tall thin goat-like demon, rust-red leathery skin, long scraggly black goat beard, backward-curving black horns, small black eyes, furry black goat legs with cloven hooves, tufted tail`

**Note:** Baliol and Belcher are deliberately opposite: short, green and toad-like against tall, red and goat-like. The devils who dance in scene 5 and carry Faustus away in scene 12 can be built from these two.

---

### Type B 5: Demon Bride · Lucifer · Beelzebub; scenes 5 and 7

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Group_DemonBride_Lucifer_Beelzebub.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Demon Bride\": a demon dressed as a woman, tall and broad-shouldered with a mannish jaw, a face caked in heavy white paint with crude round red rouge on the cheeks and smeared red lips, small glowing red eyes, a coarse black wig of thick braids slightly askew topped by a crooked tin bridal wreath of false flowers, an ill-fitting high-waisted bridal gown of tarnished ivory silk with puffed sleeves straining at the seams, large clawed grey hands, dark cloven hooves showing beneath the hem, rendered as a solid fully opaque figure, awkward coy pose, grotesque simpering smile. Middle column, captioned \"Lucifer\": Lucifer, a very tall commanding figure appearing about fifty, cold handsome face with high cheekbones, pale ash-grey skin, burning crimson eyes, long straight black hair to the shoulders, a sleek short black beard, two black horns rising from the brow, a crown of black iron spikes, a long black velvet robe with a deep blood-red lining and thin gold embroidery at the edges, large black leathery bat-like wings folded behind him, long pale hands holding a tall black iron sceptre, rendered as a solid fully opaque figure, cold contemptuous expression. Right column, captioned \"Beelzebub\": Beelzebub, a heavy bloated demon appearing about sixty, sickly yellow-green skin, a bald round head with two short stubby horns, very large glossy black insect-like eyes, heavy jowls, a thick neck, a small cruel mouth, a pair of small iridescent fly wings on his back, a long dark bronze-green brocade robe straining over a large belly, a heavy gold chain of office, gold rings on fat fingers, rendered as a solid fully opaque figure, greedy smug expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#D8CDB4", "#6A0F14", "#9A9A4A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Demon Bride\", \"Lucifer\", \"Beelzebub\""
}
```

**Identity lines:**

- Demon Bride: `demon dressed as a bride, tall broad-shouldered, heavy white face paint with crude red rouge, small glowing red eyes, coarse black braided wig askew, ill-fitting tarnished ivory silk gown, tin flower wreath, clawed grey hands, cloven hooves`
- Lucifer: `Lucifer, very tall regal figure, cold handsome ash-grey face, burning crimson eyes, long straight black hair, sleek black beard, black horns, black iron spiked crown, black velvet robe lined blood-red, black leathery wings, black iron sceptre`
- Beelzebub: `Beelzebub, bloated demon lord, sickly yellow-green skin, bald head with stubby horns, large glossy black insect eyes, heavy jowls, small iridescent fly wings, bronze-green brocade robe, heavy gold chain`

**Note:** The three greater demons are grouped together. Lucifer's iron crown is deliberate and is described explicitly.

---

### Type B 6: Pride · Covetousness · Wrath; scene 7

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Group_Pride_Covetousness_Wrath.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Pride\": a tall slender man about thirty, pale powdered face, a haughty raised chin, half-closed disdainful blue eyes, carefully curled golden hair to the shoulders, a thin upturned moustache, a jewelled blue velvet flat cap with a peacock feather, an extravagant peacock-blue and gold slashed silk doublet with huge puffed sleeves, a high standing lace-edged collar, gold-striped hose, gold velvet shoes, holding an oval hand mirror in a gilded frame, vain posing stance, admiring himself. Middle column, captioned \"Covetousness\": a wizened hunched old man about seventy, small sharp face, a long beaky nose, small greedy darting black eyes, thin white stubble, a few strands of white hair, bare head, a threadbare mustard-brown wool gown patched many times, a ring of many iron keys at the belt, clutching a bulging old leather money bag in both bony hands against his chest, suspicious greedy expression. Right column, captioned \"Wrath\": a burly muscular man about thirty-five, flushed red face, a deep scowl, bared clenched teeth, glaring light brown eyes, wild bristling red hair and a wild red beard, bare head, bare muscular arms, a scorched and torn black leather jerkin, rust-red hose, heavy black boots, holding two sheathed rapiers crossed in front of his chest, tense aggressive stance, furious expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#1F5A73", "#9A7A2E", "#A0301E", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Pride\", \"Covetousness\", \"Wrath\""
}
```

**Identity lines:**

- Pride: `Pride, tall slender vain man about thirty, pale powdered face, raised chin, curled golden hair, peacock-blue and gold slashed silk doublet, high lace collar, peacock feather cap, gilded hand mirror`
- Covetousness: `Covetousness, wizened hunched old man about seventy, beaky nose, small greedy black eyes, white stubble, threadbare patched mustard-brown gown, iron key ring, clutching a bulging leather money bag`
- Wrath: `Wrath, burly muscular man about thirty-five, flushed scowling face, wild bristling red hair and beard, bare muscular arms, scorched torn black leather jerkin, two sheathed rapiers crossed`

**Note:** The first three of the Seven Deadly Sins, in the order they appear in the play.

---

### Type B 7: Envy · Gluttony · Sloth; scene 7

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Group_Envy_Gluttony_Sloth.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Envy\": a gaunt woman about forty, sallow skin with a faint greenish pallor, sunken bitter dark eyes, tight pursed thin lips, sharp cheekbones, lank black hair escaping a dull grey linen coif, a ragged dull olive-green wool gown, thin arms wrapped tightly around herself, bare bony feet, hunched closed stance, resentful sidelong glare. Middle column, captioned \"Gluttony\": an enormously stout man about fifty, round shiny ruddy face, a triple chin, small eyes sunk in fat cheeks, greasy thin brown hair, bare head, a food-stained dull orange wool doublet unbuttoned over a straining linen shirt, wide brown breeches, a grease-spotted white linen napkin tucked at the collar, holding a large pewter tankard in one hand and a roasted drumstick in the other, belly pushed forward, satisfied hungry expression. Right column, captioned \"Sloth\": a soft puffy young man about twenty-five, pale doughy face, heavy-lidded half-closed grey eyes, mouth caught mid-yawn, tousled flattened light brown hair, bare head, a rumpled long grey linen nightshirt under a loose shabby brown wool robe hanging off one shoulder, bare feet, dragging a straw-stuffed linen pillow in one hand, slumped drooping pose, drowsy expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#5E6B3A", "#B8682E", "#9A968C", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Envy\", \"Gluttony\", \"Sloth\""
}
```

**Identity lines:**

- Envy: `Envy, gaunt woman about forty, sallow greenish pallor, sunken bitter dark eyes, pursed thin lips, lank black hair under grey coif, ragged dull olive-green gown, arms wrapped around herself`
- Gluttony: `Gluttony, enormously stout man about fifty, round shiny ruddy face, triple chin, greasy thin brown hair, food-stained dull orange doublet, napkin at the collar, pewter tankard and roasted drumstick`
- Sloth: `Sloth, soft puffy young man about twenty-five, pale doughy face, heavy half-closed grey eyes, mid-yawn, tousled light brown hair, rumpled grey nightshirt under shabby brown robe, bare feet, straw pillow`

**Note:** The next three of the Seven Deadly Sins.

---

### Type B 8: Lechery · Helen of Troy · Alexander's Paramour; scenes 7, 10 and 11

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Group_Lechery_Helen_Paramour.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Lechery\": a woman about thirty, heavily rouged cheeks, painted red lips, kohl-lined sly green eyes, loose long auburn hair crowned with red roses, a crimson velvet gown with a laced bodice and a modest square neckline edged in gold braid, long trailing sleeves, a gold ring on every finger, holding a single red rose, languid swaying pose, sly inviting smile. Middle column, captioned \"Helen of Troy\": Helen of Troy, a tall graceful young woman about twenty-two, luminous fair golden skin, delicate oval face, large grey-green eyes, long wavy golden-auburn hair partly braided with small pearls, a thin gold diadem, a long white silk chiton with a gold-embroidered border falling to the feet, gold armbands, gold sandals, rendered as a solid fully opaque figure, calm graceful pose, enigmatic faint smile. Right column, captioned \"Alexander's Paramour\": a graceful woman about twenty-five, olive skin, oval face, large dark almond-shaped eyes, dark curled hair gathered up and bound with a thin gold fillet, small gold hoop earrings, a long saffron-yellow linen chiton belted high, a deep blue himation draped over one shoulder, gold armbands, simple leather sandals, rendered as a solid fully opaque figure, calm graceful pose, serene remote expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#8A1426", "#F2ECE0", "#D9A23A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Lechery\", \"Helen of Troy\", \"Alexander's Paramour\""
}
```

**Identity lines:**

- Lechery: `Lechery, woman about thirty, heavily rouged cheeks, painted red lips, sly green eyes, loose auburn hair crowned with red roses, crimson velvet laced gown with gold braid, single red rose`
- Helen of Troy: `Helen of Troy, tall graceful young woman about twenty-two, luminous golden skin, delicate oval face, large grey-green eyes, long wavy golden-auburn hair braided with pearls, thin gold diadem, white silk chiton with gold border`
- Alexander's Paramour: `spirit of Alexander's paramour, graceful olive-skinned woman about twenty-five, large dark almond eyes, dark curled hair bound with gold fillet, saffron-yellow chiton, deep blue himation, gold armbands`

**Note:** The three women are grouped so they can be told apart clearly: auburn hair and crimson, golden hair and white, dark hair and saffron. Lechery is the last of the Seven Deadly Sins. Helen and the paramour are spirits: in the shots, add `faint unearthly glow` to their identity lines, but do not make Helen translucent, because Faustus kisses her.

---

### Type B 9: The Pope · Cardinal of Lorraine · Papal Friar; scene 8

**Size in the node:** 1536 × 1280 · **File name:** `CHR_Group_Pope_Cardinal_Friar.png`

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"The Pope\": a heavy-set man about sixty-five, jowly florid face, small shrewd dark eyes, a fleshy nose, clean-shaven, short white hair, a red velvet fur-trimmed papal cap, a red velvet shoulder cape trimmed with white ermine, a white lace-edged linen surplice over a long white silk cassock, a large gold pectoral cross on a gold chain, a heavy gold ring with a red stone, red velvet slippers, self-satisfied expression. Middle column, captioned \"Cardinal of Lorraine\": a thin tall man about forty, narrow ascetic face, a sharp aquiline nose, cool watchful hazel eyes, clean-shaven, short dark hair, a square scarlet four-ridged cardinal's cap, a scarlet silk cassock to the floor, a short scarlet shoulder cape, a plain gold pectoral cross on a red cord, scarlet gloves, black shoes, guarded calculating expression. Right column, captioned \"Papal Friar\": a plump short man about thirty-five, round pink face, small worried blue eyes, a double chin, clean-shaven, a shaved tonsure with a ring of light brown hair, a white wool Dominican habit with a white scapular, a long black wool cloak with the black hood down, a black leather belt with simple wooden beads, black shoes, holding a small bronze handbell in one hand and a tall unlit white beeswax candle in the other, anxious pious expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#9A1C22", "#B01E28", "#F0ECE2", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"The Pope\", \"Cardinal of Lorraine\", \"Papal Friar\""
}
```

**Identity lines:**

- The Pope: `the Pope, heavy-set man about sixty-five, jowly florid clean-shaven face, small shrewd dark eyes, red fur-trimmed papal cap, red velvet ermine-trimmed shoulder cape, white lace surplice over white cassock, large gold pectoral cross`
- Cardinal of Lorraine: `Cardinal of Lorraine, thin tall man about forty, narrow ascetic clean-shaven face, aquiline nose, watchful hazel eyes, square scarlet cardinal's cap, scarlet cassock and short cape, gold cross on red cord`
- Papal Friar: `papal friar, plump short man about thirty-five, round pink clean-shaven face, worried blue eyes, light brown tonsure, white Dominican habit under black cloak, bronze handbell and tall unlit candle`

**Note:** Here the titles in the captions match the costumes that are wanted, so they are kept. The Pope and the Cardinal are deliberately different: old, heavy, white and red against younger, thin and all scarlet. The friar wears the white and black of a Dominican so he is not confused with Mephistopheles's grey-brown habit.

---

### Type B 10: Charles the Fifth · Alexander the Great; scene 10

**Size in the node:** 1024 × 1536 · **File name:** `CHR_Group_CharlesV_Alexander.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"Charles the Fifth\": Charles the Fifth, a slim man of medium height about thirty-five, pale skin, a long face with a prominent jutting lower jaw, a short dark blond-brown beard covering the jaw, short cropped hair, grave blue-grey eyes, a black velvet flat cap, a black satin doublet, a long black velvet gown with a wide sable collar, a gold collar of linked flints with a small golden ram pendant on the chest, black hose, black velvet shoes, holding a pair of fine leather gloves, grave curious expression. Right column, captioned \"Alexander the Great\": the spirit of Alexander the Great, an athletic young man about thirty, clean-shaven, a strong jaw, intense deep-set eyes, tousled golden-brown curly hair swept up from the forehead, bare head, a bronze muscled cuirass over a short white linen tunic, a leather strip skirt, a deep purple wool cloak pinned at the right shoulder, bronze greaves, laced leather sandals, holding a crested bronze helmet under the left arm, rendered as a solid fully opaque figure, distant commanding expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#0E0E10", "#C9A44C", "#4A2A5A", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"Charles the Fifth\", \"Alexander the Great\""
}
```

**Identity lines:**

- Charles the Fifth: `Emperor Charles the Fifth, slim man about thirty-five, pale long face with prominent jutting jaw, short dark blond-brown beard, grave blue-grey eyes, black velvet cap, black velvet gown with sable collar, gold collar with golden ram pendant`
- Alexander the Great: `spirit of Alexander the Great, athletic clean-shaven young man about thirty, strong jaw, tousled golden-brown curls swept up from the forehead, bronze muscled cuirass, purple cloak, bronze greaves, crested helmet under left arm`

**Note:** The caption is "Charles the Fifth", not "Emperor", so the model does not add a crown. The emperor's real portraits show the long jutting jaw described here. The gold collar is the Order of the Golden Fleece. In the shots, add `faint unearthly glow` to Alexander's identity line.

---

### Type B 11: The Vintner · The Horse-courser; scenes 9 and 10

**Size in the node:** 1024 × 1536 · **File name:** `CHR_Group_Vintner_HorseCourser.png`

```json
{
  "prompt": "A character reference image arranged in a grid of two columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"The Vintner\": a burly innkeeper about fifty, broad red-cheeked face, a bald shiny head with a fringe of black hair, a thick black drooping moustache, angry dark eyes, a thick neck, the sleeves of an off-white linen shirt rolled to the elbows over hairy forearms, a dark brown wool waistcoat, a long leather apron stained purple with wine, brown breeches, heavy shoes, fists on hips, indignant angry expression. Right column, captioned \"The Horse-courser\": a wiry horse dealer about forty-five, weather-beaten tanned face, a crooked nose, cunning narrow grey eyes, a short grizzled grey-brown beard, a battered wide-brimmed brown felt hat, a long brown leather riding coat with a cracked surface, a dark green wool doublet beneath, brown breeches, tall mud-splattered riding boots, a coiled leather riding whip in the right hand, shifty relaxed stance, shrewd bargaining expression. The captions are the only text in the image.",
  "style": "Cinematic photograph, historical drama, German Renaissance, Holy Roman Empire around 1535, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
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
    "palette": ["#5A3A2A", "#6B1E2E", "#3A4A32", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Two equal columns, two rows. Top row: two front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: two front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"The Vintner\", \"The Horse-courser\""
}
```

**Identity lines:**

- The Vintner: `the Vintner, burly bald man about fifty, red-cheeked face, thick black drooping moustache, rolled linen sleeves, dark brown waistcoat, long leather apron stained purple with wine`
- The Horse-courser: `the Horse-courser, wiry man about forty-five, weather-beaten tanned face, crooked nose, cunning narrow grey eyes, grizzled beard, battered wide-brimmed brown felt hat, long brown leather riding coat, muddy riding boots, coiled whip`

**Note:** The two remaining characters, both tradesmen cheated by magic, are placed in a two-column image.

---

## Part 4: Notes

- **Image list:** seventeen images for 44 character states. Type A: Faustus (three ages), Wagner (two ages), Mephistopheles (demon and friar), Robin (man and ape), Rafe (man and dog), the Knight (with and without antlers). Type B: the two angels and the Old Man; Valdes, Cornelius and the First Scholar; the other three scholars; the Clown and Wagner's two devils; the Demon Bride, Lucifer and Beelzebub; the Seven Deadly Sins in three images; the Pope, the Cardinal and the friar; Charles the Fifth and Alexander; the Vintner and the Horse-courser.
- **Characters without a sheet:** Christ, Jupiter, Apollo, Diana, the Rector of the university and the kitchen maid are only named in quotations or in passing and are never seen. The Chorus is only a voice at the end.
- **Spirits:** Alexander, his paramour and Helen are spirits that Faustus conjures. In their shot prompts, add `faint unearthly glow` to the identity line. Do not make Helen translucent, because Faustus kisses her.
- **Captions:** captions are personal names or costume-neutral roles. Titles such as Emperor, Prince or King are left out because they add crowns and robes. The Pope and the Cardinal keep their titles because their costumes are meant to match.
- **Before use as a reference:** crop the caption strip off the image so the text does not leak into the shots. In each shot, pass only the column of the state the shot needs.
- **Keeping the face consistent in Type A:** if the face differs between the columns of one image, pass the first column's close-up as a reference and generate the image again.
- **Changes from the previous version:** the 44 six-panel sheets (front, three-quarter and profile) were converted to the new front-view format with captions and merged into seventeen images; all prompts were moved from the old fields (`scene`, `subjects`, `color_palette`, `mood`, `background`) to the node fields; the word `still` was removed from every pose; Cornelius's "bald crown" became "bald on top"; headwear is now described explicitly in every column.