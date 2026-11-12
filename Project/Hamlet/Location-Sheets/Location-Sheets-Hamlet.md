پرامپت‌های مرجع مکان‌ها و وسایل کلیدی **هملت**. رشته style و Lookها همان‌هایی است که در بخش اول سند شیت شخصیت‌ها (`character-sheet/character-sheet.md`) آمده است. همهٔ پرامپت‌ها با فیلدهای نود `Template/flux2-prompt-node-v2.html` نوشته شده‌اند.

**اندازه پیشنهادی در نود:**

- مکان‌ها: ۱۹۲۰ در ۱۲۸۰، تا هر پنل در شبکهٔ دو در دو نسبت ۳ به ۲ سینمایی داشته باشد.
- وسایل: ۱۵۳۶ در ۱۵۳۶، تا هر پنل مربع باشد.

## مکان‌ها

### ۱. نمای بیرونی قلعهٔ اِلسینور کنار دریا؛ صحنه‌های ۱، ۳، ۹، ۱۰ و ۱۲

```json
{
  "prompt": "A four-panel location reference of a Danish Renaissance castle on the sea around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A large four-winged sandstone castle in Dutch Renaissance style on a low headland at the narrow strait of the sea, towers of different heights with pointed copper-green spires and copper roofs, rows of tall windows with carved sandstone surrounds, a closed inner courtyard, wide low earthen ramparts and stone bastions with bronze cannons in embrasures, a water-filled moat with a bridge and gatehouse, black rocks and surf at the foot of the seaward wall. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level, slightly high over the water",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: cold moonlight through drifting sea mist, a few small warm points of lantern light in the windows, black water. Bottom right panel: flat grey overcast morning light, calm grey sea",
  "colors": {
    "palette": [
      "#0B1A2A",
      "#2E4A62",
      "#A9C1D3",
      "#E6EEF2"
    ],
    "mood": "cold, ominous, majestic"
  },
  "composition": "Top left: wide establishing view from the sea toward the castle across the water. Top right: reverse view from the gatehouse bridge looking out over the ramparts to the open sea. Bottom left: close detail of materials, pale sandstone blocks with carved window surrounds, green verdigris copper roof sheets and weathered rivets. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

**یادداشت:** معماری بر اساس قلعهٔ واقعی کرونبورگ است. یک عکس واقعی از کرونبورگ را هم به‌عنوان مرجع بدهید.

---

### ۲. باروی رو به دریا؛ صحنه‌های ۱، ۳ و پایان ۱۲

```json
{
  "prompt": "A four-panel location reference of the seaward rampart walk of a Danish Renaissance castle around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A long stone walkway on top of the rampart between low battlements and embrasures, a row of bronze cannons on wooden carriages pointing out to sea, worn wet flagstones, a squat corner tower with a small arched stair door, an iron bracket for a lantern, the copper spires of the castle rising behind. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "28mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: cold full moonlight through drifting sea mist, a small warm glow from an iron lantern bracket. Bottom right panel: blue-hour dawn, thinning mist, the first warm line on the sea horizon",
  "colors": {
    "palette": [
      "#0B1A2A",
      "#2E4A62",
      "#A9C1D3",
      "#E6EEF2"
    ],
    "mood": "cold, expectant, lonely"
  },
  "composition": "Top left: wide establishing view along the walkway with the cannons receding toward the corner tower. Top right: reverse view from the corner tower back along the walkway toward the castle spires. Bottom left: close detail of materials, rough battlement stone with lichen, a bronze cannon barrel with green patina, worn flagstones glistening with damp. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

**یادداشت:** پانل چهارم Look سپیده‌دم صحنه‌های ۱ و ۳ را می‌دهد. پالت آن: `#1B2735` `#4F6A86` `#C9B79C` `#F2E6D0`.

---

### ۳. برج ناقوس؛ صحنهٔ ۱

```json
{
  "prompt": "A four-panel location reference of the open belfry of a castle tower around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A square bell chamber at the top of a stone tower, a heavy weathered bronze bell with green patina hanging from dark oak beams, a thick iron clapper, wooden louvred openings on all four sides, a rough wooden floor with a trapdoor, pigeon feathers and dust. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "low angle, looking up",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: thin pale moonlight slicing through the louvres in narrow beams. Bottom right panel: flat grey daylight through the louvres",
  "colors": {
    "palette": [
      "#0B1A2A",
      "#2E4A62",
      "#A9C1D3",
      "#E6EEF2"
    ],
    "mood": "foreboding, solemn"
  },
  "composition": "Top left: wide establishing view from the trapdoor looking up at the bell and beams. Top right: reverse view from beside the bell looking out through the louvres over the castle roofs. Bottom left: close detail of materials, green-patinated bronze, iron clapper and pegged oak beams with old dust. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

---

### ۴. کارگاه توپ‌ریزی؛ صحنهٔ ۱

```json
{
  "prompt": "A four-panel location reference of a sixteenth-century cannon foundry, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A tall smoky timber-roofed workshop with a brick furnace, a deep casting pit in the earth floor with clay moulds for gun barrels buried upright, an iron-banded crucible hanging from a wooden crane, finished bronze cannon barrels lying on wooden trestles, long iron poles, buckets and piles of charcoal. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: fierce orange glow from the furnace mouth and molten metal, everything else in deep smoky shadow. Bottom right panel: cold grey morning daylight through roof vents, the furnace dark and cooling",
  "colors": {
    "palette": [
      "#120A06",
      "#7A2E0E",
      "#E8731C",
      "#FFC56B"
    ],
    "mood": "urgent, industrious, war preparation"
  },
  "composition": "Top left: wide establishing view from the doorway across the casting pit toward the furnace. Top right: reverse view from behind the furnace looking back to the open doorway. Bottom left: close detail of materials, rough clay mould surfaces, scorched brick, a cooling bronze barrel with casting seams. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

---

### ۵. تالار بزرگ دربار با تخت سلطنت؛ صحنه‌های ۲، ۴، ۹ و ۱۲

```json
{
  "prompt": "A four-panel location reference of the great hall of a Danish Renaissance castle around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A very long hall with a stone floor, a row of tall leaded windows along one side, the opposite wall hung with large woven tapestries of kings and hunting scenes, a heavy coffered oak ceiling, a raised dais at the far end with two carved high-backed thrones under a deep red canopy, tall iron candelabra, wall torches in iron brackets, and tall double oak doors with heavy iron bands at the near end. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: grey northern daylight through the leaded windows in long shafts across the floor. Bottom right panel: evening festive light from wall torches and lit candelabra, warm gold on the canopy and tapestries",
  "colors": {
    "palette": [
      "#2B2B2E",
      "#5C5A55",
      "#A39E93",
      "#D9D3C7"
    ],
    "mood": "grand, cold, watchful"
  },
  "composition": "Top left: wide establishing view from the doors down the length of the hall to the thrones. Top right: reverse view from beside the thrones back toward the double doors. Bottom left: close detail of materials, woven tapestry threads, carved gilded throne arm, iron door bands and worn flagstones. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

**یادداشت:** پانل چهارم Look جشن صحنهٔ ۲ را می‌دهد (`#1A0F0A` `#6E2A1A` `#C99A4A` `#EEDFC2`). برای صحنهٔ ۱۲ همین تالار را با میز جام‌ها و فضای خالی مسابقه در وسط توصیف کنید.

---

### ۶. راهروها و گالری قلعه؛ صحنه‌های ۴، ۵ و ۷

```json
{
  "prompt": "A four-panel location reference of the long gallery and corridors of a Danish Renaissance castle around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A long gallery with oak-panelled walls and a row of tall leaded windows with deep stone sills, a plain stone floor, a few carved oak chests and benches, arched stone doorways opening onto darker corridors, an iron wall sconce with a candle. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "28mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: grey daylight through the windows in alternating bands of light and shadow. Bottom right panel: night, the gallery dark, a few candles in iron sconces and a warm slice of light from an open doorway",
  "colors": {
    "palette": [
      "#2B2B2E",
      "#5C5A55",
      "#A39E93",
      "#D9D3C7"
    ],
    "mood": "quiet, watchful, cool"
  },
  "composition": "Top left: wide establishing view down the length of the gallery in one-point perspective. Top right: reverse view from the far end back toward the windows. Bottom left: close detail of materials, oak panelling grain, leaded window lines and a worn stone sill. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

---

### ۷. تالار خلوت با فرش دیواری؛ صحنهٔ ۵

```json
{
  "prompt": "A four-panel location reference of a quiet empty hall in a Danish Renaissance castle around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A tall bare hall with one very tall leaded window, a simple wooden prayer stool in front of it, a huge faded wool tapestry of a hunting scene covering most of one wall and hanging a little away from it so that a narrow dark space hides behind, a plain stone floor, an arched doorway at the end leading to a brighter corridor. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: cool overcast daylight from the tall window, the rest of the hall in soft shadow. Bottom right panel: dusk, the window deep blue, the hall almost dark",
  "colors": {
    "palette": [
      "#1F2226",
      "#4A4E52",
      "#8F948F",
      "#D6D2C4"
    ],
    "mood": "quiet, tense, watched"
  },
  "composition": "Top left: wide establishing view from the doorway toward the window, the prayer stool and the tapestry. Top right: reverse view from beside the tapestry looking back to the doorway. Bottom left: close detail of materials, faded tapestry wool, the narrow dark gap behind it, and the worn wood of the prayer stool. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

---

### ۸. تالار اجرای نمایش؛ صحنه‌های ۴ و ۶

```json
{
  "prompt": "A four-panel location reference of a castle hall prepared for a play around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A large hall with a small raised wooden stage hung with dark red curtains and a row of candle footlights, a simple painted canvas backdrop of apple trees, rows of wooden stools and benches facing it, a canopied royal dais with two high-backed chairs at one side, deep red tapestries on the walls, wall torches in iron brackets and a high timber roof. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: night, warm torchlight and candle footlights, smoke haze under the beams. Bottom right panel: cold grey morning after, candles burnt out, stools overturned",
  "colors": {
    "palette": [
      "#120806",
      "#5A1E14",
      "#C8742E",
      "#F5D7A0"
    ],
    "mood": "theatrical, tense, festive"
  },
  "composition": "Top left: wide establishing view from the back of the audience toward the stage. Top right: reverse view from the stage looking out over the stools to the royal dais. Bottom left: close detail of materials, red stage curtain velvet, candle wax on the footlight rail and rough painted canvas. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

**یادداشت:** برای صحنهٔ ۴، بخشی از همین تالار با چند شمع روی زمین و بدون صحنه و صندلی استفاده می‌شود (Look تالار بازیگران: `#140C07` `#5E3A1C` `#C98A3E` `#F4D9A6`).

---

### ۹. حیاط و دروازهٔ قلعه؛ صحنه‌های ۴ و ۹

```json
{
  "prompt": "A four-panel location reference of the enclosed inner courtyard and gate of a Danish Renaissance castle around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A cobbled inner courtyard enclosed by four tall sandstone wings with rows of windows and a wooden gallery above, a deep arched gateway with heavy oak gates, iron torch brackets on the walls, a stone well in the middle. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "slightly high",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: dusk, deep blue sky, warm torches burning on the walls. Bottom right panel: flat overcast daylight with dust in the air",
  "colors": {
    "palette": [
      "#140C07",
      "#5E3A1C",
      "#C98A3E",
      "#F4D9A6"
    ],
    "mood": "busy, enclosed, restless"
  },
  "composition": "Top left: wide establishing view from the gallery above looking down at the courtyard and the gateway. Top right: reverse view from inside the gateway looking into the courtyard. Bottom left: close detail of materials, worn cobblestones, iron-studded oak gate and sandstone carving. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

---

### ۱۰. نمازخانهٔ خلوت کلادیوس؛ صحنهٔ ۷

```json
{
  "prompt": "A four-panel location reference of a small private chapel inside a castle around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A small low chapel with a ribbed stone vault, a plain stone altar with one candle and a plain wooden crucifix, a faded crimson prayer cushion on the floor before it, a weathered carved stone relief of two robed figures, one striking the other with a club, set into the side wall, a high narrow slit window, and a half-open arched door to a dark corridor. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: a single altar candle as the only warm light, deep black shadows, a thin cool beam of moonlight from the slit window. Bottom right panel: flat grey daylight from the slit window, the candle out",
  "colors": {
    "palette": [
      "#0D0B0A",
      "#3B2A1E",
      "#9C6B3A",
      "#E8C88F"
    ],
    "mood": "guilt, silence, confinement"
  },
  "composition": "Top left: wide establishing view from the doorway toward the altar. Top right: reverse view from the altar back toward the half-open door. Bottom left: close detail of materials, the carved stone relief, candle wax on the altar stone and the faded prayer cushion. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

**یادداشت:** نقش‌برجسته داستان قابیل و هابیل را نشان می‌دهد.

---

### ۱۱. اتاق ملکه؛ صحنهٔ ۸

```json
{
  "prompt": "A four-panel location reference of a Danish Renaissance queen's bedchamber around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A richly hung bedchamber with a large canopied bed with deep crimson hangings, a stone fireplace with a low fire, a heavy wool tapestry covering one whole wall and hanging in deep folds to the floor, a table with a silver candelabrum, a carved chair, dark floorboards with a worn rug, and a carved oak door. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: candlelight and firelight, rich warm shadows. Bottom right panel: pale grey early morning light through a small window, the fire out",
  "colors": {
    "palette": [
      "#0F0807",
      "#4A1A1C",
      "#A8552E",
      "#EBC79A"
    ],
    "mood": "intimate, oppressive, dangerous"
  },
  "composition": "Top left: wide establishing view from the door toward the bed, the fireplace and the tapestry wall. Top right: reverse view from beside the bed toward the door and the tapestry. Bottom left: close detail of materials, tapestry folds and fringe at the floor, crimson bed hangings and a silver candelabrum. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

---

### ۱۲. اتاق خصوصی پادشاه؛ صحنهٔ ۱۰

```json
{
  "prompt": "A four-panel location reference of a Danish Renaissance king's private room around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A small dark room panelled in oak, a heavy oak table with a cluster of candles in brass holders, two carved chairs, a shuttered window, a cabinet, and a stone fireplace with a dying fire. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: candles on the table as the main light, olive and brass tones, deep shadows. Bottom right panel: grey morning light leaking through the shutters, candles out",
  "colors": {
    "palette": [
      "#0B0D0B",
      "#2E3A2C",
      "#8A7A4A",
      "#D9C79A"
    ],
    "mood": "secretive, conspiratorial"
  },
  "composition": "Top left: wide establishing view from the door toward the table and shuttered window. Top right: reverse view from behind the table toward the door. Bottom left: close detail of materials, oak tabletop with wax drips, brass candleholders and a carved chair back. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

---

### ۱۳. باغ سلطنتی؛ فلش‌بک صحنهٔ ۳

```json
{
  "prompt": "A four-panel location reference of a walled royal orchard beside a castle around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A walled orchard of old apple trees with fallen apples in long grass, a stone bench under the largest tree, an old brick wall with a wooden gate, a gravel path, and a castle tower visible beyond the wall. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: hazy golden afternoon sun through the leaves, soft bloom like a memory. Bottom right panel: cool grey overcast morning",
  "colors": {
    "palette": [
      "#3E3A22",
      "#7D7A45",
      "#C9B57A",
      "#EFE3BF"
    ],
    "mood": "idyllic, false, remembered"
  },
  "composition": "Top left: wide establishing view toward the stone bench under the apple tree. Top right: reverse view from the bench toward the gate and the castle tower. Bottom left: close detail of materials, apple bark, fallen apples in the grass and the lichen-covered stone bench. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

**یادداشت:** پس‌زمینهٔ نقاشی‌شدهٔ صحنهٔ نمایش (صحنهٔ ۶) عمداً همین باغ را نشان می‌دهد.

---

### ۱۴. جویبار و درخت بید؛ صحنهٔ ۱۰

```json
{
  "prompt": "A four-panel location reference of a slow brook with an old willow in the Danish countryside, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. An old willow leaning out over a slow clear brook, long pale-green branches hanging to the water, reeds and wildflowers on the banks, a misty meadow beyond the far bank. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: soft green-gold early morning sun through the willow leaves, mist on the water. Bottom right panel: flat grey overcast light, the water dark",
  "colors": {
    "palette": [
      "#1F2A1C",
      "#4E6B3E",
      "#A8B77A",
      "#EEF0D8"
    ],
    "mood": "lyrical, fragile, quiet"
  },
  "composition": "Top left: wide establishing view from the opposite bank toward the leaning willow. Top right: reverse view from under the willow looking along the brook. Bottom left: close detail of materials, willow bark and leaves, reeds and the clear water surface over pebbles. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

---

### ۱۵. گورستان کلیسا؛ صحنه‌های ۹ و ۱۱

```json
{
  "prompt": "A four-panel location reference of an old churchyard near a Danish castle around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. An old churchyard with leaning weathered headstones with blank worn faces, a low stone church with a squat tower, dark yew trees, a low churchyard wall with a stone gate, wet grass, and one freshly dug open grave with mounds of dark earth. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: flat diffuse overcast light, faint mist between the stones. Bottom right panel: dusk, deep grey-blue light",
  "colors": {
    "palette": [
      "#1A1C1D",
      "#45494A",
      "#8A8F8C",
      "#CFD3CF"
    ],
    "mood": "melancholy, mortality"
  },
  "composition": "Top left: wide establishing view from the gate toward the church and the open grave. Top right: reverse view from beside the open grave back toward the gate. Bottom left: close detail of materials, wet dark earth, lichen on a blank weathered headstone and yew bark. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

**یادداشت:** سنگ‌قبرها عمداً صاف و ساییده‌اند تا هیچ نوشته‌ای در تصویر نیاید.

---

### ۱۶. بندر، دریا و ساحل؛ صحنه‌های ۹ و ۱۰

```json
{
  "prompt": "A four-panel location reference of the sea and a pebble shore near a Danish castle around 1600, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, completely empty of people. A grey sea strait with a small harbour below the castle, wooden quays and a moored three-masted merchant ship with grey sails, and further along the coast a lonely pebble beach with low dunes and a small rowing boat pulled up on the stones. The same place is shown in all four panels, empty and quiet, with no people and no figures.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level",
    "distance": "wide shot in the establishing and reverse views, close-up in the detail panel",
    "lens": "24mm for the wide views, 85mm for the detail panel",
    "f-number": "f/8 for the wide views, f/2.8 for the detail panel",
    "ISO": 200,
    "focus": "deep focus in the wide views, shallow focus in the detail panel"
  },
  "lighting": "Top left, top right and bottom left panels: stormy overcast light, choppy grey sea. Bottom right panel: cold pale dawn, calm sea",
  "colors": {
    "palette": [
      "#0C1416",
      "#2C4246",
      "#6F8A86",
      "#D8E0D8"
    ],
    "mood": "exile, return, desolate"
  },
  "composition": "Top left: wide establishing view from the beach toward the sea. Top right: reverse view from the sea toward the beach, the dunes and the distant castle. Bottom left: close detail of materials, wet pebbles, weathered boat planks and rope. Bottom right: the same establishing view as top left in the second light. Identical architecture and furniture placement in all four panels"
}
```

---

## وسایل کلیدی

### ۱. نیزهٔ پارتیزان و کلاه‌خود موریون نگهبان؛ صحنه‌های ۱، ۳ و ۹

```json
{
  "prompt": "A four-panel object reference of a late sixteenth-century guard's partisan spear and morion helmet, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A tall partisan spear with a broad triangular steel blade with two small side wings, on a long dark ash-wood shaft bound with iron at the base, lying beside a steel morion helmet with a high raised comb and a curved brim rising at front and back, small brass rivets around the edge. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#8C9399",
      "#5A3E2B",
      "#B08D57",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the partisan blade edge and the riveted brim of the helmet. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

---

### ۲. فانوس شاخی؛ صحنه‌های ۱ و ۳

```json
{
  "prompt": "A four-panel object reference of a sixteenth-century horn lantern, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A small tin lantern with a pierced conical top and a ring handle, its windows made of thin translucent amber horn panels, a small door with a latch, a short tallow candle inside, lit. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#7A6A58",
      "#D9A441",
      "#3B3A36",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the translucent horn panel and the candle flame glowing through it. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

---

### ۳. شمشیر هملت؛ صحنه‌های ۳، ۷ و ۸

```json
{
  "prompt": "A four-panel object reference of a late sixteenth-century gentleman's sword in its scabbard, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A straight double-edged sword with a plain steel crossguard, a small side ring, a leather-wrapped grip bound with wire and a round steel pommel, shown partly drawn from a black leather scabbard with steel fittings. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#8C9399",
      "#1A1A1A",
      "#5A3E2B",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the crossguard, wire-bound grip and pommel. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

---

### ۴. شیشهٔ زهر؛ صحنه‌های ۳، ۴، ۶ و ۱۰

```json
{
  "prompt": "A four-panel object reference of a small sixteenth-century poison vial, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A small hand-blown glass vial of dark green glass with a slightly uneven surface, a narrow neck sealed with a cork and a twist of waxed thread, half filled with dark liquid. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#1E3A2A",
      "#4A5A3A",
      "#8A7A4A",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the cork, the waxed thread and the dark liquid behind the glass. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

---

### ۵. تاج زرین دانمارک؛ صحنه‌های ۲، ۹ و ۱۲

```json
{
  "prompt": "A four-panel object reference of a Renaissance royal crown of Denmark, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A heavy gold crown with an open circlet of alternating tall fleurons and points, set with dark red stones and small pearls, a band of fine engraved scrollwork around the base, lined inside with dark red velvet. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#B8963E",
      "#7A1F24",
      "#EFE3BF",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the engraved gold band and a dark red stone in its setting. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

---

### ۶. تاج چوبی نمایش؛ صحنه‌های ۴ و ۶

```json
{
  "prompt": "A four-panel object reference of a painted wooden stage crown of a travelling acting troupe, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A simple crown carved from wood and painted gold, the gilt chipped and worn to bare wood in places, set with coloured glass jewels, one of them missing, a rough cloth lining. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#C9A44C",
      "#7A5A3A",
      "#B86B6B",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the chipped gilt, bare wood and a glass jewel. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

**یادداشت:** عمداً نسخهٔ ارزان و بدلی تاج شمارهٔ ۵ است؛ در شات‌های ۶۱۴ و ۱۲۱۴ این دو با هم قرینه می‌شوند.

---

### ۷. کتاب دعای اوفلیا؛ صحنهٔ ۵

```json
{
  "prompt": "A four-panel object reference of a small closed sixteenth-century prayer book, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A small thick prayer book bound in dark brown leather with blind-tooled borders, closed and fastened with a brass clasp, the page edges gilded. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#4A3424",
      "#B08D57",
      "#D9C79A",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the brass clasp and gilded page edges of the closed book. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

**یادداشت:** کتاب همیشه بسته است.

---

### ۸. هدیه‌های هملت به اوفلیا؛ صحنهٔ ۵

```json
{
  "prompt": "A four-panel object reference of a Renaissance pearl necklace and gold ring, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A single string of small white pearls with a gold clasp, lying in a loose curve beside a thin gold ring set with a small dark red stone. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#EFEDE6",
      "#B8963E",
      "#7A1F24",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the gold clasp and the ring's dark red stone. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

---

### ۹. دو مدال تصویردار؛ صحنهٔ ۸

```json
{
  "prompt": "A four-panel object reference of two open Renaissance portrait lockets side by side, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. On the left a small round silver locket open on a thin silver chain, holding a painted miniature of a gaunt older man with a dark beard streaked with silver; on the right a small oval gold locket open on a short string of pearls, holding a painted miniature of a robust man with a short dark beard and a gold crown. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#C0C4C8",
      "#B8963E",
      "#4A3424",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the two painted miniature faces. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

**یادداشت:** برای چهره‌های داخل مدال‌ها، شیت‌های `CHR_King_alive` و `CHR_Claudius` را به‌عنوان مرجع بدهید. مدال نقره‌ای همان آویز هملت و مدال طلایی همان آویز گردنبند گرترود است.

---

### ۱۰. کاغذ مهرشده و انگشتر مهر؛ صحنه‌های ۵ و ۱۰

```json
{
  "prompt": "A four-panel object reference of a folded and sealed sheet of heavy paper with a gold seal ring, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A sheet of heavy cream paper folded into a small rectangle with a plain blank outer face, sealed with a round blob of dark red wax bearing a simple crown impression, beside a heavy gold seal ring. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#E8DFC8",
      "#7A1F24",
      "#B8963E",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the wax seal and the face of the gold seal ring. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

**یادداشت:** کاغذ همیشه تاشده و با روی سفیدش دیده می‌شود.

---

### ۱۱. دستهٔ گل اوفلیا؛ صحنهٔ ۹

```json
{
  "prompt": "A four-panel object reference of a loose bunch of wild herbs and flowers, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A loose hand-gathered bunch of rosemary sprigs, purple and yellow pansies, small white daisies, fennel and a few faded withered violets, tied loosely with a strand of grass. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#3E6A3A",
      "#7A5C8C",
      "#E8E2D6",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the rosemary sprigs beside the withered violets. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

---

### ۱۲. دو شمشیر مسابقه؛ صحنه‌های ۱۰ و ۱۲

```json
{
  "prompt": "A four-panel object reference of two Renaissance fencing rapiers side by side, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. Two slim rapiers with swept steel hilts and wire-bound grips lying side by side: one has its point covered by a small round leather safety button tied with thread, the other has a bare freshly honed needle-sharp point. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#8C9399",
      "#2E3236",
      "#8A6A45",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the two tips side by side, the leather button and the bare point. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

**یادداشت:** در متن، شمشیر بی‌پوشش «unbated» نامیده می‌شود.

---

### ۱۳. جام زهر و مروارید؛ صحنه‌های ۱۰ و ۱۲

```json
{
  "prompt": "A four-panel object reference of a gilded Renaissance goblet with a large pearl, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A tall gilded silver goblet with a chased pattern of vines on the cup and a knopped stem, its domed lid set aside, and beside its foot a single large lustrous pearl on dark velvet. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#B8963E",
      "#EFEDE6",
      "#3A2B22",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the chased vine pattern and the pearl. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

---

### ۱۴. جمجمهٔ یوریک؛ صحنهٔ ۱۱

```json
{
  "prompt": "A four-panel object reference of an old earth-stained human skull, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A very old brown earth-stained human skull with a few worn teeth remaining in the upper jaw, no lower jaw, crumbs of dark soil in the eye sockets and seams. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#6B5A44",
      "#3A2E22",
      "#A8977A",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the upper jaw with its few worn teeth and soil in the hollows. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

---

### ۱۵. توپ مفرغی؛ صحنه‌های ۱، ۳ و ۱۲

```json
{
  "prompt": "A four-panel object reference of a late sixteenth-century bronze cannon on a wooden carriage, arranged in a two-by-two grid of equal panels separated by thin plain grey gaps, on a plain seamless light grey backdrop, with no hands and no people. A bronze cannon barrel with mouldings at the muzzle and breech and two dolphin-shaped lifting handles, mounted on a heavy wooden carriage with iron-bound wooden wheels. The same single object is shown in all four panels.",
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "camera": {
    "angle": "eye level for the front and three-quarter views, directly overhead for the top view",
    "distance": "full view of the object in three panels, close-up in the detail panel",
    "lens": "85mm, 100mm macro for the detail panel",
    "f-number": "f/11, f/4 for the detail panel",
    "ISO": 100,
    "focus": "the whole object sharp, shallow focus in the detail panel"
  },
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, soft gentle shadows",
  "colors": {
    "palette": [
      "#8A6A45",
      "#3E5A4A",
      "#5A3E2B",
      "#C9CCCF"
    ],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Top left: front view. Top right: three-quarter view. Bottom left: view from directly above. Bottom right: close detail of the dolphin-shaped handle and the green patina on the bronze. Object centred with generous empty grey space around it, identical object in all four panels"
}
```

**یادداشت:** همین توپ‌ها در شات آخر فیلم (۱۲۲۰) بی‌آنکه شلیک کنند روی بارو ایستاده‌اند.

---

**یادداشت‌ها:**

- **پانل‌ها:** در هر مکان، سه پانل اول نور اصلی صحنه را دارند و پانل چهارم همان نمای معرف را در نور دومی که فیلم لازم دارد نشان می‌دهد.
- **بدون آدم:** همهٔ مکان‌ها خالی‌اند تا مدل فقط معماری و فضا را یاد بگیرد. شخصیت‌ها را در شات‌ها با شیت خودشان اضافه کنید.
- **بدون نوشته:** سنگ‌قبرها صاف‌اند، کتاب بسته است و کاغذ تاشده با روی سفید دیده می‌شود.
- **مکان‌های یک‌باره:** سردابهٔ تندیس سنگی و دریای مه‌آلود با قایق خالی در صحنهٔ ۵ فقط یک بار دیده می‌شوند و مرجع جدا ندارند.
- **نام فایل‌ها:** خروجی‌ها را با پیشوند `LOC_` و `PRP_` ذخیره کنید، مثلاً `LOC_Ramparts.png`، `LOC_Great_hall.png`، `PRP_Poison_cup.png`. شات‌لیست‌ها با همین نام‌ها به مرجع‌ها اشاره می‌کنند.
