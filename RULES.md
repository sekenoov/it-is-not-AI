# Rules: how not to design like an AI

For designers and for AI agents. Drop this file into a prompt, a CLAUDE.md or a system message. Each rule targets a tell from [TELLS.md](TELLS.md).

## The principle

A model makes the most probable choice at every step. So the average choices have to be banned up front, and something specific has to be required instead. If a rule isn't written down, the model will fall back on the template.

## 1. Find one idea before drawing anything

- Write the idea in one sentence before any layout. It comes from the product's own material or story, not from "premium" or "modern".
  - Disposable camera app: 35 mm film. Frame counter, undeveloped negatives, orange date stamp.
  - Fintech called Tender: legal tender. The footer is the back of a banknote.
  - Royal Oak page: Genta drew it in a single night. The page is that night, the sketch becomes steel.
- Every element on the page must belong to that idea. If something is there only to look good, delete it.
- One idea. Not a moodboard of five.

## 2. Things you do not do by default

Use them only if the brief explicitly asks for them:

- floating 3D renders with a soft shadow below
- a giant pale word behind the hero object
- handwriting fonts
- blueprint or grid lines that don't match the object
- gradient backgrounds and blurred color blobs
- "Welcome to X" headlines
- a centered stack of three sign-in buttons
- a filled plus outlined button pair
- full-width black CTA, flat color swatches
- icon in a rounded square plus title plus text cards
- Product / Company / Resources / Legal footer columns with grey uppercase labels
- the category palette (green and cream fintech, purple AI, navy and gold luxury)
- more than one accent color, or one accent on more than two elements
- emoji in UI

## 3. Imagery

- **Order the flaws.** A model gives you a good photo by default. Ask for the bad one: direct flash, blink, red-eye, motion blur, tilted horizon, thumb in the frame, someone cut off, clutter left on the table.
- **Ban the generated finish.** No centered composition, no everyone smiling at camera, no cinematic light, no shallow depth of field, no clean skin, no golden hour.
- **Keep one bad shot in every set.** One overexposed frame in a grid makes the other eleven believable.
- **Avoid stock subjects.** No beach dog, no cat with mug and plant, no laughing dinner table, unless you break them hard.
- **Ground objects.** Use a tight dark contact shadow where the object touches the surface. Never a floating blur.
- **Spend fidelity where the eye lands.** If the hero is a watch, the bracelet taper and the brushed vs polished finish matter more than any background. If you can't model a part well, crop it out of frame.
- **Engraving follows form.** Lines wrap around slopes and curve with the terrain, swell and taper within a stroke, cross-hatch only in deep shadow. Horizontal scanlines with brightness-based thickness are a filter, not an engraving.
- **One hand for everything.** Every element in an illustration uses the same visual language. The sun in an engraving is engraved too.

## 4. Layout

- **One primary action per screen.** Secondary actions become plain text links.
- **No dead bands.** If two blocks have a gap between them, join them or remove one.
- **Show the mechanic, not a welcome.** The first screen demonstrates what the product does: an empty film strip, a banknote, a sketch.
- **Structure can carry the idea too.** Footer columns numbered like an engraving (01, 02). A CTA as an engraved cartouche. A dial picker as pencil studies in the margin.

## 5. Type and color

- One family for UI, at small sizes. One display face, used once.
- Pick the type for this product. Engraved capitals for a watch, monospace numerals for a frame counter.
- Accent color only on the one thing that matters on the screen: the counter, the shutter.

## 6. Product logic

- **Write down the core rule and check every screen against it.** "Nothing taken today is visible before 9 AM." Then look at each screen and find the violation. There usually is one.
- **Make the numbers add up.** Counters, dates, times, battery and badges must agree across screens. Generators never do this, so it's a strong human signal.
- **Remove ambiguity from labels.** "Develops at 9 AM", not "Ready at 9:00".
- **Use the current platform.** If it's iOS 26, the tab bar floats on glass. Icons come from one set, at one weight.
- **Check the concept isn't someone else's.** Search for it before you draw.

## 7. Copy

- No long dashes.
- No "seamless", "elevate", "unlock", "empower", "effortless", "next level".
- No lists of three adjectives. No "not just X, it's Y".
- Use real facts and specifics: reference numbers, exact times, a true anecdote.
- Write one line that only this product could say.

## 8. Things an AI does while working, and must not

- **Adding decoration to look premium.** Premium comes from fidelity and restraint, not from layers.
- **Stacking tropes when unsure.** If one idea doesn't carry the page, a second idea won't help. Find a better first one.
- **Filling empty space.** Leave it empty, or shrink the container.
- **Centering everything by default.** Alignment is a decision, so make one.
- **Drawing each screen in isolation.** Design the set, then check screens against each other.
- **Inventing a generic stand-in.** "Welcome to X", "Lorem", a stock landscape. Use the real content or a specific placeholder.
- **Accepting the first output.** The first output is the most probable one, so it's the most generic one.
- **Explaining in the UI.** Tooltips and subtitles that describe what the user can already see.
- **Hedging in the design.** Two buttons of equal weight because it couldn't decide. Four swatches because it couldn't choose. Decide.

## 9. Checks before you call it done

1. **Swap test.** Replace the logo with another brand's. If the page still works, it isn't done.
2. **Premium test.** Point at each element and name the idea it serves. If the only answer is "it looks premium", delete it.
3. **Zoom test.** Zoom to 300% on the hero. Filters, broken lines and blobs show up right away.
4. **Rule test.** Run every screen against the core rule from section 6.
5. **Numbers test.** Add up every counter, date and time across screens.
6. **First second test.** Show it to someone for one second. Ask what it reminded them of. If they name a template, a trend or "AI", go back to section 1.

## Prompt blocks

Paste these into image or UI prompts as they are.

**Photo with flaws**

```
Photo taken on a cheap disposable film camera with direct on-camera flash, scanned at a drugstore lab.
Make it a real throwaway shot, not a good photo: harsh flash falloff, background almost black, one person mid-blink or turned away, someone partly cut off by the frame edge, slight motion blur, tilted horizon, red-eye, visible grain, faded blacks, slight green cast in shadows, clutter left in frame.
Avoid: centered composition, everyone smiling at camera, cinematic lighting, shallow depth of field, clean skin, golden hour glow.
```

**UI guardrail**

```
Before designing, state the one idea in one sentence, taken from the product's own material or story. Every element must serve it.
Do not use: floating 3D renders with soft shadows, giant ghost words behind objects, handwriting fonts, decorative blueprint lines, gradient backgrounds, "Welcome to" headlines, centered stacks of sign-in buttons, filled plus outlined button pairs, icon-in-square feature cards, template footer columns, emoji, long dashes.
One primary action per screen. One UI typeface. Accent color on at most two elements.
Write down the product's core rule and check every screen against it before finishing. Make every counter, date and time agree across screens.
If an element exists only to look premium, delete it.
```
