# Human Builder System (HBS) Taxonomy

## 1. Gender
**Description:** Primary gender classification for character creation

**Options:**
* **Identify as male**
* **Identify as female**

*Note: This parameter affects available body build options through exclusion rules (certain body types are restricted based on gender selection).*

*Note: When "Identify as male" is selected, the following female body types are excluded:*
* *hourglass-female*
* *pear-female*
* *apple-female*
* *rectangle-female*
* *inverted-triangle-female*
* *athletic-female*
* *curvy-female*
* *slender-female*
* *plus-size-female*
* *stocky-female*

*This exclusion occurs because these body types are not typically interpretable on male characters by the T2I engine.*

## 2. Visual Heritage
**Description:** Foundational physical characteristics influenced by genetic ancestry that affect overall appearance

**Options:**
* **European Heritage**
  * Visual: May include lighter skin tones, varied eye colors, straight to wavy hair textures
  * As seen in: European populations, European-descended populations worldwide
* **African Heritage**
  * Visual: May include darker skin tones, tightly coiled hair textures, fuller lips
  * As seen in: African populations, African-descended populations worldwide
* **East Asian Heritage**
  * Visual: Often includes straight black hair, monolid or almond-shaped eyes, flatter facial profiles
  * As seen in: Chinese, Japanese, Korean and related populations
* **South Asian Heritage**
  * Visual: May include brown skin tones, dark hair and eyes, varied facial features
  * As seen in: Indian subcontinent populations and diaspora
* **Southeast Asian Heritage**
  * Visual: Often includes tan skin tones, straight black hair, varied eye shapes
  * As seen in: Thai, Vietnamese, Filipino, Indonesian populations
* **Latino Heritage**
  * Visual: Highly varied appearance with characteristics from multiple heritage groups
  * As seen in: Central and South American populations and diaspora
* **Custom Heritage**
  * Visual: Allows for precise specification of desired characteristics
  * As seen in: Mixed heritage backgrounds, specific desired appearances
  * Note: Acts as an override for targeted appearance control

## 3. Skin Tone
**Description:** Natural human skin color variations that provide nuanced control over appearance

**Options:**
* **Porcelain Pale Complexion**
  * Visual: Very fair skin that may show blue undertones or veins
  * As seen in: Northern European populations, albinism
* **Fair Rosy Skin**
  * Visual: Pale skin with a natural flush or rosy quality
  * As seen in: Celtic heritage, Northwestern European populations
* **Light Beige Tone**
  * Visual: Light skin with subtle warmth rather than pink tones
  * As seen in: Central European populations, many East Asians
* **Medium Warm Hue**
  * Visual: Neither notably light nor dark, with warm undertones
  * As seen in: Southern European populations, Middle East, some Latin American regions
* **Sun-Kissed Tan**
  * Visual: Appears naturally tanned or sun-exposed
  * As seen in: Mediterranean populations, Middle Eastern regions
* **Olive Undertone Skin**
  * Visual: Mediterranean appearance with green-gray cast
  * As seen in: Greek, Italian, Turkish populations
* **Golden Caramel Shade**
  * Visual: Deep warm tone with golden or honey qualities
  * As seen in: South Asian populations, North African regions
* **Deep Bronze Coloring**
  * Visual: Rich, deep skin with warm, reddish qualities
  * As seen in: Southeast Asian populations, indigenous American groups
* **Rich Mahogany Tone**
  * Visual: Deep brown skin with subtle reddish qualities
  * As seen in: East African populations, South Indian regions
* **Dark Ebony Skin**
  * Visual: Deep black-brown skin with little to no redness
  * As seen in: Central and West African populations

## 4. Skin Texture
**Description:** Surface quality and condition of skin that affects visual appearance and perceived age

**Options:**
* **Flawless Smooth**
  * Visual: Perfectly even, pore-less appearance with uniform texture
  * As seen in: Studio photography, digital enhancements, some youthful skin
* **Fine-Pored**
  * Visual: Smooth with minimally visible pores and even surface
  * As seen in: Naturally youthful or well-maintained skin
* **Normal Textured**
  * Visual: Balanced texture with visible pores and natural variations
  * As seen in: Typical healthy adult skin
* **Matte Finish**
  * Visual: Non-reflective surface with minimal shine
  * As seen in: Certain skin types or after powder application
* **Dewy Fresh**
  * Visual: Slightly luminous with natural moisture
  * As seen in: Well-hydrated skin, certain makeup applications
* **Weather-Worn**
  * Visual: Slightly roughened texture from environmental exposure
  * As seen in: Outdoor workers, sailors, farmers
* **Line-Detailed**
  * Visual: Natural fine lines that add character without appearing aged
  * As seen in: Expressive faces, mature adults
* **Textured Mature**
  * Visual: Visible pores, fine wrinkles, and natural aging patterns
  * As seen in: Middle-aged to elderly individuals
* **Scarred Character**
  * Visual: Distinctive marking patterns that add uniqueness
  * As seen in: Various life experiences, certain professions
* **Condition-Specific**
  * Visual: Custom textures for specific character needs
  * As seen in: Specialized character development requirements

## 5. Facial Hair
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

## 6. Age
**Description:** Life stage classifications that determine physical development and appearance

**Options:**
* **Pre-adolescent Child**
  * Visual: Youthful features, larger head-to-body ratio, softer facial contours
  * As seen in: Children ages 4-12, elementary school age range
* **Teenage Years**
  * Visual: Developing adult features, varied proportions, some facial definition
  * As seen in: Adolescents ages 13-19, high school to early college age range
* **Youthful Adult Appearance**
  * Visual: Fully developed but with minimal aging signs, smooth skin texture
  * As seen in: Young adults ages 20-29, early career stage
* **Mature Adult Features**
  * Visual: Completely developed features with minimal aging signs
  * As seen in: Adults ages 30-45, established life stage
* **Middle-aged Characteristics**
  * Visual: Beginning signs of aging like fine lines, slight facial softening
  * As seen in: Adults ages 46-65, mid-to-late career stage
* **Elderly Senior Traits**
  * Visual: Pronounced aging signs including wrinkles, age spots, facial sagging
  * As seen in: Adults ages 65+, retirement and beyond

## 7. Build
**Description:** Physical body structure types specific to gender presentation

**Gender-Conditional Options:**

**For "Identify as female":**
* **Slender-Female**
  * Visual: Lean and long with subtle curves and fine bone structure
  * As seen in: Fashion models, ballet dancers, naturally thin builds
* **Rectangle-Female**
  * Visual: Similar measurements at shoulders, waist, and hips with minimal curves
  * As seen in: Athletic builds, fashion models, straighter silhouette
* **Inverted-Triangle-Female**
  * Visual: Broader shoulders narrowing to slimmer hips
  * As seen in: Athletic swimmers, certain body types
* **Athletic-Female**
  * Visual: Toned with visible muscle definition while maintaining feminine shape
  * As seen in: Fitness enthusiasts, athletes, dancers
* **Pear-Female**
  * Visual: Narrower shoulders with wider hips and thighs
  * As seen in: Common natural female shape, lower-body-dominant proportions
* **Hourglass-Female**
  * Visual: Balanced proportions between bust and hips with defined waist
  * As seen in: Classic feminine silhouette, fashion models, certain actresses
* **Apple-Female**
  * Visual: Fuller midsection with slimmer lower body and proportional shoulders
  * As seen in: Upper-body-dominant proportions, certain body types
* **Curvy-Female**
  * Visual: Pronounced curves with soft transitions between body areas
  * As seen in: Plus-size models, voluptuous figures
* **Stocky-Female**
  * Visual: Compact frame with dense muscle structure and solid appearance
  * As seen in: Certain athletes, powerlifters, sturdy builds
* **Plus-Size-Female**
  * Visual: Fuller figure with proportional distribution and soft contours
  * As seen in: Plus-size models, certain body positive representations

**For "Identify as male":**
* **Lean-Male**
  * Visual: Slender build with visible muscle definition and minimal body fat
  * As seen in: Distance runners, swimmers, naturally thin builds
* **Rectangle-Male**
  * Visual: Straight silhouette with similar width at shoulders and hips
  * As seen in: Average builds, certain body types
* **Athletic-Male**
  * Visual: Defined muscles with low body fat percentage and balanced proportions
  * As seen in: Fitness models, certain athletes
* **Hourglass-Male**
  * Visual: Proportional shoulders and hips with defined waist
  * As seen in: Certain dancers, naturally balanced physiques
* **V-Shaped-Male**
  * Visual: Broad shoulders tapering to narrow waist with clear definition
  * As seen in: Swimmers, classic masculine ideal, superhero physiques
* **Muscular-Male**
  * Visual: Substantial muscle mass with defined contours and powerful appearance
  * As seen in: Bodybuilders, strength athletes, action heroes
* **Stocky-Male**
  * Visual: Compact powerful frame with thick limbs and solid core
  * As seen in: Rugby players, powerlifters, naturally dense builds
* **Endomorph-Male**
  * Visual: Softer contours with higher fat distribution and substantial frame
  * As seen in: Certain body types, larger builds with less definition
* **Heavyset-Male**
  * Visual: Large frame with substantial presence and powerful appearance
  * As seen in: Football linemen, strongmen competitors

## 8. Height
**Description:** Vertical stature measurement

**Options:**
* **Very Short**
  * Visual: Significantly below average height
  * As seen in (male): Adult men under 5'4" (163cm)
  * As seen in (female): Adult women under 4'11" (150cm)
* **Short**
  * Visual: Below average height but within common range
  * As seen in (male): Adult men 5'4"-5'7" (163-170cm)
  * As seen in (female): Adult women 4'11"-5'3" (150-160cm)
* **Average**
  * Visual: Typical height range for gender
  * As seen in (male): Adult men 5'8"-5'11" (173-180cm)
  * As seen in (female): Adult women 5'4"-5'6" (163-168cm)
* **Tall**
  * Visual: Above average height but within common range
  * As seen in (male): Adult men 6'0"-6'3" (183-190cm)
  * As seen in (female): Adult women 5'7"-5'10" (170-178cm)
* **Very Tall**
  * Visual: Significantly above average height
  * As seen in (male): Adult men above 6'3" (190cm)
  * As seen in (female): Adult women above 5'10" (178cm)

## 9. Head Shape
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

## 10. Face Shape
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

## 11. Forehead
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

## 12. Jawline
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

## 13. Cheekbones
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

## 14. Eyes
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

## 15. Eye Color
**Description:** Color of the iris that contributes to facial impact and character distinctiveness

**Options:**
* **Brown**
  * Visual: Range from light amber to deep chocolate tones
  * As seen in: Most common global eye color, approximately 70-80% of population
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

## 16. Eyebrows
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

## 17. Nose
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

## 18. Mouth
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
  * As seen in: Thoughtful masculine expressions, certain distinctive features
* **Strong-lined**
  * Visual: Defined contours with clear boundaries
  * As seen in: Distinctive masculine features, character faces

## 19. Lips
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

## 27. Hair Style
**Description:** Specifies the way the hair is styled and positioned

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

* **Pigtails**
  * Visual: Two sections styled into two tails
  * As seen in: Playful styling, youthful presentations

**Hair Style Modifier Exclusions:**
* "Messy" and "Neatly Styled" modifiers cannot be applied simultaneously to the same hairstyle
* When "Bald" is selected, hair color options are not applicable