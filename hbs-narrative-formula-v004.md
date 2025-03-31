# Human Builder System (HBS) Narrative Formula v004

## Base Formula Structure

```
[1. Gender] [2. Visual Heritage] [3. Age (position)] with [4. Build (intensity)] and [5. Height]. [6. Skin Tone (intensity)] skin with [7. Skin Texture (visibility)] quality. [8. Head Shape (alignment/definition/prominence)] head with [9. Face Shape] face, [10. Forehead (height/width)] forehead, [11. Jawline (definition/prominence/angle)] jawline, and [12. Cheekbones (height/prominence/definition)] cheekbones. [13. Eyes (size/shape intensity/opening/angle)] [14. Eye Color (intensity)] eyes with [15. Eyebrows (aesthetic)] eyebrows. [16. Nose (simple adjective)] nose, [17. Mouth (expression)] mouth with [18. Lips] lips. [19. Facial Hair (density/grooming/style) if applicable]. [20. Hair Texture (quality)] [21. Hair Density] [22. Hair Volume] [23. Hair Length] [24. Hair Color (tone/shade)] hair, styled with [25. Hair Parting] and [26. Bangs/Fringe] [27. Tails and Buns (tightness/neatness/positioning/style) if applicable].
```

**Checksum: 378** (Sum of parameters 1-27)

## Parameter Groups

1. **Core Identity**: Parameters 1-3
   - Gender
   - Visual Heritage
   - Age (with position modifiers: early, mid, late)

2. **Body Structure**: Parameters 4-7
   - Build (with intensity modifiers: slightly, moderately, notably, extremely)
   - Height
   - Skin Tone (with intensity modifiers: light, rich, deep)
   - Skin Texture (with visibility modifiers: subtle, noticeable, prominent)

3. **Facial Structure**: Parameters 8-12
   - Head Shape (with alignment modifiers: slightly, classically, perfectly; definition modifiers: softly, moderately, sharply; prominence modifiers: subtle, pronounced)
   - Face Shape
   - Forehead (with height modifiers: low, medium, high; width modifiers: narrow, average, wide)
   - Jawline (with definition modifiers: softly defined, moderately defined, sharply defined; prominence modifiers: subtle, pronounced; angle modifiers: gently angled, strongly angled)
   - Cheekbones (with height modifiers: low, medium, high; prominence modifiers: subtle, moderate, pronounced; definition modifiers: softly defined, sharply defined)

4. **Facial Features**: Parameters 13-19
   - Eyes (with size modifiers: small, medium, large; shape intensity modifiers: slightly, distinctly, extremely; opening modifiers: narrowly open, moderately open, widely open; angle modifiers: slightly/moderately/distinctly downturned, neutral, slightly/moderately/distinctly upturned)
   - Eye Color (with intensity modifiers: pale, medium, deep)
   - Eyebrows (with aesthetic adjectives: elegant, sculpted, natural, bold, delicate, structured, expressive, refined, dramatic, subtle)
   - Nose (with simple adjectives: classic, strong, refined, delicate, prominent, subtle, elegant, distinctive)
   - Mouth (with expression modifiers: pleasant, expressive, serious, neutral, thoughtful, relaxed)
   - Lips
   - Facial Hair (with density/fullness modifiers: sparse, medium, dense, full; grooming modifiers: neatly trimmed, well-groomed, slightly unkempt, rugged; style modifiers: classic, modern, traditional)

5. **Hair Attributes**: Parameters 20-27
   - Hair Texture (with quality modifiers: silky, coarse, fine, smooth, glossy, shiny, dry, soft)
   - Hair Density
   - Hair Volume
   - Hair Length
   - Hair Color (with tone/shade modifiers: light, medium, deep)
   - Hair Parting
   - Bangs/Fringe
   - Tails and Buns (with tightness modifiers: tight, medium, loose; neatness modifiers: sleek, tidy, casual, messy; positioning modifiers: centered, off-center, asymmetric; style detail modifiers: braided, twisted, coiled, textured)

## Example Implementation

```
Female Southeast Asian early young adult with moderately athletic build and average height. Rich golden caramel skin with noticeable dewy fresh texture. Classically oval, softly defined head with heart-shaped face, high, average width gentle rounded forehead, moderately defined, subtle tapered heart jawline, and high, pronounced, sharply defined cheekbones. Medium, distinctly almond-shaped, moderately open, slightly upturned deep brown eyes with elegant arched eyebrows. Refined straight, narrow-bridge nose, pleasant medium mouth with full lips. Silky, glossy straight thick density high volume shoulder-length medium deep brown hair, styled with side part and side-swept bangs with a loose, casual, twisted high ponytail.
```

Note how adjectives and adverbs function as a weighting system, allowing for precise control over specific features:
- "Moderately athletic" vs "extremely athletic" controls the degree of muscle definition
- "Rich golden caramel" vs "light golden caramel" adjusts skin tone intensity
- "Slightly upturned" vs "distinctly upturned" controls the degree of eye angle
- "Silky, glossy" adds specific textural qualities to the hair

## Notes for Development

- Parameter numbers serve as visual verification during development
- The order follows a logical whole-to-part progression
- Connecting language maintains natural narrative flow
- Parameters should be selected to prevent conflicts according to Control File exclusion rules
- Checksum (378) confirms all parameters are present
- Adjectives and adverbs serve as a weighting system to control emphasis
  - Modifiers should be selected to maintain logical consistency
  - Contradictory modifiers should be avoided
  - Not all parameters require modifiers; some are clear without them

## Modifier Application Guidelines

1. Use only one modifier per modifier category (e.g., one intensity modifier, one angle modifier)
2. Avoid contradictory modifier combinations (e.g., "softly sharp")
3. Select modifiers appropriate to the base parameter (e.g., "refined" works for "button nose" but "strong" does not)
4. Use modifiers sparingly for clarity - not every parameter needs modifiers
5. For parameters without listed modifiers, no modifiers should be applied

## Checksum Discussion

**Q: "Include the number. It's like a 'checksum.' Wait, what does the sequence of 1-27 added equal?"**

**A: "The sum of all parameter numbers (1 through 27) equals: 1+2+3+4+5+6+7+8+9+10+11+12+13+14+15+16+17+18+19+20+21+22+23+24+25+26+27 = 378"**

**Q: "Let's do this for development purposes to make sure all parameters are there at first glance. Thoughts?"**

**A: "Including the parameter numbers in the development version is an excellent approach. It offers several advantages:
1. Immediate Verification: You can quickly see if any parameters are missing just by scanning the numbers in sequence.
2. Debugging Aid: If there are issues with specific parameters, the numbers make it easy to reference them in discussions or documentation.
3. Structure Validation: The numbering helps ensure the narrative flow maintains the logical parameter progression.
4. Dependency Tracking: When adjusting conditional conflicts, the numbers make it easier to track which parameters affect others.
5. Consistent Implementation: Development teams have a clear reference for which parameter is which without ambiguity."**
