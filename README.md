# Color Priority in Interface Design

[Live Demo](https://denn1s.github.io/color-priority/)

---

## What is Color Priority?

In any UI, color does more than decorate — it communicates. Every color you choose for a component implicitly tells the user how important that component is relative to everything else on the screen. This is color priority: the intentional assignment of visual weight to interface elements so that the user's eye travels in the order you intend.

Not all colors carry equal weight. A saturated, high-contrast color demands attention. A muted, low-contrast color recedes. The hierarchy between them determines whether a user immediately finds the action you want them to take, or gets lost scanning a visually flat — or visually chaotic — screen.

Getting color priority right means your backgrounds stay quiet, your content is readable without shouting, and your call-to-action is the loudest thing on the page — because it should be.

---

## The Six Color Roles

Well-structured interfaces tend to use color in six distinct roles, each with an expected place in the visual hierarchy.

### Surface (Priority 1)
The canvas. This is the base layer that everything else sits on top of. It should be the quietest color in the entire system — typically a neutral, low-saturation tone. If your surface color draws the eye, it will compete with every element placed on it. The surface should feel invisible.

### Surface Alt (Priority 1)
Secondary containers: navigation bars, sidebars, cards, modals. Still quiet, but distinct enough from the main surface to create spatial separation. Surface Alt and Surface share the same priority level because neither is meant to attract attention — they only need to differentiate themselves from each other to establish layout structure.

### Feedback (Priority 2)
Success states, error messages, warnings, loading indicators. Feedback colors need enough contrast to be noticed when they appear, but they are contextual and temporary. They should not compete with the CTA when both are visible. A common mistake is making feedback colors too loud permanently, when their job is to appear, communicate, and get out of the way.

### Content (Priority 3)
Body text, headings, labels, icons that carry meaning. Content must be readable — high enough contrast against its background to meet accessibility standards — but it should not attract attention beyond what the words themselves carry. Text that feels visually aggressive pulls focus away from the interactive elements the user should be acting on.

### Interactive (Priority 4)
Buttons, links, form controls, toggles. These elements should draw the eye and signal affordance clearly. They are more visually prominent than content, but they must not outshine the primary call-to-action. If your secondary buttons and links are visually louder than your CTA, the user will not know where to act first.

### Accent / CTA (Priority 5)
The loudest element in the system. This is the call-to-action, the brand highlight, the one thing on the screen that should win every visual competition. There should typically be only one true CTA color, applied sparingly. If everything uses your accent color, nothing is accented.

---

## Common Mistakes

**Loud backgrounds.** Using a saturated or dark color for the surface makes every element placed on it fight for contrast. The background becomes a design statement instead of a foundation, and the hierarchy collapses before it starts.

**A CTA that blends in.** If your call-to-action color is similar in lightness and saturation to your interactive or content colors, users will not instinctively know where to click. The CTA should win on sight — not require scanning.

**Flat priority — everything at the same level.** When all six roles use colors of similar visual weight, the result is an interface with no entry point. The eye does not know where to start. This is one of the most common outcomes when colors are chosen aesthetically rather than functionally.

**Interactive louder than CTA.** Secondary buttons, links, and form controls that are more saturated or higher-contrast than the primary action create a hierarchy inversion. The user's eye lands on the wrong element first.

**Overusing the accent color.** When the accent appears on headings, icons, borders, and backgrounds in addition to the CTA, it stops being an accent. Reserve it. The rarer it appears, the more it commands attention when it does.

---

## How to Use the Tool

The interactive tool presents a skeleton wireframe representing a generic UI layout — a navigation bar, a content area, a card, a form, and a primary action button. Each region corresponds to one of the six color roles above.

For each role, you can:
- Select a color using the color picker
- Assign a priority level from 1 (quietest) to 5 (loudest)

The wireframe updates live as you make changes. The goal is not to produce a beautiful interface — it is to observe the effect of priority decisions on visual hierarchy. Pay attention to where your eye goes first, second, and last. Ask yourself whether that order matches the intended user flow.

Try deliberately breaking the hierarchy: make the surface loud, flatten all priorities to the same level, or set Interactive higher than Accent. Notice how quickly the layout becomes confusing or directionless. Then restore a clear hierarchy and observe how the interface resolves.

---

## Salience vs. Preference

The Visual Priority Map offers two tabs that measure fundamentally different things.

### Salience — "What grabs your eye?"

Salience measures involuntary attention capture: which color a user's eye lands on first, before conscious thought kicks in. The formula is contrast-dominant. A color that doesn't stand out from the background can't be salient no matter how vivid its hue. Once contrast is established, saturation and hue amplify the effect.

The hue salience curve peaks at red (evolutionary alertness signals — danger, blood, ripe fruit) with a secondary peak at blue. Green and yellow-green sit at the bottom. This aligns with attentional research showing that warm, high-contrast colors trigger faster reaction times.

A practical consequence: pure blue (#0000FF) scores higher than pure red (#FF0000) on a white background in salience mode. This is not a bug. Blue has a much higher luminance contrast against white (8.6:1 vs 4.0:1) because human vision weights green heavily in luminance calculations, making pure blue appear very dark. Contrast is the gate — even a "loud" hue can't win if it doesn't visually separate from its background.

### Preference — "What do people find pleasing?"

Preference is based on the findings of Camgoz, Yener, and Guvenc (2002), who studied foreground-background color combinations with 123 university students. Their key findings:

1. **Blue is universally preferred.** Regardless of background color, blue was the most preferred foreground hue (p = 0.0001). This held across red, yellow, cyan, green, and magenta backgrounds.
2. **Maximum saturation and brightness win.** The BS100 level (100% brightness, 100% saturation) was significantly preferred on almost every background tested.
3. **Hue, saturation, and brightness all matter.** All three attributes of color were statistically significant in determining preference.
4. **Preference ranking by hue** (from Fig. 3): Blue > Magenta > Purple > Red > Cyan > Green > Yellow > Yellow-Green.
5. **Gender and screen position had no effect** on preference choices.

Unlike salience, contrast is not the dominant factor in the preference formula. People preferred blue even on backgrounds where it had poor contrast. Instead, hue drives the score, with saturation and brightness as amplifiers. Achromatic colors (greys, black, white) score low because preference is inherently about chromatic appeal.

### Why both matter

A blue call-to-action scores high on both tabs — people will both notice it and like it. A red CTA scores highest on salience (urgency, alertness) but lower on preference. A desaturated grey content color scores well on salience (if it has good contrast) but poorly on preference (no hue identity).

This tension is the point. Designing effective UI means balancing what grabs attention with what feels pleasant. The two tabs let students observe where these goals align and where they conflict.

---

## Key Principles

- Color priority is about relative weight, not absolute color value. A color is "loud" or "quiet" only in relation to everything around it.
- The surface and surface alt colors set the baseline. Every other decision is measured against them.
- Reserve your highest-priority color for one thing. If two elements share priority 5, you effectively have no priority 5.
- Readable is not the same as attention-grabbing. Content should meet contrast standards without competing visually with interactive elements.
- Feedback colors occupy a special category — they need situational prominence, not permanent prominence.
- When in doubt, reduce. Most hierarchy problems come from too many loud colors, not too few.

---

## About

This tool was built for HCI (Human-Computer Interaction) courses at Universidad del Valle de Guatemala (UVG). It is intended as a hands-on complement to lecture material on visual design principles, giving students a low-friction way to experiment with color hierarchy decisions and observe their effects in a realistic layout context.

---

## References

- Camgoz, N., Yener, C., & Guvenc, D. (2002). Effects of Hue, Saturation, and Brightness on Preference. *Color Research and Application*, 27(3), 199-207. DOI: 10.1002/col.10051
