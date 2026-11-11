# Instructions: Preparing Persian Text for AI Speech Generation

Nov 8, 2026 · @Vahid

## 1. Purpose

These instructions define how to edit written Persian text so that AI text-to-speech (TTS) systems, such as ElevenLabs, pronounce it accurately and naturally. The procedure applies only the smallest technical changes needed for correct pronunciation, natural pauses, and fluent rhythm.

The original meaning, wording, tone, and structure must remain exactly as they are. The expected result is Persian text that matches the original exactly in content and differs only in technical refinements (punctuation, spacing, orthography, and minimal vowel marks), ready to send directly to the speech generator.

## 2. Prerequisites

### 2.1 Required knowledge

- Expert command of Persian orthography, grammar, ezafe usage, and standard pronunciation.
- Understanding of how TTS engines process text, in particular that they read visible markup, brackets, and notes aloud.

### 2.2 Required input

- The Persian source text to be prepared for speech generation.

### 2.3 Technical requirements

- The ability to enter standard Persian characters «ی» and «ک», the zero-width non-joiner (نیم‌فاصله), the vowel marks (َ ِ ُ ّ ً), and the sukun «ْ».

### 2.4 Initial conditions

No other initial conditions are specified.

## 3. Procedure

**Content preservation rule (applies to every step):**

- Do **not** rewrite, summarize, expand, translate, interpret, or reorder the text.
- Do **not** add, remove, or replace words. The only exception is respelling a word so that it is pronounced correctly.
- Keep the original register, style, emotional tone, and level of formality.
- Keep proper nouns, technical terms, numbers, abbreviations, and quotations. Change them only if they would otherwise be mispronounced.

### Phase A: Orthography and spacing

1. **Read the full text.** Note its meaning, tone, and formality, and identify words that are likely to be mispronounced.
2. **Standardize characters.** Replace the Arabic «ي» and «ك» with the Persian «ی» and «ک».
3. **Apply the zero-width non-joiner.** Use it correctly in compounds and affixes, for example «می‌شود», «کتاب‌ها», and «پیش‌بینی». Correct use prevents words from being split or merged by mistake.
4. **Clean up spacing.** Remove extra spaces and make every word boundary clear.

### Phase B: Punctuation and segmentation

5. **Correct the punctuation for spoken delivery.** Use the Persian marks «،» «؛» «؟» «.» «...» «« »» to mark natural pauses and sentence boundaries.
6. **Break very long sentences.** Use commas or periods only. Never change words to shorten a sentence.
7. **Segment the paragraphs.** Split paragraphs into units of meaning that also match where a speaker would breathe.
8. **Restrict ellipses.** Keep «...» for intentional narrative pauses only.

### Phase C: Vowel marks

9. **Add vowel marks only where they prevent ambiguity or mispronunciation.** Apply them in the following cases:

| Case | Action | Example |
| --- | --- | --- |
| Homographs | Mark the intended reading. | «کَرد / کُرد», «مُلک / مَلِک / مِلک», «گُل / گِل» |
| Ezafe | Add a kasra where a missing or wrong ezafe would change the meaning or rhythm. | «تاریخِ صنعت» |
| Rare, foreign, or technical words | Mark words that TTS systems often misread. | None specified |
| Proper nouns | Mark names whose pronunciation is uncertain. | None specified |

**Warning:** Do not add vowel marks to the whole text. Excessive vowel marks can make TTS output worse.

### Phase D: Difficult words and syllabification

10. **Fix pronunciation inside the text.** Use vowel marks or a phonetic Persian spelling. **Never** use brackets, IPA, Latin transliteration, or parenthetical notes, because the TTS engine reads them aloud.
11. **Write out items that could be misread.** Write abbreviations, foreign names, and numbers in Persian letters only when needed. For example, write «سال هزار و نهصد و شصت و یک» only if the digits would be read incorrectly.
12. **Clarify syllable boundaries.** Use vowel marks, the sukun «ْ», or the zero-width non-joiner. Do **not** insert hyphens, dots, or other visible syllable markers.

### Phase E: Phonology and prosody

13. **Refine the flow.** Aim for natural connected speech, correct stress, and smooth transitions between sounds. Use punctuation to make emphasis and rhythm clear.
14. **Resolve alternative pronunciations.** **Decision point:** when more than one pronunciation is possible, choose the standard Persian pronunciation that fits the context.

### Phase F: Output

15. **Return only the edited Persian text,** ready to send to the speech generator, with:
    - natural Persian paragraphs and punctuation;
    - clear spacing and correct use of the zero-width non-joiner;
    - vowel marks only where needed;
    - no headings, labels, preamble, or closing remarks.

Provide explanations, comments, change lists, or notes only if the user requests them.

## 4. Verification

Before returning the text, confirm each of the following:

- [ ] Every word and piece of information from the original is still present, with no additions or omissions.
- [ ] The meaning, tone, and formality are unchanged.
- [ ] Punctuation creates natural pauses and sentence boundaries.
- [ ] Homographs, ezafe, and difficult words are clarified with minimal vowel marks.
- [ ] The zero-width non-joiner and Persian characters are used correctly.
- [ ] Nothing in the text would be read aloud as markup or commentary.
- [ ] A Persian TTS system can read the text fluently and naturally.

**Success criterion:** the output matches the original exactly in content and differs only in technical refinements that make it sound accurate, clear, and natural as Persian speech.

The result is **unsuccessful** if any word is added, removed, or replaced (other than a permitted respelling for pronunciation), if the meaning or tone has changed, if vowel marks are applied excessively, or if any visible markup, note, or commentary remains in the text.

## 5. Troubleshooting and Important Notes

### 5.1 Prohibited actions

- Changing the meaning, adding content, or leaving anything out.
- Translating any part of the text.
- Including explanations, comments, change lists, or notes, unless the user asks for them.
- Inserting performance directions inside the text, such as «با هیجان».
- Using visible markup that the TTS engine would read aloud.

### 5.2 Common conditions and corrective actions

| Condition | Corrective action |
| --- | --- |
| A word would be mispronounced as written | Add vowel marks or use a phonetic Persian spelling within the text. Do not add brackets or notes. |
| Digits or abbreviations would be misread | Write them out in Persian letters. Otherwise, leave them unchanged. |
| A sentence is too long for natural delivery | Divide it with a comma or period without changing any words. |
| Several pronunciations are valid | Use the standard Persian pronunciation that fits the context. |
| The text contains too many vowel marks | Remove any mark that does not prevent ambiguity or mispronunciation. |
| Arabic «ي» or «ك» appears | Replace it with Persian «ی» or «ک». |

No further troubleshooting procedures are specified.

## 6. Accuracy Review

- **Undefined thresholds:** "Smallest technical changes," "very long sentences," and "uncertain pronunciation" are not defined and depend on editorial judgment.
- **Engine-specific behavior:** The guidance is general, and ElevenLabs is cited only as an example. How a specific TTS engine handles vowel marks, the zero-width non-joiner, and digits is unverified and may vary between engines and versions. Whether digits need to be written out can only be confirmed by testing the target engine.
- **Respelling exception:** The boundary between a permitted respelling and a prohibited word replacement is not defined. Writing numbers out in Persian letters is treated as a permitted respelling.
- **Unknown pronunciations:** No procedure is specified when the editor does not know the correct pronunciation of a proper noun or foreign word.
- **Verification method:** The source specifies no method for confirming that a TTS system reads the text fluently, such as generating and reviewing test audio. Step 1 (reading the full text first) is an interpretation added for completeness.
- **Requested explanations:** The format for explanations or change lists, when the user requests them, is not specified.
