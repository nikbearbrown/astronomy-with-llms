# Images Brief: Chapter 19 — Celestial Distances

Visual requirements and design notes for illustrations supporting the Attenborough × Feynman v1.1 chapter on measuring celestial distances.

---

## Figure 1: Parallax Principle — Two Eyes to Two Observations

**Purpose:** Teach the parallax concept via human depth perception before scaling to astronomy.

**What to show:**
- Left panel: A face with two eyes separated by a few centimeters, viewing a pen held at arm's length.
- Middle panel: Same setup, pen now moved to the side (arm's length away). Show the apparent shift of the pen relative to a background (bookshelf, house frame).
- Right panel: Same pen, now held much farther away (across the room). Show a smaller apparent shift.

**Annotations:**
- Label the eye separation as "baseline."
- Label the apparent shift angle as "parallax."
- Arrow from the pen showing: *farther away = smaller shift*.
- Add: "Your brain uses this shift to judge distance to anything within ~30 meters."

**Caption:**
Parallax is how your eyes judge distance. Two viewing points separated by a baseline (your eye separation) produce an apparent shift in the object's position against a background. The farther the object, the smaller the shift. Astronomers use the same principle, with Earth's orbit as the baseline.

**What the student should notice:** The geometric relationship between baseline, distance, and angle. The principle scales to any baseline and any distance.

---

## Figure 2: Earth's Orbital Baseline for Stellar Parallax

**Purpose:** Show how Earth's annual motion provides the baseline for measuring stellar distances.

**What to show:**
- A circle (the Sun) at the center.
- Earth's orbit around it.
- Two positions of Earth: June (left) and December (right), separated by the orbital diameter (2 AU).
- A nearby star (exaggerated for visibility) in the foreground.
- A background of very distant stars (represented as small dots).
- Dashed lines from Earth's June and December positions to the nearby star, forming a triangle.
- Dashed lines from both Earth positions to a distant background star (should be nearly parallel, showing no shift).

**Annotations:**
- Label the baseline: "2 AU" (or "~300 million km").
- Label the angle at the star (formed by the two sight lines): "2 × parallax (p)."
- Label the parallax: "p = half of this angle."
- Show with an arrow: the nearby star's position relative to background stars shifts between June and December.
- Nearby star relative to distant background: "June position" and "December position," with a small angle between.

**Caption:**
As Earth orbits the Sun, nearby stars appear to shift position against the background of distant stars. The baseline is the diameter of Earth's orbit (2 AU, about 300 million km). The angle of shift depends on the star's distance. For the nearest star (Proxima Centauri), the total shift is only 1.5 arcseconds — less than 1/2400th of a degree.

**What the student should notice:** The enormous baseline (2 AU) still produces a tiny angle. This is why parallax requires precision instruments. The relationship between angle, baseline, and distance is the key to all distance measurement.

---

## Figure 3: The Parallax Ruler — Distance vs. Parallax Angle

**Purpose:** Show the inverse relationship between distance and parallax angle.

**What to show:**
- A horizontal axis labeled "Distance (light-years)" with tick marks at 0, 10, 50, 100, 500, 1000.
- A vertical axis labeled "Parallax Angle (arcseconds)" with tick marks at 0.01, 0.05, 0.1, 0.5, 1.0.
- A hyperbolic curve (inverse relationship) showing the relationship D = 206,265 AU / p.
- Annotate specific points:
  - Proxima Centauri: 4.25 light-years, parallax 0.76 arcseconds.
  - Bessel's 61 Cygni: 10.4 light-years, parallax 0.314 arcseconds.
  - A faint star at 30 light-years, parallax 0.11 arcseconds.
  - A point labeled "Hipparcos limit (~300 light-years)" with a parallax of ~0.011 arcseconds.
  - A point labeled "Gaia limit (~30,000 light-years)" with a parallax of ~0.0001 arcseconds.

**Annotations:**
- Shade the region "Ground telescopes (Hipparcos limit)" and "Space telescopes (Gaia)."
- Add note: "Smaller angle = farther distance. The relationship is inverse: D = 1/p."

**Caption:**
The parallax-distance relationship. Larger parallax angles correspond to nearby stars; tiny angles correspond to distant stars. Ground-based telescopes can measure angles down to about 0.001 arcseconds (Hipparcos), reaching 300 light-years. Space telescopes like Gaia can measure angles as small as 0.00005 arcseconds (50 microarcseconds), reaching 30,000 light-years.

**What the student should notice:** The geometric boundary where parallax becomes unmeasurable. Why space telescopes are necessary to extend distance measurement. The practical limits of precision.

---

## Figure 4: Variable Star Light Curve — Cepheid Example

**Purpose:** Show how variability is measured and linked to distance.

**What to show:**
- A graph with time on the x-axis (horizontal, in days, spanning 5–10 days for a typical Cepheid period).
- Brightness (apparent magnitude or relative brightness) on the y-axis.
- A smooth sinusoidal-like curve showing the star rising to maximum brightness, then falling more slowly to minimum, repeating.
- Annotate:
  - "Maximum brightness" at the peak.
  - "Minimum brightness" at the trough.
  - "Period" spanning one full cycle (e.g., 5.4 days for Delta Cephei).

**Include a callout box:**
"The period-luminosity relation:
Longer periods = intrinsically brighter stars.
Period tells you luminosity.
Luminosity + apparent brightness = distance."

**Caption:**
A Cepheid variable star's light curve. The star expands and contracts, brightening and dimming regularly. The period (time for one cycle) is easy to measure. The period-luminosity relation, discovered by Henrietta Leavitt in 1908, shows that the period is directly related to the star's intrinsic brightness — longer-period Cepheids are intrinsically brighter. By measuring the period and comparing intrinsic brightness to apparent brightness, astronomers can calculate distance.

**What the student should notice:** The regularity of the variation. The connection between period (observable) and luminosity (physical property). How observation leads to inference of distance.

---

## Figure 5: The Cosmic Distance Ladder

**Purpose:** Show how each distance method builds on the one below it.

**What to show:**
- A literal ladder (or stepped structure) with rungs labeled from bottom to top:
  1. **Foundation: Trigonometric Parallax** (nearest stars, 0–30,000 light-years with Gaia; ~60 light-years with ground telescopes).
  2. **Rung 2: Cepheid Variables** (nearby galaxies, up to ~60 million light-years).
  3. **Rung 3: RR Lyrae Variables** (older stellar populations, up to ~300,000 light-years).
  4. **Rung 4: Type Ia Supernovae** (distant galaxies, up to ~5 billion light-years).
  5. **Top: Hubble Constant** (cosmological distances, expansion rate of the universe).

**Annotations:**
- Next to each rung, show the method and its reach: "Parallax: 30,000 ly," "Cepheids: 60 Mly," etc.
- Show arrows or lines connecting each rung to the one above it, with labels like "Calibrated against" to show the dependency.
- Highlight: "Each rung is calibrated using objects of known distance from the rung below."

**Callout box at the side:**
"Why the ladder works:
1. Parallax measures nearby stars directly (no assumptions).
2. Cepheids in those nearby stars define the period-luminosity relation.
3. Distant Cepheids use this relation to find distance.
4. Type Ia supernovae in galaxies with known Cepheid distances are calibrated.
5. Distant supernovae measure galaxies billions of light-years away."

**Caption:**
The cosmic distance ladder. Each method of measuring distance builds on the one below it. Parallax (geometry) is the foundation. Variable stars are calibrated against parallax. Supernovae are calibrated against variable stars. The entire structure rests on parallax being correct.

**What the student should notice:** The hierarchical structure. Why precision in parallax matters for all distant distance measurements. The interconnectedness of astronomical methods.

---

## Figure 6: Scale Oscillation — From Eyes to Gaia

**Purpose:** Illustrate the progression of scale from human perception to space-based measurement.

**What to show:**
- A series of paired illustrations, growing in scale:
  1. Two human eyes (centimeters apart), viewing a pen at arm's length. Parallax shift: large and obvious.
  2. Earth's two positions (June/December, AU apart), viewing a nearby star. Parallax shift: 0.76 arcseconds (Proxima Centauri).
  3. Ground telescope (Hipparcos-like), measuring stars at 60–300 light-years. Parallax shift: ~0.01 arcseconds.
  4. Space telescope (Gaia), measuring stars at 30,000 light-years. Parallax shift: ~0.0001 arcseconds.

**Annotations:**
- For each level, label the baseline (eye separation, AU, telescope aperture, satellite orbital precision).
- For each level, label the angular precision achieved.
- For each level, label the maximum distance reachable.

**Caption:**
From human depth perception to cosmic distance measurement, the principle scales: baseline + angular precision = distance. Your eyes have a baseline of a few centimeters and can judge distance to ~30 meters. Earth's orbit (300 million km baseline) and precise angle measurement allow us to measure distances to the nearest stars. Space telescopes with microarcsecond precision reach across the galaxy.

**What the student should notice:** The fractal-like repetition of the same geometric principle at vastly different scales. Why precision matters — each improvement in angle measurement extends the reachable distance.

---

## Figure 7: The Hubble Tension

**Purpose:** Show the discrepancy between two methods of measuring the cosmic expansion rate.

**What to show:**
- A plot with "Measurement Method" on the x-axis and "Hubble Constant (km/s/Mpc)" on the y-axis.
- Two bars (or measurements with error bars):
  1. "Distance Ladder (Parallax + Cepheids + Type Ia Supernovae)" at ~73 km/s/Mpc, with error bars showing ±1.5.
  2. "Cosmic Microwave Background (Planck satellite)" at ~67 km/s/Mpc, with error bars showing ±0.5.
- A gap between the two bars, labeled "Hubble Tension (~9% discrepancy)."
- A horizontal dashed line at the average or midpoint, labeled "Predicted value if all methods agree."

**Annotations:**
- Note: "Error bars are small enough that the disagreement is statistically significant."
- Add a question mark or alert symbol near the gap.

**Caption:**
The Hubble tension. Two independent measurements of the universe's expansion rate disagree. The distance ladder (parallax calibrated through Cepheids and Type Ia supernovae) gives ~73 km/s/Mpc. The cosmic microwave background gives ~67 km/s/Mpc. The discrepancy is about 9% and statistically significant, suggesting either systematic error in one method or physics not yet understood.

**What the student should notice:** That measurement discrepancies can reveal new physics or hidden errors. That astronomical methods are constantly being checked against each other. That precision is double-edged — it reveals small discrepancies that were hidden before.

---

## Design Principles

- **Clarity over realism:** Illustrations should be schematic, emphasizing the concept over photorealistic detail. For example, star positions can be exaggerated for visibility.
- **Labels and annotations:** Every figure should be self-explanatory. A student should be able to understand the core idea from the illustration and caption alone.
- **Color:** Use contrasting colors (e.g., bright star against dark background, different colors for Earth's two positions, color-coded rungs of the distance ladder).
- **Figures serve the text:** Each figure is referenced in the chapter narrative and corresponds to a specific concept or mechanism.

---

## Integration Notes

- **Figure 1** appears in Concept 1 (Parallax principle).
- **Figure 2** appears in Concept 1 (Earth's baseline).
- **Figure 3** appears in Concept 1 (Parallax-distance relationship, connects to space missions in Concept 2).
- **Figure 4** appears in Concept 2 (Variable stars and period-luminosity).
- **Figure 5** appears in Synthesis (Cosmic distance ladder).
- **Figure 6** appears in Synthesis or Connections Forward (scale oscillation, moral weight).
- **Figure 7** appears in Connections Forward or Chapter Summary (Hubble tension, open questions).

