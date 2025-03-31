# Human Builder System (HBS) - Control File v004

## Version Information
**Version:** v004
**Last Updated:** March 2025
**System Name:** T2I Human Build System

## System Overview
The Human Builder System (HBS) is a comprehensive taxonomy for defining human character parameters optimized for text-to-image (T2I) engines. This control file serves as the master reference for implementation and cross-file parameter relationships, including the Adjectives & Adverbs (A&A) engine.

## File Structure
The HBS taxonomy is divided into three primary files:

1. **Body Parameters** - Contains fundamental physical attributes including gender, ethnicity, skin properties, age, build, and height
2. **Facial Features** - Contains all parameters related to the face including head shape, facial features, and expressions
3. **Hair Attributes** - Contains all parameters related to hair including texture, density, volume, color, and styling

## Parameter Dependency Map

### Primary Dependencies (Cross-File)

| Parameter | File | Affects | In File | Relationship Type |
|-----------|------|---------|---------|------------------|
| Gender | Body | Build | Body | Exclusion |
| Gender | Body | Forehead | Face | Gender-Conditional Options |
| Gender | Body | Jawline | Face | Gender-Conditional Options |
| Gender | Body | Cheekbones | Face | Gender-Conditional Options |
| Gender | Body | Eyes | Face | Gender-Conditional Options |
| Gender | Body | Eyebrows | Face | Gender-Conditional Options |
| Gender | Body | Nose | Face | Gender-Conditional Options |
| Gender | Body | Mouth | Face | Gender-Conditional Options |
| Gender | Body | Facial Hair | Face | Conditional Display |
| Gender | Body | Hair Styling | Hair | Preference Weighting |
| Age | Body | Skin Texture | Body | Style Weighting |
| Age | Body | Facial Features | Face | Style Weighting |
| Age | Body | Hair Style | Hair | Style Weighting |
| Hair Length | Hair | Tails and Buns | Hair | Option Availability |
| Hair Style | Hair | Hair Color | Hair | Option Availability |

### Secondary Dependencies (Internal)

| Parameter | File | Affects | Relationship Type |
|-----------|------|---------|------------------|
| Build | Body | Height | Style Weighting |
| Eyes - Shape | Face | Eyes - Modifiers | Exclusion |
| Hair Texture | Hair | Hair Density | Style Weighting |
| Hair Style | Hair | Hair Volume | Style Weighting |

## Complete Exclusion Rules List

### Gender-Based Exclusions
When "Identify as male" is selected, the following female body types are excluded:
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

These body types are not typically interpretable on male characters by the T2I engine.

### Eye Modifier Exclusions
"Upturned" and "Downturned" modifiers cannot be applied simultaneously to the same character as the T2I engine cannot interpret contradictory eye angles.

### Hair Style and Length Exclusions
* When hair length is "Buzz Cut," longer styles such as ponytails, buns, and certain braided styles are unavailable
* When hair styles like "Pixie Cut," "Bob Cut," "Undercut," or "Pompadour" are selected, "Long" and "Medium" hair lengths are excluded as these styles inherently dictate a specific length range
* T2I engines are unlikely to generate correct hair length when the defined style dictates a different length

### Hair Style Modifier Exclusions
* "Messy" and "Neatly Styled" modifiers cannot be applied simultaneously to the same hairstyle
* When "Bald" is selected, hair color options are not applicable

## Adjectives & Adverbs (A&A) Engine Conflict Rules

### Direct Contradictions (Strict Enforcement)
These combinations should be prevented in the system:

1. **Contradictory Intensity Modifiers**
   * Prevent combinations like "slightly extremely" for any parameter
   * Only one intensity modifier should be applied to a parameter

2. **Contradictory Angle Modifiers**
   * Prevent combinations of "upturned" and "downturned" for eyes
   * Only one angle direction should be applied

3. **Contradictory Definition Modifiers**
   * Prevent combinations like "softly sharply defined" for any parameter
   * Only one definition modifier should be applied

4. **Contradictory Property Modifiers**
   * Prevent opposite properties like "silky coarse" or "dry glossy" for hair texture

### Base Parameter and Modifier Conflicts
These combinations are logically inconsistent:

1. **Eye Shape and Modifier Conflicts**
   * "Cat-Eyes" + "downturned" (Cat-Eyes are inherently upturned)
   * "Deep-Set" + "widely open" (creates interpretation issues)

2. **Nose Shape and Adjective Conflicts**
   * "Button Nose" + ["strong", "prominent"] (Button noses are inherently small)
   * "Aquiline/Hawk Nose" + ["subtle", "delicate"] (these noses are inherently prominent)

3. **Tails and Buns Style Conflicts**
   * "Tight" + "loose" (contradictory tightness)
   * "Sleek" + "messy" (contradictory neatness)

4. **Build Type and Intensity Conflicts**
   * "Slightly Muscular-Male" (contradictory as muscular implies definition)
   * "Extremely Slender-Female" (may push toward unhealthy appearance)

5. **Facial Hair Type and Density Conflicts**
   * "Dense Light Stubble" (light stubble is defined by sparseness)
   * "Sparse Full Beard" (fullness implies density)

## Processing Sequence Recommendations

For optimal parameter processing, implement in the following order:

1. **Primary Identity Parameters**
   - Gender
   - Visual Heritage
   - Age

2. **Body Structure Parameters**
   - Build (after Gender)
   - Height
   - Skin Tone
   - Skin Texture (after Age)

3. **Facial Structure Parameters**
   - Head Shape
   - Face Shape
   - Forehead (after Gender)
   - Jawline (after Gender)
   - Cheekbones (after Gender)

4. **Facial Feature Parameters**
   - Eyes (after Gender)
   - Eye Color
   - Eyebrows (after Gender)
   - Nose (after Gender)
   - Mouth (after Gender)
   - Lips
   - Facial Hair (after Gender)

5. **Hair Parameters**
   - Hair Texture
   - Hair Density
   - Hair Volume
   - Hair Length
   - Hair Color (after checking for "Bald")
   - Hair Parting
   - Bangs/Fringe
   - Tails and Buns (after Length)

## Implementation Guidelines

### T2I Prompt Construction
When constructing text-to-image prompts based on this taxonomy:

1. Use "identify as" phrasing rather than biological sex terminology
2. Order parameters from most influential to least influential
3. Place physical attributes before stylistic elements
4. Group related parameters (e.g., all facial features together)
5. Emphasize distinctive features that differentiate the character

### Adjectives & Adverbs Implementation
When implementing the A&A engine:

1. Apply modifiers only to parameters that have defined modifier sets
2. Use only one modifier per category (e.g., one intensity modifier)
3. Check for conflicts between modifiers and base parameters
4. Consider the visual impact of modifier combinations
5. Prioritize clarity over complexity - not every parameter needs modifiers

### Parameter Weighting
Not all parameters have equal influence on the generated image:

**High-Influence Parameters:**
* Gender
* Visual Heritage
* Age
* Build
* Skin Tone
* Eye Shape
* Hair Color
* Hair Style

**Medium-Influence Parameters:**
* Head Shape
* Face Shape
* Nose
* Hair Texture
* Hair Length
* Skin Texture

**Low-Influence Parameters:**
* Exact Height
* Subtle Facial Details
* Hair Volume
* Hair Parting

### Combining with Other Parameters
This taxonomy focuses exclusively on physical appearance. For complete character generation, consider combining with:

* Clothing/Attire
* Setting/Environment
* Pose/Action
* Lighting/Atmosphere
* Emotional Expression
* Artistic Style

## Validation Criteria
When validating parameter combinations:

1. Check for gender-based exclusions first
2. Validate internal dependencies within each file
3. Cross-validate parameters with dependencies across files
4. Check for logical inconsistencies (e.g., "Bald" with "Long Hair")
5. Verify age-appropriate feature combinations
6. Check for A&A engine conflicts (contradictory modifiers, etc.)

## Modifier Application Guidelines

1. Use only one modifier per modifier category (e.g., one intensity modifier, one angle modifier)
2. Avoid contradictory modifier combinations (e.g., "softly sharp")
3. Select modifiers appropriate to the base parameter (e.g., "refined" works for "button nose" but "strong" does not)
4. Use modifiers sparingly for clarity - not every parameter needs modifiers
5. For parameters without listed modifiers, no modifiers should be applied

## Future Enhancements
Areas for potential expansion in future versions:

1. Specific clothing/attire taxonomy integration
2. Extended cultural variation options
3. Additional accessibility/inclusivity parameters
4. Enhanced emotional expression options
5. Expanded modifier system for fine-tuning
6. Pose and composition parameter integration

## Checksum Verification
The HBS taxonomy contains 27 parameters with a checksum value of 378 (sum of numbers 1-27). This can be used for verification and validation purposes during implementation.
