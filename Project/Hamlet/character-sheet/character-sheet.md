برای هر پنج شخصیت یک پرامپت شیت شخصیت نوشتم: نگهبان اول، مارسلوس، هوراشیو، شبح پادشاه، و هملت که در شات ۱۲ دیده می‌شود و در صحنه‌های بعد نقش اصلی را دارد. هر تصویر شش پنل دارد. ردیف بالا سه کلوزآپ است و ردیف پایین سه فول‌شات، هر ردیف به ترتیب تمام‌رخ، سه‌رخ و نیم‌رخ. ساختار JSON همان ساختار شات‌لیست است.

**چند نکته برای اینکه شخصیت‌ها یکسان بمانند:**

- **پس‌زمینه:** خاکستری و ساده است و نور یکنواخت استودیویی دارد تا مدل فقط چهره و لباس را یاد بگیرد. حال‌وهوای نور صحنه را در پرامپت شات‌ها می‌دهید.
- **شبح:** در شیت عمداً جسم کامل و غیرشفاف است تا جزئیات زره و چهره واضح بماند. نیمه‌شفاف بودن را در پرامپت شات‌ها اضافه کنید.
- **کلمات ممنوع:** در پرامپت‌ها از «character sheet» یا «turnaround» استفاده نکردم، چون مدل با این کلمه‌ها برچسب و نوشته داخل تصویر می‌گذارد.
- **اندازه تصویر:** پیشنهاد من 1536×1024 است. این را در نود تنظیم کنید، نه در متن پرامپت.
- **خط هویت:** زیر هر پرامپت یک خط کوتاه انگلیسی گذاشتم. آن را عیناً در `description` هر شاتی که آن شخصیت دارد کپی کنید تا متن و تصویر مرجع با هم هماهنگ باشند.

---

### ۱. نگهبان اول، برناردو

```json
{
  "scene": "A six-panel reference image of one late sixteenth-century Danish castle sentinel, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "A stocky Danish castle guard about forty years old, weathered ruddy face, heavy brow, deep-set brown eyes, broad nose, short dark brown beard with a few grey hairs, steel morion helmet with a raised comb and curved brim, dark brown wool cloak over a buff leather jerkin with padded sleeves, brown wool breeches, worn knee-high leather boots, a small horn lantern hanging from a leather belt on the left hip, holding a tall partisan spear upright in the right hand",
      "position": "the same man repeated once in each of the six panels",
      "action": "standing still in a neutral relaxed pose, calm tired expression"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#5A3E2B", "#A68A64", "#8C9399", "#C9CCCF"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left. Bottom row: full-body views from helmet to boots with the whole spear visible, in the same three angles and order. Identical face, clothing, helmet and props in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `stocky Danish guard about forty, weathered ruddy face, short dark brown beard with grey hairs, steel morion helmet, dark brown wool cloak over buff leather jerkin, horn lantern on left hip, partisan spear`

---

### ۲. نگهبان دوم، مارسلوس

```json
{
  "scene": "A six-panel reference image of one late sixteenth-century Danish castle guard, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "A lean Danish castle guard about thirty years old, narrow face, high cheekbones, sharp nose, alert light blue eyes, short reddish-blond beard and moustache, steel morion helmet with a raised comb and curved brim, grey-blue wool cloak over a buff leather jerkin with padded sleeves, dark grey wool breeches, knee-high leather boots, holding a tall partisan spear upright in the left hand",
      "position": "the same man repeated once in each of the six panels",
      "action": "standing still in a neutral relaxed pose, slightly wary expression"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#4F6475", "#B07A4F", "#A68A64", "#C9CCCF"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left. Bottom row: full-body views from helmet to boots with the whole spear visible, in the same three angles and order. Identical face, clothing, helmet and props in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `lean Danish guard about thirty, narrow face, sharp nose, light blue eyes, short reddish-blond beard, steel morion helmet, grey-blue wool cloak over buff leather jerkin, partisan spear`

برای اینکه دو نگهبان کنار هم با هم اشتباه نشوند، رنگ ریش، رنگ شنل و فرم صورتشان را عمداً متفاوت گذاشتم.

---

### ۳. هوراشیو

```json
{
  "scene": "A six-panel reference image of one young Renaissance university scholar, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "Horatio, a slim young scholar about twenty-five years old, medium height, oval face, clean-shaven, short wavy dark brown hair, dark brown eyes, straight nose, thoughtful sceptical expression, plain black wool doublet buttoned to the neck with a small white linen falling collar, black wool breeches and black hose, low black leather shoes, long black wool cloak fastened at the right shoulder, narrow leather belt with a small leather pouch",
      "position": "the same young man repeated once in each of the six panels",
      "action": "standing still in a neutral relaxed pose, hands loose at his sides"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#111111", "#3A3A3A", "#E8E2D6", "#C9CCCF"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left. Bottom row: full-body views from head to shoes, in the same three angles and order. Identical face, hair and clothing in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `Horatio, slim young scholar about twenty-five, clean-shaven oval face, short wavy dark brown hair, dark brown eyes, plain black wool doublet with small white linen collar, long black wool cloak`

---

### ۴. شبح پادشاه، هملت پدر

```json
{
  "scene": "A six-panel reference image of one aged Danish warrior king in full plate armour, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "A tall, broad-shouldered king about sixty years old, gaunt pale face, sunken sorrowful dark eyes, strong straight nose, short dark beard and moustache heavily streaked with silver, wearing complete late sixteenth-century plate armour from head to foot in dark polished steel with thin gilded borders, close helmet with the visor raised to show the whole face, steel gorget, rounded pauldrons, articulated gauntlets, a deep crimson sash across the breastplate from right shoulder to left hip, holding a short dark marshal's baton in the right hand; rendered as a solid, fully opaque figure",
      "position": "the same king repeated once in each of the six panels",
      "action": "standing still in a dignified neutral pose, solemn grieving expression"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#2B2F33", "#6E757C", "#B8963E", "#7A1F24"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, clean highlights on the steel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups of the face inside the raised visor, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left. Bottom row: full-body views from helmet to steel sabatons with the baton visible, in the same three angles and order. Identical face, armour, sash and baton in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `ghostly king about sixty, gaunt pale face, sorrowful dark eyes, short dark beard streaked with silver, full dark steel plate armour with thin gilded borders, visor raised, crimson sash, short marshal's baton in right hand`

در پرامپت شات‌ها این را به خط هویت اضافه کنید: `faintly translucent, glowing pale`.

---

### ۵. هملت

```json
{
  "scene": "A six-panel reference image of one young Danish prince in mourning clothes, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "Hamlet, Prince of Denmark, a slim man about thirty years old, pale complexion, angular face with high cheekbones, intense grey eyes with faint shadows beneath them, dark brown hair falling just below the ears and slightly unkempt, short neatly trimmed dark beard and moustache, wearing deep mourning black: a fitted black velvet doublet with subtle black embroidery and a small white linen collar, black breeches and black hose, black leather shoes, a long black wool cloak, and a thin silver chain with a small round pendant on his chest",
      "position": "the same young man repeated once in each of the six panels",
      "action": "standing still in a neutral relaxed pose, brooding melancholy expression"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#0A0A0A", "#2A2A2E", "#C0C4C8", "#E8E2D6"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left. Bottom row: full-body views from head to shoes, in the same three angles and order. Identical face, hair, clothing and silver chain in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `Hamlet, slim prince about thirty, pale angular face, intense grey eyes, slightly unkempt dark brown hair below the ears, short trimmed dark beard, black velvet mourning doublet with small white collar, long black cloak, thin silver chain with round pendant`

---
سه پرامپت شیت آماده است. هر تصویر شش پنل دارد: ردیف بالا سه کلوزآپ، ردیف پایین سه فول‌شات، هر ردیف به ترتیب تمام‌رخ، سه‌رخ و نیم‌رخ. مشخصات هر شخصیت دقیقاً همان خط هویتی است که در شات‌لیست‌ها آمده، تا متن پرامپت‌ها و تصویر مرجع با هم بخوانند. اندازه پیشنهادی تصویر 1536×1024 است و آن را در نود تنظیم کنید.

---

### ۱. اوفلیا

```json
{
  "scene": "A six-panel reference image of one young Danish noblewoman of the late sixteenth century, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "Ophelia, young noblewoman about eighteen, slender and of medium height, delicate oval face, pale skin with a faint natural blush, large hazel eyes, small straight nose, soft full lips, long straight light golden-brown hair parted in the centre and gathered in a loose braid down her back, wearing a pale blue silk gown with a fitted bodice, long sleeves and a small white lace collar, a thin silver girdle at the waist, holding a small closed prayer book with a dark leather cover and brass clasp in both hands",
      "position": "the same young woman repeated once in each of the six panels",
      "action": "standing in a neutral relaxed pose, gentle shy expression"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#9DB4CC", "#E9EEF2", "#B8875A", "#C9CCCF"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left with the braid visible down her back. Bottom row: full-body views from head to the hem of the gown, in the same three angles and order. Identical face, hair, gown and prayer book in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `Ophelia, young noblewoman about eighteen, delicate oval face, pale skin, large hazel eyes, long straight light golden-brown hair in a loose braid down her back, pale blue silk gown with a fitted bodice and small white lace collar, holding a small closed prayer book with a dark leather cover and brass clasp`

---

### ۲. گرترود

```json
{
  "scene": "A six-panel reference image of one Danish queen of the late sixteenth century, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "Gertrude, Queen of Denmark, handsome woman about forty-five, upright and graceful, fair skin, composed face with fine lines at the eyes, high forehead, grey-green eyes, auburn hair parted in the centre and drawn back under a dark velvet French hood edged with a row of pearls, wearing a deep blue velvet gown with gold embroidered bands, a square neckline and full sleeves with slashed cuffs, a pearl necklace with a small gold pendant, a gold ring on her right hand",
      "position": "the same woman repeated once in each of the six panels",
      "action": "standing in a neutral dignified pose, hands folded at her waist, calm reserved expression"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#1E2F5C", "#B8963E", "#8A3B1F", "#C9CCCF"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left showing the shape of the French hood. Bottom row: full-body views from head to the hem of the gown, in the same three angles and order. Identical face, hood, gown and jewellery in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `Gertrude, Queen of Denmark, handsome woman about forty-five, fair skin, composed face with fine lines, grey-green eyes, auburn hair under a pearl-edged French hood, deep blue velvet gown with gold embroidery and a square neckline, pearl necklace`

---

### ۳. بازیگر نقش ملکه

```json
{
  "scene": "A six-panel reference image of one Renaissance boy actor dressed and made up to play a queen on stage, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "Player Queen, a slim beardless youth about sixteen playing a woman, narrow boyish face with a slightly square jaw beneath the makeup, thick white powder on the face, round rouged cheeks, darkened eyebrows, reddened lips, light brown eyes, a long pale blonde stage wig with a slightly artificial sheen topped by a small painted wooden crown, wearing a stiff old-fashioned gold-and-rose brocade gown that is a little too broad at the shoulders, with worn patches and a frayed hem, and a lace ruff yellowed with age",
      "position": "the same youth repeated once in each of the six panels",
      "action": "standing in a neutral relaxed pose, hands clasped in front in a theatrical ladylike manner"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#C9A35A", "#B86B6B", "#F2E9DC", "#C9CCCF"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left showing the edge of the wig and the boyish jawline. Bottom row: full-body views from crown to the hem of the gown, in the same three angles and order. Identical face, makeup, wig, crown and gown in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `Player Queen, a slim beardless youth about sixteen playing a woman, powdered face, rouged cheeks, long pale wig, stiff old-fashioned brocade gown`

در این شیت عمداً جزئیاتی گذاشتم که نشان می‌دهد پسری نقش زن را بازی می‌کند: فک کمی مربعی، کلاه‌گیسی که مصنوعی به نظر می‌رسد و لباسی که سرشانه‌اش گشاد است. این‌طوری بیننده او را با گرترود یا اوفلیا اشتباه نمی‌گیرد. تاج چوبی هم همان تاج نمایش در شات‌های ۴۰۷، ۶۰۳ و ۶۱۴ است.

---

این شیت برای اوفلیا بعد از دیوانگی است، یعنی صحنه ۹. چهره‌اش دقیقاً همان چهرهٔ شیت اول است و فقط مو، لباس و حالتش عوض شده.

برای اینکه چهره یکی بماند، موقع ساخت این شیت، کلوزآپ تمام‌رخ و سه‌رخ شیت اول (`CHR_Ophelia`) را به‌عنوان تصویر مرجع به مدل بدهید.

```json
{
  "scene": "A six-panel reference image of one young Danish noblewoman of the late sixteenth century after grief has broken her mind, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "Ophelia, young noblewoman about eighteen, slender and of medium height, the same delicate oval face, pale skin, large hazel eyes, small straight nose and soft full lips as before, now thinner and paler with faint shadows under red-rimmed eyes; long light golden-brown hair worn loose and tangled to the waist, with small wildflowers and stems caught in it; wearing a modest loose white linen gown with long sleeves and a high gathered neckline, crumpled, slipping slightly off one shoulder of a linen under-shift, the hem grey with dust and torn in one place; barefoot; holding a loose bunch of wild herbs and flowers against her chest: rosemary sprigs, purple and yellow pansies, small white daisies and a few faded violets",
      "position": "the same young woman repeated once in each of the six panels",
      "action": "standing in a neutral pose with her head tilted slightly, a distant dreamy half-smile, eyes unfocused"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#EDE8DE", "#B8875A", "#7A5C8C", "#C9CCCF"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left showing the loose hair with flowers caught in it. Bottom row: full-body views from head to bare feet, in the same three angles and order. Identical face, hair, gown and bunch of flowers in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `Ophelia after her madness, young noblewoman about eighteen, delicate oval face, pale skin, large hazel eyes with red rims, long loose tangled light golden-brown hair with wildflowers caught in it, modest loose white linen gown with long sleeves, crumpled and dusty at the hem, barefoot, holding a bunch of rosemary, pansies, daisies and faded violets`

---

چند نکته:

- **هماهنگی با نریشن:** گل‌های دسته را از نریشن صحنه ۹ گرفتم: رزماری، بنفشه سه‌رنگ و بنفشه پژمرده. موقع گل دادن به دیگران در شات‌ها همین گل‌ها دیده می‌شوند.
- **لباس:** لباس عمداً پوشیده و ساده است. پیراهن کتانی سفید آستین‌بلند و یقه‌بسته است و فقط چروک و خاک‌آلود بودنش آشفتگی او را نشان می‌دهد.
- **نام فایل:** فایل خروجی را `CHR_Ophelia_mad` بنامید. در شات‌لیست صحنه‌های ۹ تا ۱۱ از این نام استفاده می‌کنم. برای صحنه ۱۰، یعنی روایت غرق شدن، همین شیت را با اضافه کردن تاج گل وحشی روی سر به کار ببرید.

---

این شیت لائرتس است، با همان قالب شش‌پنلی شیت‌های قبلی. مشخصاتش دقیقاً همان خط هویتی است که در شات‌لیست صحنه‌های ۹ و ۱۰ آمده است.

```json
{
  "scene": "A six-panel reference image of one young Danish nobleman of the late sixteenth century just returned from France, arranged in two rows of three panels on a plain seamless background",
  "subjects": [
    {
      "description": "Laertes, son of Polonius, athletic young man about twenty-two, tall with broad shoulders and a fencer's upright stance, handsome square face, fair complexion, strong straight brows, light grey-green eyes, short light golden-brown hair brushed back, short clipped golden-brown beard along the jaw and a light moustache, wearing a fashionable French-cut slate-grey travelling doublet with a row of small silver buttons and a narrow white linen collar, dark grey breeches, a dark charcoal wool cloak over one shoulder, brown leather riding gloves, high brown leather riding boots, a rapier with a swept steel hilt in a dark leather scabbard on his left hip",
      "position": "the same young man repeated once in each of the six panels",
      "action": "standing in a neutral confident pose, left hand resting on the rapier hilt, serious proud expression"
    }
  ],
  "style": "Cinematic photograph, historical drama, Renaissance-era Denmark, natural film grain, rich shadow detail, restrained realistic color, image fills the entire frame edge to edge",
  "color_palette": ["#5B646B", "#2E3236", "#8A6A45", "#C9CCCF"],
  "lighting": "Soft, even, diffused studio light from the front left with gentle fill, consistent in every panel, no harsh shadows",
  "mood": "Neutral, clear, documentary reference",
  "background": "Plain seamless light grey backdrop in every panel",
  "composition": "Two rows of three equal panels separated by thin plain grey gaps. Top row: head-and-shoulders close-ups, first facing the camera directly, second turned three-quarters to the left, third in full side profile facing left. Bottom row: full-body views from head to boots with the whole rapier visible, in the same three angles and order. Identical face, hair, beard, doublet, gloves and rapier in all six panels",
  "camera": {
    "angle": "eye level in every panel",
    "distance": "close-up in the top row, full shot in the bottom row",
    "lens": "85mm for the close-ups, 50mm for the full shots",
    "depth_of_field": "deep focus, everything sharp"
  }
}
```

**خط هویت:** `Laertes, son of Polonius, athletic young man about twenty-two, handsome square face, fair complexion, short light golden-brown hair, light grey-green eyes, short clipped golden-brown beard along the jaw, fashionable French-cut slate-grey travelling doublet with silver buttons, dark cloak, high leather riding boots, rapier at his hip`

---

- **شباهت با اوفلیا:** رنگ مو و ریش لائرتس عمداً همان قهوه‌ای‌طلایی موی اوفلیاست تا معلوم باشد خواهر و برادرند. چهره‌اش اما مربعی و مردانه است تا با چهره بیضی اوفلیا یکی نشود.
- **دستکش:** دستکش‌های چرمی را در شیت گذاشتم چون در شات ۹۱۴ دیده می‌شوند.
- **نام فایل:** فایل خروجی را `CHR_Laertes` بنامید.
- **صحنه ۱۲:** در مسابقهٔ شمشیربازی، لائرتس احتمالاً بدون شنل و چکمه‌های سواری است. در شات‌لیست آن صحنه همین شیت را به کار می‌برم و تغییر لباس را در توضیح شات می‌نویسم.