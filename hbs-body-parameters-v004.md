# Human Builder System - Body Parameters v004

## Cross-File Dependencies
This file contains parameters that affect options in other files:
- Gender affects facial feature options in the Facial Features file
- Gender affects certain hair styling options in the Hair Attributes file
- Age affects facial features in the Facial Features file
- Age affects hair styles in the Hair Attributes file

See the Control File for a complete parameter dependency map.

## 1. Gender
**Description:** Primary gender classification for character creation

**Options:**
* **Identify as male**
* **Identify as female**

**Exclusion Rules:**
* When "Identify as male" is selected, the following female body types are excluded:
  * hourglass-female
  * pear-female
  * apple-female
  * rectangle-female
  * inverted-triangle-female
  * athletic-female
  * curvy-female
  * slender-female
  * plus-size-female
  * stocky-female
* This exclusion occurs because these body types are not typically interpretable on male characters by the T2I engine.

**External Dependencies:**
* Gender selection affects available options for Forehead, Jawline, Cheekbones, Eyes, Eyebrows, Nose, and Mouth in the Facial Features file
* Gender selection enables or disables Facial Hair in the Facial Features file
* Gender selection influences probable selections for Hair Styling in the Hair Attributes file

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

**External Dependencies:**
* Heritage selection influences probable selections for Skin Tone and Hair Texture, though any combination is valid

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

**Internal Dependencies:**
* Visual Heritage selection influences likelihood of certain skin tone selections, but any combination is valid

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

**Internal Dependencies:**
* Age selection influences probability of certain skin textures (e.g., "Flawless Smooth" more common with younger age settings)

## 5. Age
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

**External Dependencies:**
* Age selection influences probable skin texture options
* Age selection affects facial feature rendering in the Facial Features file
* Age selection influences hair styling and coloration options in the Hair Attributes file

## 6. Build
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

**Internal Dependencies:**
* Gender selection directly determines which build options are available

## 7. Height
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

**Internal Dependencies:**
* Gender selection affects the specific height ranges associated with each category
* Build selection influences height perception in generated images