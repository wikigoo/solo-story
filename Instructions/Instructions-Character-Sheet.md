# Instructions: Writing Character Reference Sheet Prompts

Version for all Solo channel play projects · FLUX.2 Prompt Builder Node

## 1. Purpose

These instructions define how to write text-to-image prompts for **character reference sheets** for any play adapted on the Solo channel. A character sheet is a single image that fixes the face, body, and costume of one or more characters. It is later given to the image model as a reference, so that each character looks the same in every shot of the film.

Every prompt uses the exact field structure of the node `Template/flux2-prompt-node-v2.html`, so that each field can be pasted into the matching node field.

## 2. Inputs

Before writing, collect the following from the project folder (`Project/<Play-Name>/`):

| Input | Use |
|---|---|
| `Key-Scenes.md` | The list of characters and the scenes they appear in. |
| `Narration/Narration-1.md` | Ages, costumes, and conditions as the story describes them, and every change of appearance. |
| The play's source file (for example `<Play-Name>.md`) | Facts about the characters, their relationships, and the setting. |
| Fixed film decisions | The historical period, costume rules, and the fixed `style` string. If they do not exist yet, write them first (see Section 10). |

## 3. Reference Examples

Two example images show the target result. Keep them in the repository, for example:

- `Example/character-sheet/Sample-Type-A.png`: one character in three states (Hamlet in mourning, fencing, and dishevelled clothes).
- `Example/character-sheet/Sample-Type-B.png`: three different characters (Horatio, the queen, and Claudius).

The examples show the **layout** to match. Their content belongs to the Hamlet project and must not be copied into other projects.

## 4. Output Layout (applies to every sheet)

Each image is a grid of **columns × 2 rows** on a plain light grey background, with a **caption strip** under each column.

| Element | Rule |
|---|---|
| Columns | 3 per image. Use 2 only when fewer subjects remain. One column = one character state or one character. |
| Top row | Head-and-shoulders close-up, facing the camera directly. |
| Bottom row | Full-body view from head to feet, facing the camera directly, standing upright, arms relaxed. |
| Angles | Front view only. No three-quarter or profile views. |
| Alignment | Eye lines aligned across the top row; feet on one baseline across the bottom row. |
| Gaps | Thin plain grey gaps between all panels. |
| Background | Plain seamless light grey in every panel. |
| Caption strip | A light grey strip under each column with the name in English, centred, in a clean bold dark navy sans-serif font. |
| Other text | None. The captions are the only text in the image. |

## 5. Procedure

### Step 1: List every character and every state

Read the key scenes and the narration. For each character who is **seen** (not only mentioned), write down:

- the scenes in which they appear;
- every distinct **state**: a different age, costume, or condition (for example mourning clothes, travel clothes, after madness, after an injury, in old age, in a disguise, as a ghost).

A new state exists only when the change is visible and lasts at least one whole scene. Small changes inside one scene, such as a removed hat or a raised visor, are described later in the shot prompts, not in a new state.

### Step 2: Decide who needs no sheet

Skip characters who are seen only from behind, in silhouette, as part of a crowd, as a partial body (hands, feet), or in a single distant shot. List them in the notes section of the document.

### Step 3: Sort characters into sheet types

**Type A: Multi-state sheet (one character, several states)**

Use Type A for every character with **two or more states**.

- Put all states of one character in one prompt and one image, one state per column.
- Order the columns by story order.
- If a character has more than three states, split them over several Type A images of up to three columns. Repeat the main state as the first column of each image so the face is anchored in every image.
- If a character has exactly two states, make a 2-column Type A image.

**Type B: Group sheet (three different characters, one state each)**

Use Type B for every character with **one state only**.

- Put three different characters in one prompt and one image, one character per column.
- Group characters who appear in the same scenes or belong together, such as a couple, two guards, two courtiers, or a family. This makes contrast and scale easy to check.
- If one or two characters remain at the end, make a 2-column Type B image rather than inventing a filler.

### Step 4: Fix the distinguishing features

Before writing descriptions, make sure any two characters who could be confused, such as servants, soldiers, siblings, or twins played by different actors, differ clearly in at least three of the following: face shape, hair colour and length, beard, height and build, costume colour.

Family members may share one feature on purpose (for example hair colour) to show their relationship.

### Step 5: Write the prompts

Follow the field rules in Section 6, the caption rules in Section 7, and the description rules in Section 8.

### Step 6: Write the identity lines

Under each prompt, write one **identity line** in English for each column (see Section 9).

### Step 7: Verify

Go through the checklist in Section 13 before delivering.

## 6. Field-by-Field Rules (node schema)

Use only these keys, in this order: `prompt`, `style`, `camera`, `lighting`, `colors`, `composition`.

### `prompt`

Write it in this order:

1. **Layout sentence:** "A character reference image arranged in a grid of {N} columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column."
2. **Row sentence:** "In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly."
3. **One block per column**, starting with "Left column:", "Middle column:", "Right column:". Each block contains:
   - the caption text in double quotes, for example `captioned "{Name}"`;
   - the description, in the order given in Section 8;
   - for Type A, after the first column: "the same {man / woman} as in the other columns, with an identical face".
4. **Closing sentence:** "The captions are the only text in the image."

### `style`

Use the project's fixed style string, copied exactly. It is the same in every prompt of the project. Pattern:

```
Cinematic photograph, historical drama, {period and place}, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge
```

### `camera`

```json
{
  "angle": "eye level, straight-on front view in every panel",
  "distance": "close-up in the top row, full shot in the bottom row",
  "lens": "85mm for the close-ups, 50mm for the full shots",
  "f-number": "f/8",
  "ISO": 100,
  "focus": "deep focus, everything sharp in every panel"
}
```

### `lighting`

"Soft, even, diffused studio light from the front left with gentle fill, identical in every panel, soft gentle shadows."

### `colors`

- `palette`: three or four hex colours taken from the costumes, plus the background grey `#C9CCCF`.
- `mood`: "neutral, clear, documentary reference".

### `composition`

Restate the grid: the number of columns, the two rows, the close-ups above and full bodies below, the aligned eye lines and the common baseline, and the caption strip with every caption text in double quotes.

## 7. Caption Rules

- Write the exact caption text in double quotes, both in `prompt` and in `composition`.
- Use English only, at most four words, and no punctuation except spaces.
- Use the character's **personal name**, not a title or role. Write "Gertrude", not "Queen of Denmark". Title words such as *king*, *queen*, *prince*, *pope*, *emperor*, *bishop*, or *royal* pull the model toward crowns, veils, mitres, and robes that the description did not ask for.
- For a character without a name, use a short role that implies no costume, for example "First Gravedigger", "Old Man", or "Second Student".
- For Type A states, use the pattern "{Name} in {State}", for example "{Name} in Travel Clothes" or "{Name} in Old Age".
- After generating, check the spelling of every caption. If one is wrong, regenerate, or correct the text in an image editor.

## 8. Description Rules

**Order of description in each column:**

1. name or role;
2. age;
3. height and build;
4. face shape and skin;
5. eyes and nose;
6. hair: colour, length, style;
7. beard or moustache;
8. headwear, always stated;
9. costume from top to bottom, with materials and colours;
10. jewellery and accessories;
11. props held;
12. expression.

**Further rules:**

- **Be positive.** FLUX.2 ignores negative instructions. Write "bare head with short dark hair" instead of "no crown", and "a dark velvet hood edged with pearls" instead of "no veil".
- **Always state the headwear.** If none is described, the model may invent one, especially for rulers and clergy.
- **Keep the period consistent.** Every costume, weapon, and accessory must belong to the project's fixed historical period.
- **Age changes (Type A).** Say what ages (lines, grey or thinning hair, posture, weight) and what stays fixed (bone structure, eye colour, nose shape).
- **Costume changes (Type A).** Repeat the fixed facial features in every column, and change only the costume and grooming.
- **Supernatural and unusual figures.** Ghosts, spirits, angels, devils, and allegorical figures are rendered as solid and fully opaque. Glow, translucency, and smoke are added later in the shot prompts.
- **Animals or transformed characters.** Treat a transformation as a separate state of the same character in a Type A sheet. Describe one feature that links it to the human form, such as eye colour or a scarf.
- **Children.** Describe children with modest, age-appropriate clothing and neutral expressions only.
- **Props.** Keep props simple. Books stay closed, folded papers show only their blank side, and hands hold props in a relaxed way.
- **Avoid text-trigger words** everywhere except the captions: *subtitle, caption bar, label, sign, signage, poster, banner, title, logo, watermark, letter, screen, still, film still, screenshot*.

## 9. Identity Lines

For every column, write one identity line in English: a single sentence of about 30 to 50 words that repeats the fixed features (age, face, hair, eyes, beard, headwear, costume, key prop). It is copied word for word into the `prompt` of every shot in which that character, in that state, appears.

Pattern:

```
{Name}, {age and build}, {face}, {eyes}, {hair}, {beard}, {headwear}, {main costume}, {key prop}
```

## 10. Fixed Film Decisions (write once per project)

If the project does not yet have them, write these before any sheet. They open the character sheet document.

- **Historical period:** one period and place for the whole film, matching the play's setting or a deliberate staging choice.
- **Costume, weapons, architecture, and light sources** typical of that period.
- **Fixed `style` string** (see Section 6).
- **Look table:** for each location, the scenes, the base lighting, and a palette of four hex colours.
- **Recommended image sizes** (see Section 11).

## 11. Image Size

Set the size in the node, never in the prompt text. Use dimensions divisible by 16.

| Columns | Recommended size |
|---|---|
| 3 | 1536 × 1024 |
| 2 | 1024 × 1024 |

## 12. Using the Sheets as References

- Save each image with a clear English name:
  - Type A: `CHR_{Name}_states.png`, or `CHR_{Name}_states_2.png` for a second image.
  - Type B: `CHR_Group_{Name1}_{Name2}_{Name3}.png`.
- Before passing a sheet to the model as a reference, **crop out the caption strip**. Text in a reference image can leak into the shots.
- Where possible, pass only the column of the state the shot needs.
- For a Type A sheet, pass the close-up of the main state as an extra reference when generating the other states, so the face does not drift.

## 13. Document Format

Save the document as `Project/{Play-Name}/character-sheet/character-sheet.md`, with these parts:

1. **Fixed film decisions** (Section 10).
2. **Type A sheets:** one section per character with several states.
3. **Type B sheets:** one section per group.
4. **Notes:** characters without a sheet (with the reason), and any changes from earlier versions.

Each sheet section contains:

- a heading with the caption names and scene numbers, for example `### Type A: {Name}, scenes 1–12`;
- the JSON prompt in its own code block;
- the identity line for every column;
- a short note, only when needed.

## 14. Templates

Replace every `{…}` placeholder. Delete the third column for 2-column images.

### Type A: one character, several states

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"{Name} in {State 1}\": {Name}, {age}, {height and build}, {face and skin}, {eyes and nose}, {hair}, {beard}, {headwear}, {costume top to bottom}, {jewellery}, {props}, {expression}. Middle column, captioned \"{Name} in {State 2}\": the same {man/woman} as in the other columns, with an identical face, {changed grooming or age}, {headwear}, {costume top to bottom}, {props}, {expression}. Right column, captioned \"{Name} in {State 3}\": the same {man/woman} as in the other columns, with an identical face, {changed grooming or age}, {headwear}, {costume top to bottom}, {props}, {expression}. The captions are the only text in the image.",
  "style": "{fixed project style string}",
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
    "palette": ["{hex 1}", "{hex 2}", "{hex 3}", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"{Name} in {State 1}\", \"{Name} in {State 2}\", \"{Name} in {State 3}\""
}
```

### Type B: three different characters

```json
{
  "prompt": "A character reference image arranged in a grid of three columns and two rows, separated by thin plain grey gaps, on a plain seamless light grey backdrop, with a caption strip under each column. In every column the top panel is a head-and-shoulders close-up facing the camera directly, and the bottom panel is a full-body view from head to feet facing the camera directly. Left column, captioned \"{Name 1}\": {full description in the order of Section 8}. Middle column, captioned \"{Name 2}\": {full description in the order of Section 8}. Right column, captioned \"{Name 3}\": {full description in the order of Section 8}. The captions are the only text in the image.",
  "style": "{fixed project style string}",
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
    "palette": ["{hex 1}", "{hex 2}", "{hex 3}", "#C9CCCF"],
    "mood": "neutral, clear, documentary reference"
  },
  "composition": "Three equal columns, two rows. Top row: three front-facing head-and-shoulders close-ups with eye lines aligned. Bottom row: three front-facing full-body views with feet on the same baseline. Under each column a light grey caption strip with centred bold dark navy sans-serif text: \"{Name 1}\", \"{Name 2}\", \"{Name 3}\""
}
```

## 15. Verification Checklist

**Before delivering the prompts:**

- [ ] Every seen character and every visible state in the narration is covered by exactly one column, or listed in the notes as needing no sheet.
- [ ] Characters with several states are in Type A sheets; single-state characters are grouped in Type B sheets.
- [ ] Every panel is a front view: close-up on top, full body below.
- [ ] Every column has a caption in double quotes, in English, using a personal name or a costume-neutral role.
- [ ] Headwear is described positively in every column.
- [ ] Look-alike characters differ in at least three visible features.
- [ ] Every costume and prop fits the project's period.
- [ ] The JSON uses only the node keys and parses without errors.
- [ ] The `style` string is identical in every prompt of the project.
- [ ] No text-trigger words appear outside the captions.
- [ ] Every column has an identity line.

**After generating the images:**

- [ ] Captions are spelled correctly.
- [ ] Within each Type A sheet, the face is the same in every column.
- [ ] Headwear and costume match the description; there are no invented crowns, veils, or hats.
- [ ] All poses face the camera directly.
- [ ] The caption strip has been cropped off the copy used as a reference.