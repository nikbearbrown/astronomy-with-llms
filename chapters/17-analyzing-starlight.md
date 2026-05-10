# Analyzing Starlight

**TL;DR:** A star's spectrum is a fingerprint written in light. Temperature dominates which lines appear; pressure and motion reveal the rest. Through the OBAFGKM sequence, we read the universe's chemical biography.

---

## Chapter opening

Imagine standing in a darkened observatory, the dome open to the winter sky. Your eye meets Sirius — the Dog Star, burning white in Canis Major, brighter than any other star visible from Earth. It looks simple: a point of light. You might think everything interesting about it is exhausted in that brightness, that color.

You are wrong.

The light from that star has traveled 8.6 light-years through vacuum. It carries, compressed into those photons, a message about the star's temperature, its composition, the metals it holds, the forces at work in its surface layers, whether it is moving toward you or away, how fast it spins. A spectrograph — a prism that spreads that light into its component wavelengths — reveals the message. What you see is a continuous band of color, crossed by thin dark lines. Those lines are not in the starlight itself. They are absences. Atoms in the star's outer atmosphere have plucked specific colors out of the beam, the way a traffic signal removes all wavelengths except red. Every element leaves its mark at precise wavelengths. Read the pattern of marks, and you can reconstruct what the star is made of, how hot it burns, what its surface pressure is, whether it is a giant or a dwarf.

This is the real work of observational astronomy: not gazing at starlight, but decoding it.

### Learning Objectives

By the end of this chapter, you will understand:

- How to measure a star's brightness and what those measurements tell you about distance and luminosity
- Why a star's color reveals its surface temperature, and how the OBAFGKM spectral sequence organizes stars by that temperature
- How spectral lines work: which elements produce which lines, and why temperature determines which ones dominate a spectrum
- What line widths, line shifts, and line broadening reveal about pressure, motion, and rotation
- Why the composition of most stars is similar — mostly hydrogen and helium, with heavier elements as traces — and what those traces tell us about cosmic history

### Prerequisites

You should already understand:
- The electromagnetic spectrum and photon energy
- How atoms absorb and emit light at specific wavelengths
- The inverse-square law for light (brightness decreases with the square of distance)
- Wien's law (hotter objects emit peak wavelength at shorter wavelengths)

---

## Concept 1: Measuring Light — Brightness, Distance, and the Magnitude Scale

### The puzzle

In the night sky, some stars look brighter than others. But brightness is a lie. Sirius looks brighter than Polaris not because it gives off more energy, but because it sits 26 light-years away while Polaris sits 430 light-years away. A dim bulb at arm's length outshines a searchlight miles away. We need a way to separate what we see from what actually is.

Astronomers had to invent two different words for this problem. **Luminosity** is the total power output of the star — the amount of energy it radiates in all directions every second, measured in watts. **Apparent brightness** is the amount of that energy that happens to reach Earth. The first is intrinsic. The second is an accident of geography.

To a star, space is egalitarian. It radiates equally in every direction. Imagine the star as a point, and draw a sphere of radius *r* around it. The star's total luminosity is spread over the surface area of that sphere: 4π*r*². When Earth is twice as far away, that sphere has four times the area. The same luminosity is now spread thinner. Receive one quarter the light.

This is not a coincidence or an approximation. This is geometry.

### The mechanism: The inverse-square law in practice

Here is the key trade-off that astronomers had to accept early on: **we can measure apparent brightness easily, but we cannot know luminosity without knowing distance.** Look at the night sky with a telescope and measure how much light hits your detector from a faint star. Call that measurement *b*. Now look at a brighter star. Call its brightness *B*. You can say with certainty that *B* > *b*. But you cannot say whether the bright star is intrinsically luminous or simply close, or whether the faint star is intrinsically dim or simply far away. Both luminosity and distance are hidden inside that brightness measurement. To extract either one, you need the other.

This problem haunted astronomy for centuries. The solution, when it came, had two parts. First, use other methods to measure distance — parallax, Cepheid variables, the cosmic distance ladder. We will return to those. Second, develop a system to describe apparent brightness that is sensitive enough to capture real differences while being standard enough for comparison.

The system that emerged is the **magnitude scale** — one of those accidents of history that stuck.

In 150 BCE, Hipparchus of Rhodes, standing on the island in the Mediterranean, looked at the night sky and sorted the stars into six categories by eye: the brightest he called *first-magnitude*, the dimmest visible to the eye *sixth-magnitude*. This was not science; it was taxonomy by squinting. It persisted because it worked. Bright stars really are orders of magnitude brighter than faint ones, and the human eye is good at relative brightness.

By the 19th century, astronomers had precision photometers, and they asked: what is the actual ratio between first and sixth magnitude stars? The measurement came back: roughly 100 to 1. A first-magnitude star sends us one hundred times more light than a sixth-magnitude star.

That number — 100 — is arbitrary but historically locked in. Given that a difference of five magnitudes corresponds to a brightness ratio of 100:1, what number, multiplied by itself five times, gives 100? The fifth root of 100, which is approximately 2.51. So each step of magnitude — moving from magnitude 6 to magnitude 5, or from 2 to 1 — corresponds to a brightness increase by a factor of roughly 2.51.

This is the trade-off: **clarity for counterintuitiveness.** The scale works because historical convention locked it in place. It is harder to use than a linear scale. You cannot simply add magnitudes. But it captures the logarithmic way the human eye perceives brightness, and it has been in continuous use for over 2,000 years. Any astronomer can instantly know what "a first-magnitude star" means. That consensus is valuable.

The scale also goes backward. A larger magnitude means a fainter object. The brightest star in the sky, Sirius, has magnitude −1.5. Venus at its brightest is −4.4. The Sun is −26.8. The faintest objects detected by the Hubble Space Telescope hover near magnitude 30. Backward, yes. Counterintuitive, absolutely. Still in use everywhere.

### Worked example: Calculating brightness ratios

An astronomer wants to know how much brighter Sirius is than a typical third-magnitude star. Sirius is magnitude −1.5; call that star magnitude 3.0. The difference is −1.5 − 3.0 = −4.5 magnitudes.

Using the relationship that each magnitude step is a factor of 2.51, a difference of 4.5 steps is 2.51^4.5 ≈ 100. So Sirius sends roughly 100 times more light to Earth than that third-magnitude star.

But wait — that tells us about apparent brightness. To know whether Sirius is intrinsically brighter, we need distance. And here the second part of the solution arrives: once we know distances (through parallax or other methods), we can calculate **absolute magnitude** — the magnitude the star would have if placed at a standard distance of 10 parsecs. That number is intrinsic. It reflects real luminosity differences.

### Common misconceptions

**"A dimmer star has a higher magnitude because it's farther away."** No. Magnitude measures brightness as we see it from Earth. Whether that brightness comes from a faint nearby star or a luminous distant one is hidden in the magnitude alone. Distance requires separate measurement.

**"The magnitude scale is logarithmic, so magnitudes don't add."** Correct, and that's why we use the formula m₁ − m₂ = 2.5 log(*b₂*/*b₁*). But this is not a bug; it's a feature. The scale reflects how our eyes work.

---

## Concept 2: Temperature Reads Color — Wien's Law and Spectral Classification

### The puzzle

Walk into the Sagittarius Star Cloud and you see red stars, orange stars, yellow stars, white stars, blue stars. They are not random. The colors form a sequence. The bluest stars are the hottest. The reddest are the coolest. This is not a trick of Earth's atmosphere. A star's color reveals its surface temperature.

Why? Because hot objects emit most of their light at short wavelengths, and cool objects emit most of their light at long wavelengths. Wien's law makes this precise: the peak wavelength is inversely proportional to temperature. A 30,000 K star peaks in the ultraviolet; most of its visible light is blue. A 3,000 K star peaks in the infrared; most of its visible light is red. In between sit yellow stars, like our Sun, at about 5,800 K.

But we need a second piece: a way to assign that color to a precise temperature. Astronomers use **color indices** — the difference in brightness through two different colored filters.

### The mechanism: Color indices as a thermometer

A spectrograph spreads light into a rainbow. But a telescope with colored filters can work too, and it is faster. You put a blue filter in front of the detector. You measure the brightness of the star in blue light only. Call that magnitude *B*. Then you put a visual filter (yellow-green) in front. Call that magnitude *V*. The difference *B* − *V* is the **color index**.

The key insight: this number is independent of distance. A red star looks red whether it is nearby or far away. The ratio of its brightness in blue to its brightness in visual light is a property of the star itself, not the distance. But the color index depends on temperature, and temperature alone.

By convention, the color index of a 10,000 K star (like Vega) is set to zero. A hotter star, which emits more blue light relative to visual light, has a negative *B* − *V*. A cooler star has a positive *B* − *V*. Blue stars range from about −0.4 (40,000 K) to red stars at +2.0 (2,000 K).

This is elegant trade-off: **accuracy for simplicity.** You do not need to resolve the spectrum into thousands of wavelengths. You measure the star's brightness through two filters. From one number — the color index — you infer surface temperature to within a few hundred Kelvin. This is how most stellar temperatures are determined in practice.

### Worked example: Using color to find temperature

You observe a star and measure its *B* magnitude as 5.5 and its *V* magnitude as 5.0. The color index is 5.5 − 5.0 = +0.5. Looking up the color-temperature relationship: a *B* − *V* of +0.5 corresponds to a star with surface temperature around 5,700 K. (The Sun's *B* − *V* is about 0.65, corresponding to 5,800 K.) This star is roughly as hot as the Sun, perhaps slightly hotter.

### Common misconceptions

**"A red star must be cool."** True. **"Therefore, a red star is faint."** Not necessarily. A cool star can be luminous if it is giant-sized. Betelgeuse is a red supergiant — cool on the surface but radiating enormous total power because its surface area is immense.

**"Color depends on distance because distant stars look dimmer."** No. Color depends on temperature. Dimness depends on distance and luminosity. The two are independent. A red star looks red whether it is 10 light-years or 10,000 light-years away.

---

## Concept 3: Spectral Lines and Temperature — Why OBAFGKM Works

### The puzzle

In 1814, Joseph Fraunhofer aimed a prism at the Sun and saw a continuous rainbow crossed by hundreds of thin dark lines. In the 1860s, William and Margaret Huggins took spectra of stars and found the same pattern: dark lines superimposed on a rainbow. They realized — through laboratory work with heated elements — that each element produced absorption lines at specific wavelengths.

Here was a tool of unprecedented power: a way to read the chemical composition of distant stars. But the patterns were bewildering. Different stars had different lines. The first astronomers to study stellar spectra thought this meant different stars were made of different elements. They were wrong. Almost all stars have the same composition: roughly three-quarters hydrogen, nearly a quarter helium, and 1% or less of everything else. The difference is not composition. The difference is temperature.

### The mechanism: How temperature determines which lines dominate

This is the key to reading stellar spectra, and it is not obvious.

Hydrogen, the most abundant element in the universe, does not always show strong absorption lines. In a very hot star — say, 40,000 K — the hydrogen atoms are completely ionized. An ionized atom has lost its electrons. With no electrons orbiting, there are no electrons to jump between energy levels, and thus no absorption lines. Ionized hydrogen produces nothing.

In a very cool star — say, 2,000 K — hydrogen atoms still have their electrons. But the electrons sit almost exclusively in the ground state, the lowest energy level. To absorb light, an electron must jump to a higher level. The only photons energetic enough to make this jump are ultraviolet photons. A cool star emits very little ultraviolet light. Most of its radiation is in the visible and infrared. Result: essentially no visible hydrogen lines.

In a warm star — around 10,000 K — hydrogen atoms are neutral and excited. Enough thermal energy pumps a significant fraction of electrons into the second energy level. These electrons can now absorb visible photons (the Balmer lines, corresponding to jumps from the second level to higher levels). The result: strong, prominent hydrogen absorption lines.

Every element, in every ionization state, has a characteristic temperature at which it produces the strongest absorption lines. Helium ionized once (He+) peaks in the 20,000-30,000 K range. Calcium ionized once (Ca+) peaks around 6,000-7,500 K. Titanium oxide (a molecule) becomes abundant only below 3,500 K. These are not arbitrary. They reflect the ionization energy of the atom and the thermal energy available at that temperature.

This is the deep trade-off: **simplicity for detail.** A star's spectrum is dominated by the element whose ionization temperature matches the star's surface temperature. By reading which lines are strong, we learn the star's temperature. We sacrifice the ability to say precisely how much iron is present, but we gain a thermometer that is cheap, fast, and works from the ground.

In the 1890s, Annie Jump Cannon compiled a system to organize this chaos. She kept just seven letters from an earlier alphabetical system: O, B, A, F, G, K, M, arranged in order of decreasing temperature. (The remaining letters were discarded for historical reasons — another accident of convention.) She added a mnemonic to help students remember: "Oh Be A Fine Girl, Kiss Me." Updated for diversity: "Oh Be A Fine Guy/Girl, Kiss Me." With the discovery of brown dwarfs and ultra-cool objects, the sequence has expanded: L, T, Y.

Each letter is subdivided into ten subtypes, 0–9. A B0 star is the hottest B star; a B9 is the coolest B star and barely hotter than an A0 star. Our Sun is G2.

Here is the Harvard spectral sequence, with representative examples:

**O**: 30,000+ K, blue. Ionized helium, weak hydrogen. Example: 10 Lacertae.

**B**: 10,000–30,000 K, blue-white. Neutral helium, strong hydrogen. Examples: Rigel, Spica.

**A**: 7,500–10,000 K, white. Strongest hydrogen, weak ionized metals. Examples: Sirius, Vega.

**F**: 6,000–7,500 K, yellow-white. Strong hydrogen, strong ionized calcium, many metal lines. Examples: Canopus, Procyon.

**G**: 5,200–6,000 K, yellow. Weak hydrogen, strong ionized calcium, strong sodium. Examples: Sun, Capella.

**K**: 3,700–5,200 K, orange. Very weak hydrogen, ionized calcium, sodium, many neutral metals. Examples: Arcturus, Aldebaran.

**M**: 2,400–3,700 K, red. Neutral metals and molecular bands dominate; titanium oxide strong. Examples: Betelgeuse, Antares.

### Worked example: Reading a spectrum

You observe a star's spectrum. Hydrogen lines are present but weak. Ionized calcium lines are strong. Sodium lines are present. Comparing to the reference spectra: this pattern matches the G or K types. If the ionized metals are stronger and hydrogen very weak, it is likely K. If ionized metals are strong but hydrogen still visible, likely G. Measure the color index to break the tie. A *B* − *V* of +0.5 points to G. A *B* − *V* of +1.2 points to K.

Annie Jump Cannon did this by eye, looking at photographic plates under a microscope, classifying up to three stars per minute. She classified around 500,000 stars in her lifetime — a monument to both her skill and the repetitive labor that astronomy once demanded of its practitioners, particularly its women.

### Common misconceptions

**"If a star has hydrogen lines, it contains hydrogen."** Correct, but misleading. Almost all stars contain hydrogen — it is the dominant element. The presence of hydrogen lines tells you about temperature, not composition. The absence of hydrogen lines does NOT mean the star lacks hydrogen. It means the temperature is wrong for hydrogen to absorb visible light.

**"Spectral type directly tells you how bright a star is."** No. Two stars with the same spectral type can differ wildly in luminosity. A red dwarf (spectral type M) and a red supergiant (also spectral type M) both have similar surface temperatures, but the giant is millions of times more luminous because it is gigantic.

---

## Concept 4: What Spectra Reveal Beyond Temperature — Size, Motion, Rotation, Composition

### The puzzle

Temperature dominates the spectrum, but it is not the only story. Line widths can reveal a star's size. Doppler shifts reveal motion. Line broadening reveals rotation. And with careful analysis, the relative strengths of different lines tell you the star's elemental abundances.

### The mechanism: Four types of information read from spectral lines

#### 1. **Line widths and stellar size**

A giant star has a large, extended photosphere. Because the same amount of material is spread over a huge volume, the density is low. Low density means fewer collisions between atoms. Few collisions mean narrow spectral lines.

A dwarf star is smaller, denser. More collisions. Broad spectral lines.

This is the trade-off: **extended atmospheres for line broadness.** A giant and a dwarf with identical surface temperature will have identical line positions and identical colors — they look the same temperature. But the shapes of their lines are different. A careful study of line width can distinguish a giant from a dwarf even without knowing distance. This is how we separate luminosity classes.

#### 2. **Doppler shift and radial velocity**

A star moving toward us compresses the wavelengths it emits. The absorbed light shifts toward the blue. A star moving away stretches the wavelengths. The absorbed light shifts toward the red.

In 1868, William Huggins observed the spectrum of Sirius and saw its hydrogen lines shifted. He concluded the star was moving toward Earth. (Later, more precise measurements showed it was actually moving away, but Huggins pioneered the technique.)

The magnitude of the shift tells the velocity. A shift of 0.1 nm in the Balmer-alpha line (at 656 nm) corresponds to motion at several tens of kilometers per second. This is **radial velocity** — motion along our line of sight. Combined with proper motion (the star's movement across the sky, measured in arcseconds per year), radial velocity gives the complete space velocity.

#### 3. **Line broadening and rotation**

Imagine a star rotating. One edge rotates toward us, the other edge rotates away. Light from the approaching edge is blue-shifted. Light from the receding edge is red-shifted. The light from the star's center is neither.

A non-rotating star has a sharp absorption line. A rotating star produces a smeared, broadened line — the superposition of all those Doppler shifts from different parts of the star's surface.

The faster the rotation, the broader the line. Some stars, like Vega, rotate so fast (one rotation every 12.5 hours) that they are distorted — flattened at the equator like an oblate spheroid, 23% wider at the equator than at the poles.

The Sun rotates slowly, with a period of about a month. Young stars rotate rapidly, sometimes with periods of only hours. As stars age, they lose angular momentum through magnetic braking and slow down.

#### 4. **Line strength and elemental abundance**

Suppose two stars have identical temperatures and pressures, but lines of sodium are stronger in one star than the other. Stronger lines mean more atoms absorbing light. That star contains more sodium.

This is the principle of abundance analysis: the strength of an absorption line is proportional to the number of atoms producing it. By calculating how many atoms must be present to produce the observed line strength, we can determine the elemental abundances.

The universe is not equally mixed. Hydrogen makes up roughly 73% of the mass of a typical star. Helium about 25%. Everything else — all the carbon, nitrogen, oxygen, iron, silicon, nickel, all the elements that make planets and people — constitutes 1% or less.

Yet this 1% carries history. A star with 2% "metals" (the astronomical term for all elements heavier than helium) is richer in heavy elements than a star with 0.2%. Where do those heavy elements come from? From previous generations of stars that fused lighter elements into heavier ones and exploded, scattering those elements into the interstellar medium.

Read the abundances of old stars, and you read the chemical history of the galaxy. Young stars have more heavy elements than old stars because the galaxy has been enriching itself with heavy elements over time. This is how we know the universe has a history.

### Worked example: Combining multiple pieces of information

You observe a G-type star. Its spectral lines are sharp and narrow — suggesting a dwarf, not a giant. Its hydrogen lines show a Doppler shift of 20 nm toward the blue — it is moving toward us at about 10 km/s. The lines are slightly broadened, suggesting a rotation period of several days. Iron lines are 10 times stronger than in the Sun, suggesting a metal abundance of 10 times solar.

This is a young, metal-rich, nearby dwarf moving toward us. It is probably a member of a young stellar cluster or association, enriched in metals by repeated star formation and supernovae in its neighborhood.

### Common misconceptions

**"A strong line means the element is abundant."** Only if temperature and pressure are the same. The same element in a hot star might show weak lines while it dominates in a cool star, because temperature determines ionization.

**"Doppler shift tells you distance."** No. It tells you motion along the line of sight. Distance requires parallax, main-sequence fitting, or other independent measurements.

---

## Integration: The Universe's Chemical Biography

We can now see the full picture. Stars are not all the same. They differ in temperature, size, rotation, motion, and composition. But they are cousins, not strangers.

Most stars are mostly hydrogen and helium — the elements created in the Big Bang. The heavy elements, from carbon to iron and beyond, were forged in the cores of massive stars and scattered into space when those stars exploded. A star with 2% heavy elements is enriched by at least two generations of stellar nucleosynthesis. A star with 0.2% heavy elements was probably born early in the galaxy's history, before many previous stars had finished their work of creation.

You are made of carbon, oxygen, nitrogen, calcium, iron. Every atom of these elements in your body was manufactured in a star's core, ejected in a supernova, mixed with interstellar gas, incorporated into a new star-forming cloud, and eventually built into the solar system. The spectroscopic analysis of starlight is how we trace that history backward, element by element, abundance by abundance.

The OBAFGKM sequence is not a collection of arbitrary pigeonholes. It is a thermometer. The strength and shape of spectral lines are a pressure gauge. Doppler shifts are a motion detector. Line broadenings are a rotation counter. Together, they are a complete diagnostic tool. Point a spectrograph at a distant star, and you can read:

- Its surface temperature (to within a few hundred Kelvin)
- Its size, whether dwarf or giant (from line width)
- Its motion, how fast and in what direction (from Doppler shift)
- Its rotation rate (from line broadening)
- The elemental abundance of most known elements (from line strength, with careful calculation)

And from those facts, you can infer luminosity, mass, age, and evolutionary state. A star's spectrum is its biography written in light.

---

## Exercises

### Warm-up

1. **Magnitude reversal.** Sirius has magnitude −1.5. Polaris has magnitude 2.0. How many magnitudes apart are they? Which is brighter? By what factor?

2. **Color and temperature.** A star has *B* − *V* = −0.2. Is it hotter or cooler than the Sun (which has *B* − *V* ≈ 0.65)? Roughly what temperature range?

3. **Spectral type logic.** You see a spectrum with strong hydrogen lines and neutral helium lines. What spectral type is it? (Refer to the sequence in Concept 3.)

### Application

4. **Reading the lines.** A star shows a prominent sodium line at 589.3 nm in the laboratory frame. In your observation, you measure it at 589.8 nm. Is the star moving toward you or away from you? Roughly how fast?

5. **Combining clues.** A star has spectral type K, narrow spectral lines, and no detectable Doppler shift. What can you infer about its size, luminosity, and motion through space?

6. **Abundance story.** Star A has a metal abundance of 3% (three times solar). Star B has a metal abundance of 0.5% (half solar). Which star was probably born first? Why?

### Synthesis

7. **Historical context.** Annie Jump Cannon classified around 500,000 stars by eye, at a rate of up to 3 per minute. How many hours of work did this represent? (Hint: 500,000 stars ÷ 3 per minute = total minutes; convert to hours.) What does this tell you about the nature of astronomical labor in the early 20th century, and why such work was deemed acceptable to assign to women but not men?

8. **Integration challenge.** You are given a star's spectrum. You measure:
   - Spectral type: A0
   - Line widths: narrow
   - Doppler shift of hydrogen line: 0.5 nm toward red
   - Iron line strength: 20× solar

   Describe this star in plain language. What is its temperature? Is it a giant or dwarf? Is it moving toward or away from us? What can you say about its chemical history?

---

## Summary

A star's light carries the imprint of its properties. Apparent brightness and magnitudes tell us how the star looks from Earth, though they conflate luminosity and distance. Color and spectral type reveal surface temperature — temperature alone determines which elements show strong absorption lines. Line widths distinguish giants from dwarfs; Doppler shifts reveal motion; line broadening reveals rotation; line strength reveals composition. Through spectroscopy, a distant point of light becomes a three-dimensional object with a history. The OBAFGKM sequence was a historical accident, a way to organize the chaos of stellar spectra by eye. It persists because it works. It is a thermometer, and the thermometer has never stopped working.

The chemical composition of stars tells us that the universe has a biography. Young stars contain heavier elements produced by older stars. We are made of star stuff — specifically, of elements forged in the cores of previous stars and scattered by their explosions into the interstellar medium. When you read starlight, you are reading the history of element creation, preserved in light.

---

## What would change my mind

If spectroscopic analysis could be shown to systematically misidentify stellar temperatures — that is, if stars classified as O-type showed surface behaviors inconsistent with 30,000+ K — I would need to reconsider the foundations of spectral classification. But decades of multiwavelength observations, direct temperature measurements from other methods, and the successful use of spectral type to predict stellar properties has locked this in firmly.

## Still puzzling

I do not fully understand why the human eye's perception of brightness maps so cleanly onto the logarithmic magnitude scale, or whether this is a deep property of perception or a fortunate coincidence that persists because it became standardized so early.

---

**Tags:** #spectroscopy #stellar-classification #OBAFGKM #Annie-Jump-Cannon #Doppler-shift #stellar-composition #hydrogen-lines #cosmic-chemistry #observational-astronomy

**Byline:** Nik Bear Brown

**Word count:** 5,240
