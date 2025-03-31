# Human Builder System - Hair Attributes v004

## Cross-File Dependencies
This file contains parameters that are affected by options in other files:
- Hair styling options are influenced by Gender from the Body Parameters file
- Hair color and styling are influenced by Age from the Body Parameters file
- Hair texture has some correlation with Visual Heritage from the Body Parameters file

This file also contains internal dependencies between parameters:
- Hair Style options depend on Hair Length selection
- Hair Style modifiers have exclusion rules between incompatible options
- Bald styling affects applicability of Hair Color options

See the Control File for a complete parameter dependency map.

## 20. Hair Texture
**Description:** Describes the natural surface appearance and feel of individual hair strands

**Options:**
* **Straight**
  * Visual: Lacking any natural bends or curves
  * As seen in: East Asian populations, straight-haired individuals across all ethnicities

* **Wavy**
  * Visual: Characterized by gentle "S" shaped curves from root to tip
  * As seen in: Mediterranean populations, wavy-haired individuals across all ethnicities

* **Curly**
  * Visual: Formed in defined spirals or ringlets
  * As seen in: Various populations globally, particularly common in certain European and Middle Eastern regions

* **Coily**
  * Visual: Manifesting tight, spring-like formations, often with a zig-zag pattern
  * As seen in: African populations, African-descended populations worldwide

* **Kinky**
  * Visual: Displaying very tight, angular coils in a defined zig-zag pattern
  * As seen in: African populations, African-descended populations worldwide

**External Dependencies:**
* Visual Heritage from Body Parameters influences probability of certain hair textures
* This parameter affects the rendering of virtually all other hair parameters

## 21. Hair Density
**Description:** Quantifies the thickness of the hair by measuring the number of strands present on the head

**Options:**
* **Fine Density**
  * Visual: Thin, with fewer strands per square inch
  * As seen in: Delicate hair appearances, subtle hair presence

* **Medium Density**
  * Visual: Average thickness, possessing a moderate amount of strands
  * As seen in: Balanced hair volume, typical hair presentations

* **Thick Density**
  * Visual: Dense, with a high concentration of strands per square inch
  * As seen in: Voluminous hair presentations, substantial hair appearance

**Internal Dependencies:**
* Hair Texture influences perception of Hair Density
* Hair Volume is affected by Hair Density selection

## 22. Hair Volume
**Description:** Indicates the degree of fullness and body of a hairstyle

**Options:**
* **Flat Volume**
  * Visual: Lying close to the head with minimal lift
  * As seen in: Sleek styles, minimalist hair presentations

* **Slight Volume**
  * Visual: Exhibiting a small amount of lift and body
  * As seen in: Natural casual looks, subtle styling

* **Medium Volume**
  * Visual: Representing a moderate amount of fullness
  * As seen in: Balanced hair styling, everyday presentations

* **High Volume**
  * Visual: Displaying significant lift and body
  * As seen in: Dramatic styling, statement hairstyles

* **Voluminous**
  * Visual: Achieving an exceptionally full and puffy aesthetic
  * As seen in: Editorial looks, extravagant styling

**Internal Dependencies:**
* Hair Density directly influences achievable Hair Volume
* Hair Texture affects how volume is expressed visually
* Hair Style selection influences probable Hair Volume options

## 23. Hair Length
**Description:** Indicates the distance from the top of the head to the end of the hair

**Options:**
* **Buzz Cut**
  * Visual: Extremely short
  * As seen in: Military styling, minimalist appearances

* **Ear Length**
  * Visual: Approximately reaching the ears
  * As seen in: Classic short styles, cropped looks

* **Chin Length**
  * Visual: Approximately reaching the chin
  * As seen in: Bob cuts, structured short hairstyles

* **Shoulder Length**
  * Visual: Approximately reaching the shoulders
  * As seen in: Medium hairstyles, versatile cuts

* **Mid-Back Length**
  * Visual: Approximately reaching halfway down the back
  * As seen in: Long hairstyles, flowing presentations

* **Waist Length**
  * Visual: Approximately reaching the waist
  * As seen in: Extra-long styling, dramatic hair presentations

* **Hip Length**
  * Visual: Approximately reaching the hips
  * As seen in: Extremely long hair, statement length appearances

**Hair Style and Length Exclusions:**
* When hair length is "Buzz Cut," longer styles such as ponytails, buns, and certain braided styles are unavailable
* When hair styles like "Pixie Cut," "Bob Cut," "Undercut," or "Pompadour" are selected, "Long" and "Medium" hair lengths are excluded as these styles inherently dictate a specific length range
* T2I engines are unlikely to generate correct hair length when the defined style dictates a different length

**External Dependencies:**
* Gender from Body Parameters influences probability of certain hair length selections
* Age from Body Parameters influences probability of certain hair length selections

**Internal Dependencies:**
* Hair Length directly affects available Hair Style options

## 24. Hair Color
**Description:** Denotes what the dominant shade of the hair is

**Options:**
* **Blonde**
  * **Light Blonde**
    * Visual: Very pale
    * As seen in: Nordic appearances, platinum styling

  * **Golden Blonde**
    * Visual: Warm and yellow-toned
    * As seen in: Sun-kissed looks, honey-colored styling

  * **Strawberry Blonde**
    * Visual: Reddish-blonde
    * As seen in: Copper-tinted blonde, warm pale red tones

  * **Medium Blonde**
    * Visual: Neutral
    * As seen in: Classic blonde appearances, balanced light tones

  * **Ash Blonde**
    * Visual: Cool and silver or gray-toned
    * As seen in: Modern cool styling, muted blonde presentations

  * **Dark Blonde**
    * Visual: Deep and rich
    * As seen in: Sandy colorations, deep golden tones

* **Red**
  * **Bright Red**
    * Visual: Vivid and intense
    * As seen in: Statement red styling, vibrant colorations

  * **Auburn**
    * Visual: Reddish-brown with warm undertones
    * As seen in: Natural redhead appearances, rich red-brown blends

  * **Deep Red**
    * Visual: Rich and dark
    * As seen in: Burgundy shades, wine-colored styling

* **Gray/White**
  * **White**
    * Visual: Pure, lacking pigment
    * As seen in: Silver hair styling, platinum appearances

  * **Gray**
    * Visual: Mixed with pigmented strands
    * As seen in: Natural aging, silver-toned presentations

  * **Salt and Pepper**
    * Visual: Varied mixture of gray and pigmented strands
    * As seen in: Distinguished appearances, mature styling

* **Brown**
  * **Light Brown**
    * Visual: Pale
    * As seen in: Soft brunette looks, caramel tones

  * **Golden Brown**
    * Visual: Warm and golden-toned
    * As seen in: Honey-brown coloration, sun-touched brunette

  * **Ash Brown**
    * Visual: Cool and silver or gray-toned
    * As seen in: Muted brown styling, cool-toned brunette

  * **Medium Brown**
    * Visual: Neutral
    * As seen in: Classic brunette appearances, standard brown tones

  * **Deep Brown**
    * Visual: Rich and dark
    * As seen in: Espresso coloration, dark chocolate tones

* **Black**
  * **Soft Black**
    * Visual: With a subtle sheen
    * As seen in: Natural black hair, blue-black reflections

  * **Deep Black**
    * Visual: Rich and dark
    * As seen in: Intense dark styling, statement black presentations

**External Dependencies:**
* Visual Heritage from Body Parameters influences probability of certain hair colors
* Age from Body Parameters influences probability of certain hair colors (e.g., gray/white more common with older age settings)

**Internal Dependencies:**
* Hair Style selection of "Bald" makes Hair Color options not applicable

## 25. Hair Parting
**Description:** Specifies positioning of the line where the hair divides on the head

**Options:**
* **Center Part**
  * Visual: Divided evenly down the middle
  * As seen in: Symmetrical styling, balanced presentations

* **Side Part**
  * Visual: Divided to one side, creating asymmetry
  * As seen in: Classic styling, professional appearances

* **Deep Side Part**
  * Visual: Parted dramatically to one side
  * As seen in: Dramatic styling, vintage-inspired looks

* **Zigzag Part**
  * Visual: Parted in a zigzag pattern
  * As seen in: Creative styling, textural interest

* **No Part**
  * Visual: Without a defined division
  * As seen in: Tousled styling, casual appearances

**Internal Dependencies:**
* Hair Length must be sufficient to show parting (not applicable to very short cuts)
* Hair Style affects how parting is expressed visually

## 26. Bangs/Fringe
**Description:** Specifies hair that is cut short and falling across the forehead

**Options:**
* **Blunt Bangs**
  * Visual: Cut straight across, typically at eyebrow level
  * As seen in: Graphic styling, bold hair statements

* **Wispy Bangs**
  * Visual: Thinned with soft edges that partially reveal the forehead
  * As seen in: Delicate styling, subtle framing

* **Shaggy Bangs**
  * Visual: Textured and layered, blending into the rest of the hair
  * As seen in: Casual styling, effortless appearances

* **Side-Swept Bangs**
  * Visual: Styled to sweep across the forehead, typically covering one side
  * As seen in: Asymmetrical styling, elegant framing

**Internal Dependencies:**
* Hair Length must be sufficient to support bangs (not applicable to very short cuts)
* Hair Texture affects how bangs lie and appear

## 27. Tails and Buns
**Description:** Specifies hairstyles with gathered sections secured at specific positions

**Options:**
* **Ponytail**
  * Visual: Gathered and secured
  * As seen in: Practical styling, athletic appearances

* **High Ponytail**
  * Visual: At the crown of the head
  * As seen in: Youthful styling, energetic presentations

* **Low Ponytail**
  * Visual: At the nape of the neck
  * As seen in: Elegant styling, refined appearances

* **Side Ponytail**
  * Visual: On one side of the head
  * As seen in: Asymmetrical styling, playful presentations

* **Pigtails**
  * Visual: Two sections styled into two tails
  * As seen in: Playful styling, youthful presentations

* **Bun**
  * Visual: Twisted into a circular coil and secured
  * As seen in: Practical styling, tidy appearances

* **Classic Bun**
  * Visual: Twisted into a circular coil and secured at the back of the head
  * As seen in: Traditional styling, polished presentations

* **Messy Bun**
  * Visual: Loosely twisted in an intentionally casual style
  * As seen in: Relaxed styling, effortless appearances

* **Top Knot**
  * Visual: High on the head
  * As seen in: Contemporary styling, fashion-forward looks

* **Chignon**
  * Visual: Low and smooth at the nape of the neck
  * As seen in: Formal styling, elegant appearances

**Internal Dependencies:**
* Hair Length must be sufficient to gather into tails or buns (generally shoulder length or longer)
* Hair Texture affects how tails and buns appear and hold

## 28. Hair Style
**Description:** Specifies other ways the hair is styled and positioned

**Options:**
* **Loose Natural**
  * Visual: Worn down without significant styling
  * As seen in: Everyday appearances, casual presentations
  
* **Braided**
  * Visual: Hair woven in various patterns
  * As seen in: Traditional styling, intricate presentations
  
* **Pixie Cut**
  * Visual: Very short, layered style with tapered back and sides
  * As seen in: Modern short styles, contemporary feminine looks
  
* **Bob Cut**
  * Visual: Blunt cut typically between ears and chin
  * As seen in: Classic structured short styles, refined appearances
  
* **Undercut**
  * Visual: Closely clipped sides and back with longer top
  * As seen in: Contemporary edgy styles, alternative presentations
  
* **Pompadour**
  * Visual: Volume at the front swept upward and back
  * As seen in: Vintage-inspired styles, dramatic presentations

* **Bald**
  * Visual: Head with minimal to no hair
  * As seen in: Minimalist presentations, certain cultural affiliations

**Hair Style Modifiers:**
* **Messy**
  * Visual: Intentionally disheveled with casual placement
  * As seen in: Relaxed styling, effortless appearances

* **Neatly Styled**
  * Visual: Precisely arranged with controlled placement
  * As seen in: Formal styling, professional appearances

* **Windblown**
  * Visual: Appearing moved by air currents with dynamic flow
  * As seen in: Outdoor imagery, movement-focused styles

* **Wet Look**
  * Visual: Appearing damp with sleek definition
  * As seen in: Contemporary styling, editorial fashion

* **Shiny**
  * Visual: Reflecting light with glossy finish
  * As seen in: Healthy hair representations, polished appearances

* **Matte**
  * Visual: Non-reflective with textural emphasis
  * As seen in: Natural styling, certain product-enhanced looks

**Hair Style Modifier Exclusions:**
* "Messy" and "Neatly Styled" modifiers cannot be applied simultaneously to the same hairstyle
* When "Bald" is selected, most hair modifiers are not applicable

**External Dependencies:**
* Gender from Body Parameters influences probability of certain hairstyles
* Age from Body Parameters influences probability of certain hairstyles

**Internal Dependencies:**
* Hair Length directly restricts available Hair Style options (e.g., ponytails require sufficient length)
* Hair Texture affects how different styles are rendered
* Hair Density affects the visual fullness of styling