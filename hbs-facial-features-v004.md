# Human Builder System - Facial Features v004

## Cross-File Dependencies
This file contains parameters that are affected by options in other files:
- Many facial features have gender-conditional options based on Gender from the Body Parameters file
- Facial Hair is conditionally displayed based on Gender from the Body Parameters file
- Facial features are influenced by Age from the Body Parameters file

See the Control File for a complete parameter dependency map.

## 8. Head Shape
**Description:** Overall cranial structure that forms the foundation of facial appearance

**Options:**
* **Oval**
  * Visual: Slightly elongated curved form with balanced proportions
  * As seen in: Classical artistic representations, considered universally balanced
* **Round**
  * Visual: Circular shape with equal width and height, softer angles
  * As seen in: Certain East Asian populations, youthful appearances
* **Square**
  * Visual: Angular with similar width at forehead and jaw, strong lines
  * As seen in: Classic masculine ideal, strong-featured individuals
* **Rectangular**
  * Visual: Elongated square shape with vertical emphasis
  * As seen in: Certain European populations, longer facial structures
* **Heart**
  * Visual: Wider at forehead tapering to a narrower chin point
  * As seen in: Classic feminine ideal, certain youthful faces
* **Diamond**
  * Visual: Narrow forehead widening at cheekbones then tapering to chin
  * As seen in: Fashion models, distinctive angular appearances
* **Triangle**
  * Visual: Narrow forehead widening significantly at jawline
  * As seen in: Certain body types, faces with prominent lower features
* **Inverted-Triangle**
  * Visual: Wide forehead narrowing significantly toward chin
  * As seen in: Certain athletic builds, faces with prominent upper features
* **Long**
  * Visual: Vertically extended with narrow proportions throughout
  * As seen in: Certain European and African populations
* **Baseball**
  * Visual: Shortened oval with slight angularity at sides
  * As seen in: Certain East Asian and Native American populations

**Internal Dependencies:**
* Face Shape is often correlated with Head Shape but can be selected independently

## 9. Face Shape
**Description:** Distinctive facial contour that defines overall appearance

**Options:**
* **Oval**
  * Visual: Slightly elongated curved form with balanced proportions
  * As seen in: Considered universally flattering, many fashion models
* **Round**
  * Visual: Full cheeks with soft angles and similar width/height
  * As seen in: Youthful appearances, certain East Asian populations
* **Square**
  * Visual: Strong jawline creating angular corners at similar width to forehead
  * As seen in: Strong-featured individuals, certain masculine ideals
* **Rectangular**
  * Visual: Elongated with angular jaw and similar width at forehead/jawline
  * As seen in: Longer facial structures, certain European populations
* **Heart**
  * Visual: Wide forehead and cheekbones tapering to a pointed chin
  * As seen in: Classic feminine ideal, faces with prominent cheekbones
* **Diamond**
  * Visual: Narrow forehead and jawline with prominent cheekbones
  * As seen in: High-fashion models, distinctive angular appearances
* **Triangle**
  * Visual: Narrow forehead with wide jawline creating bottom-heavy appearance
  * As seen in: Faces with prominent jaw structures
* **Inverted-Triangle**
  * Visual: Wide forehead tapering significantly to narrow chin
  * As seen in: Faces with prominent upper features
* **Long**
  * Visual: Vertically extended with narrow proportions throughout
  * As seen in: Certain European and African populations
* **Baseball**
  * Visual: Shortened oval with slight angularity at sides
  * As seen in: Certain East Asian and Native American populations

**External Dependencies:**
* Gender selection from Body Parameters influences probability of certain face shapes, though any option is valid for either gender

## 10. Forehead
**Description:** Upper facial feature that frames the face and influences overall proportions

**Gender-Conditional Options:**

**For "Identify as female":**
* **Smooth High**
  * Visual: Vertically extended with even surface and minimal texture
  * As seen in: Classical feminine beauty, balanced facial proportions
* **Gentle Rounded**
  * Visual: Soft curved surface with harmonious transitions
  * As seen in: Youthful feminine appearances, softer facial features
* **Delicate Flat**
  * Visual: Minimal protrusion with refined even surface
  * As seen in: Certain East Asian feminine features, elegant proportions
* **Feminine Slope**
  * Visual: Subtle backward incline from brow to hairline
  * As seen in: Classical female profiles, graceful facial angles
* **Vertical Balanced**
  * Visual: Perpendicular angle to facial plane with smooth texture
  * As seen in: Symmetrical feminine features, modern beauty standards

**For "Identify as male":**
* **Pronounced High-and-Wide**
  * Visual: Vertically extended with significant horizontal span
  * As seen in: Classical masculine representations, strong features
* **Rugged Receding**
  * Visual: Noticeable backward slope from brow line toward hairline
  * As seen in: Mature masculine features, distinctive male profiles
* **Bossed Prominent**
  * Visual: Forward projection with distinct prominence above brows
  * As seen in: Strong-featured males, powerful masculine appearances
* **Strong Flat**
  * Visual: Minimal slope with substantial surface area
  * As seen in: Certain masculine ethnic features, balanced strong features
* **Brow-Heavy**
  * Visual: Developed ridge above eyes creating shadow effect
  * As seen in: Traditional masculine features, powerful expressions
* **Angled Structural**
  * Visual: Distinct planes creating architectural appearance
  * As seen in: Defined male features, sculptural facial structures

**External Dependencies:**
* Gender selection from Body Parameters file directly determines available forehead options

## 11. Jawline
**Description:** Lower facial structure that defines face shape and contributes to overall character

**Gender-Conditional Options:**

**For "Identify as female":**
* **Soft Oval**
  * Visual: Gently curved with smooth transitions and minimal angles
  * As seen in: Classical feminine features, balanced facial structures
* **Delicate Round**
  * Visual: Soft curves without distinct angles, subtle definition
  * As seen in: Youthful feminine appearances, softer facial features
* **Tapered Heart**
  * Visual: Rounded with a gentle point at the chin
  * As seen in: Traditional feminine beauty standards, certain models
* **Subtle Defined**
  * Visual: Noticeable but not prominent jawline with soft angles
  * As seen in: Athletic female features, fashion models
* **Graceful Wide**
  * Visual: Broader jawline maintaining feminine softness
  * As seen in: Strong-featured women, certain ethnic characteristics
* **Elegant Pointed**
  * Visual: Refined tapering to a noticeable chin point
  * As seen in: High fashion models, distinctive feminine profiles

**For "Identify as male":**
* **Strong Square**
  * Visual: Pronounced angular lines with defined corners
  * As seen in: Classic masculine jawlines, action figures
* **Bold Mandibular**
  * Visual: Prominent horizontal emphasis with distinct angle
  * As seen in: Masculine ideals, strong facial structures
* **Chiseled Defined**
  * Visual: Sharp delineation with noticeable angularity
  * As seen in: Athletic male features, defined masculine profiles
* **Broad Wide**
  * Visual: Extended lateral spread creating prominent lower face
  * As seen in: Strong masculine features, powerful appearances
* **Rugged Round**
  * Visual: Fuller jawline with moderate definition
  * As seen in: Natural masculine features, less angular profiles
* **Subtle Receding**
  * Visual: Less pronounced jawline with gradual transition to neck
  * As seen in: Certain male facial structures, intellectual appearances

**External Dependencies:**
* Gender selection from Body Parameters file directly determines available jawline options
* Face Shape selection influences appropriate jawline options

## 12. Cheekbones
**Description:** Facial bone structure that influences facial width and light dynamics

**Gender-Conditional Options:**

**For "Identify as female":**
* **High-and-Prominent**
  * Visual: Elevated position with noticeable projection
  * As seen in: Fashion models, distinctive feminine features
* **Softly-Rounded**
  * Visual: Gentle curves with smooth transitions and subtle definition
  * As seen in: Youthful appearances, classical feminine faces
* **Delicate-Features**
  * Visual: Refined structure with elegant contours
  * As seen in: Feminine beauty standards, subtle facial structures
* **Balanced-Asymmetry**
  * Visual: Naturally varied prominence between sides creating character
  * As seen in: Unique feminine faces, natural beauty standards
* **Dramatic-Contour**
  * Visual: Strongly defined with notable light-catching properties
  * As seen in: Editorial models, striking feminine features
* **Natural-Flow**
  * Visual: Harmoniously integrated with other facial features
  * As seen in: Balanced feminine faces, approachable appearances

**For "Identify as male":**
* **Angular-Definition**
  * Visual: Distinct planes with structural emphasis
  * As seen in: Masculine facial structures, defined features
* **Wide-and-Strong**
  * Visual: Broad structure creating facial width
  * As seen in: Powerful masculine appearances, strong features
* **Sculpted-Look**
  * Visual: Clearly defined with dramatic shadows
  * As seen in: Chiseled masculine features, heroic imagery
* **Flat-Profile**
  * Visual: Minimal projection with subtle definition
  * As seen in: Certain ethnic features, understated appearances
* **Weathered-Character**
  * Visual: Distinctive definition with maturity markers
  * As seen in: Experienced faces, character actors
* **Pronounced-Structure**
  * Visual: Highly visible bone structure influencing overall appearance
  * As seen in: Strong masculine features, distinctive profiles

**External Dependencies:**
* Gender selection from Body Parameters file directly determines available cheekbone options
* Age selection from Body Parameters influences visual expression of cheekbone options (e.g., more pronounced with age)
* Face Shape influences perception of cheekbone prominence

## 13. Eyes
**Description:** Shape and positioning of eyes that significantly impact facial expression and character

**Gender-Conditional Main Options:**

**For "Identify as female":**
* **Almond**
  * Visual: Elongated oval shape with subtle tapering at corners
  * As seen in: Classic feminine beauty standards, balanced elegant eyes
* **Round**
  * Visual: Circular shape with open appearance and minimal corner angles
  * As seen in: Youthful feminine features, certain anime-inspired looks
* **Hooded**
  * Visual: Partially covered by upper eyelid creating depth
  * As seen in: Mature feminine faces, certain ethnic characteristics
* **Monolid**
  * Visual: Smooth upper eyelid without visible crease
  * As seen in: East Asian feminine features, certain global populations
* **Cat-Eyes**
  * Visual: Distinctly upward angle at outer corners
  * As seen in: Dramatic feminine looks, editorial fashion
* **Wide-Set**
  * Visual: Greater than average distance between eyes
  * As seen in: Certain unique feminine features, ethereal appearances
* **Close-Set**
  * Visual: Less than average distance between eyes
  * As seen in: Focused feminine gazes, intense expressions

**For "Identify as male":**
* **Almond**
  * Visual: Moderately elongated shape with defined corners
  * As seen in: Balanced masculine features, universally flattering eye shape
* **Deep-Set**
  * Visual: Positioned beneath prominent brow ridge creating shadow
  * As seen in: Strong masculine features, intense expressions
* **Hooded**
  * Visual: Partially covered by upper eyelid or brow ridge
  * As seen in: Mature masculine faces, certain rugged appearances
* **Monolid**
  * Visual: Smooth upper eyelid without visible crease
  * As seen in: East Asian masculine features, certain global populations
* **Narrow**
  * Visual: Horizontally compressed with subtle opening
  * As seen in: Strong masculine expressions, focused appearances
* **Wide-Set**
  * Visual: Greater than average distance between eyes
  * As seen in: Certain distinctive masculine features, approachable expressions
* **Close-Set**
  * Visual: Less than average distance between eyes
  * As seen in: Focused masculine gazes, concentrated expressions

**Modifiers (applicable to any eye shape):**
* **Upturned**
  * Visual: Outer corners positioned higher than inner corners
  * As seen in: Various facial structures across genders
* **Downturned**
  * Visual: Outer corners positioned lower than inner corners
  * As seen in: Various facial structures across genders

**Eye Shape Modifier Exclusions:**
* "Upturned" and "Downturned" modifiers cannot be applied simultaneously to the same character
* This restriction exists because the T2I engine cannot interpret contradictory eye angles

**External Dependencies:**
* Gender selection from Body Parameters file directly determines available main eye shape options
* Visual Heritage from Body Parameters influences probability of certain eye shapes (e.g., Monolid more common with East Asian heritage)
* Age affects the rendering of eye shapes (e.g., potential hooding increases with age)

## 14. Eye Color
**Description:** Color of the iris that contributes to facial impact and character distinctiveness

**Options:**
* **Brown**
  * Visual: Range from light amber to deep chocolate tones
  * As seen in: Most common global eye color, approximately 70-80% of population
* **Blue**
  * Visual: Range from pale ice blue to deep navy tones
  * As seen in: Approximately 8-10% of global population, more common in
* **Blue**
  * Visual: Range from pale ice blue to deep navy tones
  * As seen in: Approximately 8-10% of global population, more common in European heritage
* **Green**
  * Visual: Range from pale sage to deep emerald tones
  * As seen in: Rarest natural eye color, approximately 2% of global population
* **Hazel**
  * Visual: Multi-tonal blend of brown and green with gold flecks
  * As seen in: Approximately 5-8% of global population, varies with lighting conditions
* **Grey**
  * Visual: Range from light silver to deep slate tones
  * As seen in: Approximately 3% of global population, often appears blue-tinged
* **Other**
  * Visual: Non-standard eye colors including amber, violet, red, etc.
  * As seen in: Fantasy characters, certain aesthetic styles
  * Note: Text-to-image systems may interpret these colors inconsistently or default to more common natural colors

**External Dependencies:**
* Visual Heritage from Body Parameters influences probability of certain eye colors (e.g., Brown more common with non-European heritage)

## 15. Eyebrows
**Description:** Facial features that frame the eyes and significantly impact expression

**Gender-Conditional Main Shape Options:**

**For "Identify as female":**
* **Arched**
  * Visual: Curved upward with highest point above outer third of eye
  * As seen in: Classic feminine beauty standards, elegant expressions
* **Straight**
  * Visual: Minimal curve following horizontal line above eyes
  * As seen in: Modern minimalist looks, certain East Asian features
* **Rounded**
  * Visual: Gentle curve with soft angles throughout
  * As seen in: Youthful feminine appearances, approachable expressions
* **S-shaped**
  * Visual: Complex curve with multiple directional changes
  * As seen in: Distinctive fashionable looks, unique facial features
* **Soft-angled**
  * Visual: Subtle angle with gentle transitions between segments
  * As seen in: Balanced feminine features, natural elegant appearances
* **Curved**
  * Visual: Continuous smooth bend following eye contour
  * As seen in: Harmonious feminine faces, classical beauty standards

**For "Identify as male":**
* **Straight**
  * Visual: Horizontal line with minimal arc above eyes
  * As seen in: Strong masculine features, certain cultural aesthetics
* **Flat**
  * Visual: Low-arch horizontal shape with subtle definition
  * As seen in: Understated masculine features, certain ethnic characteristics
* **Angular**
  * Visual: Distinct change of direction creating visible corner
  * As seen in: Striking masculine features, defined expressions
* **Slightly Arched**
  * Visual: Subtle upward curve with minimal height
  * As seen in: Balanced masculine features, approachable expressions
* **Bold Straight**
  * Visual: Prominent horizontal shape with minimal curve
  * As seen in: Strong masculine features, powerful expressions
* **Natural Line**
  * Visual: Following orbital bone with modest definition
  * As seen in: Classic masculine faces, natural appearances

**Modifiers (applicable to any eyebrow shape):**
* **Bushy**
  * Visual: Dense hair with substantial volume
  * As seen in: Natural untamed appearances, certain masculine styles
* **Thin**
  * Visual: Minimal width with precise definition
  * As seen in: Groomed appearances, certain fashion styles
* **Tapered**
  * Visual: Gradually narrowing from inner to outer edges
  * As seen in: Refined appearances, balanced facial features
* **High-set**
  * Visual: Positioned with significant space above eyes
  * As seen in: Surprised expressions, certain unique facial structures
* **Low-set**
  * Visual: Positioned closer to eyes with minimal space between
  * As seen in: Intense expressions, certain ethnic characteristics
* **Feathered**
  * Visual: Individual hairs visible creating textured appearance
  * As seen in: Natural untamed styles, current beauty trends
* **Groomed**
  * Visual: Clearly defined shape with precise edges
  * As seen in: Polished appearances, contemporary styling
* **Asymmetric**
  * Visual: Intentional or natural variation between sides
  * As seen in: Unique character faces, expressive features

**External Dependencies:**
* Gender selection from Body Parameters file directly determines available main eyebrow shape options
* Age from Body Parameters influences probability of certain eyebrow modifiers

## 16. Nose
**Description:** Central facial feature that significantly influences profile and frontal appearance

**Gender-Conditional Main Shape Types:**

**For "Identify as female":**
* **Straight**
  * Visual: Even bridge line without curves or angles
  * As seen in: Classical feminine profiles, balanced facial features
* **Button**
  * Visual: Small rounded shape with slightly upturned tip
  * As seen in: Youthful feminine appearances, certain idealized features
* **Celestial**
  * Visual: Gently curved bridge with upturned tip
  * As seen in: Delicate feminine profiles, softer facial features
* **Roman**
  * Visual: Subtle convex curve with refined proportions
  * As seen in: Elegant feminine profiles, certain Mediterranean features
* **Nubian**
  * Visual: Low bridge with wider nostrils and distinct definition
  * As seen in: Certain African and Middle Eastern feminine features
* **Greek**
  * Visual: Straight bridge continuing line of forehead
  * As seen in: Classical beauty standards, sculptural feminine profiles

**For "Identify as male":**
* **Straight**
  * Visual: Even bridge line with proportional width
  * As seen in: Balanced masculine profiles, universal facial features
* **Aquiline**
  * Visual: Prominent convex curve creating "eagle-like" appearance
  * As seen in: Strong masculine profiles, certain Mediterranean features
* **Roman**
  * Visual: Distinct convex curve with substantial bridge
  * As seen in: Classical masculine profiles, distinguished appearances
* **Hawk**
  * Visual: Pronounced convex curve with sharp downward angle at tip
  * As seen in: Powerful masculine features, distinctive profiles
* **Nubian**
  * Visual: Low bridge with wider nostrils and substantial presence
  * As seen in: Certain African and Middle Eastern masculine features
* **Bulbous**
  * Visual: Enlarged rounded tip with unique character
  * As seen in: Distinctive masculine features, mature appearances
* **Snub**
  * Visual: Short with slightly upturned tip
  * As seen in: Certain masculine facial structures, approachable features

**Modifiers (applicable to any nose type):**
* **Narrow-bridge**
  * Visual: Thin upper portion connecting to forehead
  * As seen in: Various facial structures across ethnicities
* **Wide-base**
  * Visual: Broader lower portion where nostrils connect
  * As seen in: Various facial structures across ethnicities
* **High-bridge**
  * Visual: Prominent elevation from facial plane
  * As seen in: Various facial structures across ethnicities
* **Low-bridge**
  * Visual: Minimal elevation from facial plane
  * As seen in: Various facial structures, particularly East Asian features
* **Flared-nostrils**
  * Visual: Expanded nostril width creating broader appearance
  * As seen in: Various facial structures across ethnicities
* **Narrow-nostrils**
  * Visual: Compressed nostril width creating slender appearance
  * As seen in: Various facial structures across ethnicities
* **Rounded-tip**
  * Visual: Soft curved endpoint without angular features
  * As seen in: Various facial structures across ethnicities
* **Pointed-tip**
  * Visual: More defined endpoint with angular quality
  * As seen in: Various facial structures across ethnicities
* **Asymmetric**
  * Visual: Natural variation between sides creating unique character
  * As seen in: Natural human variation across all populations
* **Deviated-septum**
  * Visual: Visible shift of center line creating distinctive appearance
  * As seen in: Natural human variation, often from prior injury
* **Upturned**
  * Visual: Tip angled upward from the base, creating a slightly elevated appearance
  * As seen in: Various facial structures across ethnicities, particularly common in certain feminine features

**External Dependencies:**
* Gender selection from Body Parameters file directly determines available main nose shape options
* Visual Heritage from Body Parameters influences probability of certain nose shapes
* Age from Body Parameters affects rendering of nose (e.g., potential enlargement with age)

## 17. Mouth
**Description:** Facial feature that significantly impacts expression and character appearance

**Gender-Conditional Options:**

**For "Identify as female":**
* **Small**
  * Visual: Compact size with delicate proportions
  * As seen in: Certain feminine beauty standards, delicate facial features
* **Medium**
  * Visual: Balanced proportions harmonious with other facial features
  * As seen in: Universal feminine facial proportions, natural appearances
* **Wide**
  * Visual: Extended horizontally creating expressive appearance
  * As seen in: Certain distinctive feminine features, expressive faces
* **Thin**
  * Visual: Minimal vertical height with refined appearance
  * As seen in: Certain elegant feminine features, mature appearances
* **Upturned**
  * Visual: Corners naturally angled upward creating subtle smile effect
  * As seen in: Friendly feminine expressions, certain youthful appearances
* **Downturned**
  * Visual: Corners naturally angled downward creating thoughtful appearance
  * As seen in: Serious feminine expressions, certain distinctive features
* **Bow-shaped**
  * Visual: Defined cupid's bow with curved upper lip
  * As seen in: Classic feminine beauty standards, refined features

**For "Identify as male":**
* **Medium**
  * Visual: Proportional size harmonious with other facial features
  * As seen in: Balanced masculine facial structures, natural appearances
* **Large**
  * Visual: Substantial size creating distinctive appearance
  * As seen in: Certain expressive masculine features, character faces
* **Wide**
  * Visual: Extended horizontally with strong presence
  * As seen in: Distinctive masculine features, expressive faces
* **Thin**
  * Visual: Minimal vertical height with precise appearance
  * As seen in: Certain masculine features, mature appearances
* **Neutral**
  * Visual: Even horizontal line without significant turning
  * As seen in: Composed masculine expressions, professional appearances
* **Downturned**
  * Visual: Corners naturally angled downward creating serious appearance
  * As seen in: Authoritative masculine expressions, certain distinctive features
* **Strong-lined**
  * Visual: Defined contours with clear boundaries
  * As seen in: Distinctive masculine features, character faces

**External Dependencies:**
* Gender selection from Body Parameters file directly determines available mouth options
* Facial structure options influence perception of mouth size and shape

## 18. Lips
**Description:** Shape and fullness of the lips

**Gender-Conditional Options:**

**For "Identify as female":**
* **Thin**
  * Visual: Minimal vertical height with delicate appearance
  * As seen in: Certain elegant feminine features, mature appearances
* **Medium**
  * Visual: Balanced fullness harmonious with other facial features
  * As seen in: Universal feminine facial proportions, natural appearances
* **Full**
  * Visual: Substantial volume creating defined appearance
  * As seen in: Contemporary feminine beauty standards, youthful appearances
* **Wide**
  * Visual: Extended horizontally with distinctive proportions
  * As seen in: Certain distinctive feminine features, expressive faces
* **Bow-shaped**
  * Visual: Defined cupid's bow with curved upper lip
  * As seen in: Classic feminine beauty standards, refined features
* **Round**
  * Visual: Soft curved shape with even fullness
  * As seen in: Youthful feminine appearances, approachable features
* **Defined**
  * Visual: Clear borders with precise shape
  * As seen in: Editorial beauty standards, striking features
* **Asymmetric**
  * Visual: Natural variation between sides creating character
  * As seen in: Unique feminine faces, distinctive appearances

**For "Identify as male":**
* **Thin**
  * Visual: Minimal vertical height with precise lines
  * As seen in: Certain masculine features, mature appearances
* **Medium**
  * Visual: Balanced proportions appropriate to facial structure
  * As seen in: Typical masculine facial features, natural appearances
* **Full**
  * Visual: More substantial volume creating defined appearance
  * As seen in: Certain masculine beauty standards, expressive features
* **Wide**
  * Visual: Extended horizontally with strong presence
  * As seen in: Distinctive masculine features, character faces
* **Defined**
  * Visual: Clear borders with precise shape
  * As seen in: Modern masculine beauty standards, refined features
* **Natural**
  * Visual: Organic shape without exaggerated features
  * As seen in: Everyday masculine faces, approachable appearances
* **Asymmetric**
  * Visual: Natural variation between sides adding character
  * As seen in: Unique masculine faces, distinctive appearances

**External Dependencies:**
* Gender selection from Body Parameters file directly determines available lip options
* Visual Heritage from Body Parameters influences probability of certain lip shapes
* Mouth selection directly affects available lip options

## 19. Facial Hair
**Description:** Presence and style of hair growth on the face

**Condition:** Display only when "Gender" = "Identify as male" or when explicitly enabled for other gender selections

**Options:**
* **Clean Shaven**
  * Visual: No visible facial hair, smooth skin appearance
  * As seen in: Many professional environments, certain cultural preferences
* **Light Stubble**
  * Visual: Short, even growth showing hair follicles without significant length
  * As seen in: "Five o'clock shadow," early beard growth
* **Heavy Stubble**
  * Visual: Prominent short facial hair creating textured appearance
  * As seen in: "Designer stubble," 3-7 days of growth
* **Mustache**
  * Visual: Hair growth specifically above the upper lip
  * As seen in: Various styles from thin to full
* **Goatee**
  * Visual: Hair on chin and mustache with shaved cheeks
  * As seen in: Contemporary professional environments, artistic communities
* **Short Beard**
  * Visual: Full facial hair kept trimmed close to the face
  * As seen in: Modern professional settings, contemporary fashion
* **Full Beard**
  * Visual: Complete facial hair coverage with moderate length
  * As seen in: Traditional styles, contemporary fashion trends
* **Long Beard**
  * Visual: Extended facial hair growth past the chin
  * As seen in: Certain religious traditions, specific subcultures

**External Dependencies:**
* Gender selection from Body Parameters file determines whether this parameter is displayed
* Age from Body Parameters influences the visual density and distribution of facial hair