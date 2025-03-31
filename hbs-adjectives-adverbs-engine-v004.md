# Human Builder System (HBS) Adjectives & Adverbs Engine

## Overview
This document defines the adjective and adverb modifiers for each parameter in the HBS taxonomy. These modifiers act as a weighting system to adjust the emphasis and characteristics of each parameter without changing its base value.

## Core Identity Parameters

### 1. Gender
**Status:** Locked without modifiers

### 2. Visual Heritage
**Status:** Locked without modifiers

### 3. Age
**Status:** Locked with position modifiers
- **Position modifiers:** early, mid, late

## Body Structure Parameters

### 4. Build
**Status:** Locked with intensity modifiers
- **Intensity modifiers:** slightly, moderately, notably, extremely

### 5. Height
**Status:** Locked without modifiers

### 6. Skin Tone
**Status:** Locked with intensity modifiers
- **Intensity modifiers:** light, rich, deep

### 7. Skin Texture
**Status:** Locked with visibility modifiers
- **Visibility modifiers:** subtle, noticeable, prominent

## Facial Structure Parameters

### 8. Head Shape
**Status:** Locked with multiple modifier types
- **Alignment modifiers:** slightly, classically, perfectly
- **Definition modifiers:** softly, moderately, sharply
- **Prominence modifiers:** subtle, pronounced

### 9. Face Shape
**Status:** Locked without modifiers

### 10. Forehead
**Status:** Locked with dimensional modifiers
- **Height modifiers:** low, medium, high
- **Width modifiers:** narrow, average, wide

### 11. Jawline
**Status:** Locked with multiple modifier types
- **Definition modifiers:** softly defined, moderately defined, sharply defined
- **Prominence modifiers:** subtle, pronounced
- **Angle modifiers:** gently angled, strongly angled

### 12. Cheekbones
**Status:** Locked with multiple modifier types
- **Height modifiers:** low, medium, high
- **Prominence modifiers:** subtle, moderate, pronounced
- **Definition modifiers:** softly defined, sharply defined

## Facial Feature Parameters

### 13. Eyes
**Status:** Locked with multiple modifier types
- **Size modifiers:** small, medium, large
- **Shape intensity modifiers:** slightly, distinctly, extremely
- **Opening modifiers:** narrowly open, moderately open, widely open
- **Angle modifiers:** 
  - downturned: slightly downturned, moderately downturned, distinctly downturned
  - neutral
  - upturned: slightly upturned, moderately upturned, distinctly upturned

### 14. Eye Color
**Status:** Locked with intensity modifiers
- **Intensity modifiers:** pale, medium, deep

### 15. Eyebrows
**Status:** Locked with aesthetic adjectives
- **Aesthetic adjectives:** elegant, sculpted, natural, bold, delicate, structured, expressive, refined, dramatic, subtle

### 16. Nose
**Status:** Locked with simple adjectives
- **Simple adjectives:** classic, strong, refined, delicate, prominent, subtle, elegant, distinctive

### 17. Mouth
**Status:** Locked with expression modifiers
- **Expression modifiers:** pleasant, expressive, serious, neutral, thoughtful, relaxed

### 18. Lips
**Status:** Locked without modifiers

### 19. Facial Hair
**Status:** Locked with multiple modifier types
- **Density/Fullness modifiers:** sparse, medium, dense, full
- **Grooming modifiers:** neatly trimmed, well-groomed, slightly unkempt, rugged
- **Style modifiers:** classic, modern, traditional

## Hair Parameters

### 20. Hair Texture
**Status:** Locked with quality modifiers
- **Quality modifiers:** silky, coarse, fine, smooth, glossy, shiny, dry, soft

### 21. Hair Density
**Status:** Locked without modifiers

### 22. Hair Volume
**Status:** Locked without modifiers

### 23. Hair Length
**Status:** Locked without modifiers

### 24. Hair Color
**Status:** Locked with tone/shade modifiers
- **Tone/shade modifiers:** light, medium, deep

### 25. Hair Parting
**Status:** Locked without modifiers

### 26. Bangs/Fringe
**Status:** Locked without modifiers

### 27. Tails and Buns
**Status:** Locked with multiple modifier types
- **Tightness modifiers:** tight, medium, loose
- **Neatness modifiers:** sleek, tidy, casual, messy
- **Positioning modifiers:** centered, off-center, asymmetric
- **Style detail modifiers:** braided, twisted, coiled, textured

## Usage Guidelines

1. Each parameter can have zero, one, or multiple modifiers applied
2. Modifiers should be applied consistently within parameter groups
3. When using multiple modifiers for a single parameter, order them by modifier type
4. Not all modifiers will be appropriate for all base options within a parameter
5. Conflicting modifiers (e.g., "slightly" and "extremely") should not be used together

## Examples

- "moderately athletic-female build" - Parameter 4 with intensity modifier
- "high, narrow feminine slope forehead" - Parameter 10 with height and width modifiers
- "large, distinctly upturned almond eyes" - Parameter 13 with size and angle modifiers
- "silky, glossy straight hair" - Parameter 20 with multiple quality modifiers
- "tight, sleek high ponytail" - Parameter 27 with tightness and neatness modifiers

## Conditional Conflicts

The A&A engine should respect the existing conditional conflicts defined in the HBS Control File. Modifiers do not override these conflicts but rather enhance the parameters within their valid ranges.
