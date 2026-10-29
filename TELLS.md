# Tells: how AI design gets caught

A model picks the most probable option at every step. One average choice is invisible. Twenty of them in a row make a page that looks generated, even when nothing is technically wrong.

This is a list of the tells people notice first, roughly in that order.

## Imagery

- **Everyone's a winner.** Every photo is a good photo: centered subject, everyone laughing into the lens, the dog frozen mid-stride with a perfect reflection. Real camera rolls are mostly throwaway shots: a blink, a thumb over the lens, red-eye, a tilted horizon, someone cut off by the frame.
- **Stock prompt subjects.** Dog running on a beach at sunset. Cat on a windowsill next to a mug and a plant. Friends laughing at a dinner table. A guy giving a thumbs up from the driver's seat. Girl on a bike at night. If the subject list reads like a prompt for "aesthetic photos", viewers read it the same way.
- **Generated photo finish.** Clean skin, cinematic lighting, shallow depth of field, golden hour glow, slight film grain that looks added.
- **The floating 3D object.** A glossy plastic render hanging in the air with a soft blurred shadow far below it. This is the most recognizable generated onboarding illustration right now.
- **Baked-in background.** The image was dropped in with its own background and shadow, so the shadow gets clipped by the screen edge or the white doesn't match the page white.
- **Low fidelity where it matters.** A procedural 3D model where the hero part is built from identical boxes: a watch bracelet made of rectangular blocks that look like keyboard keys, flat grey metal with no difference between brushed and polished surfaces. The viewer looks exactly where the model is weakest.
- **The image-to-lines filter.** Horizontal scanlines whose thickness follows brightness. It reads as "engraving" for half a second, then as a shader. Real engraving lines follow the form: they wrap around a slope, curve with a valley, cross-hatch in deep shadow.
- **Uneven detail.** One mountain is carefully modeled, the other is flat. Trees turn into blobs. Lines break into noisy dashes.

## Decoration

- **The ghost word.** A giant pale serif word (usually the product name) set behind the hero object and cut off by it.
- **Fake handwriting.** Annotations in a handwriting font with leader lines. The letters are identical every time, the pressure never changes, and the lines point at empty space. Half a label hidden behind the object looks like a mistake, not a choice.
- **Decorative blueprint.** Technical drawing lines under the product that do not match its geometry. They are there for texture, and it shows.
- **Stacking.** Ghost type, plus handwriting, plus blueprint, plus 3D, plus soft shadow, plus configurator. Each one is a known premium trope, and together they read as an answer to "make it look premium".
- **Mixed visual languages.** An empty outlined circle as the sun inside a detailed engraving. A clean vector icon inside a painted scene. One element drawn by a different hand breaks the whole picture.

## Layout

- **The default welcome screen.** Illustration, "Welcome to X", grey subtitle on two lines, Continue with Apple, Continue with Google, Continue with email, tiny Terms text. Everything centered. It says nothing about the product.
- **The default footer.** Logo, tagline and two buttons on the left, four columns on the right (Product, Company, Resources, Legal) with grey uppercase labels, legal fine print at the bottom.
- **The button pair.** One filled button next to one outlined button, always with the same weight.
- **Full-width black CTA and flat color swatches.** The configurator from every online store, whatever the product is.
- **Icon in a rounded square, title, text, button.** The feature card that can hold any feature of any product.
- **Dead bands.** A 300 px empty gap between two blocks that were clearly generated separately and never joined.

## Color and type

- **One color for everything.** Yellow background, yellow product, yellow counter, yellow badge. The palette was generated from a single word.
- **Category palettes.** Deep green on cream for fintech, purple gradient for AI, navy and gold for luxury.
- **Three typefaces with no relation to the brand.** A neutral grotesk for UI, a bookish serif for the ghost word, a handwriting font for notes. None of them was chosen for this product.
- **Default UI font** at default sizes, default tracking, default weights.

## Product logic

- **Screens that break the product's own rule.** The app says you will see photos tomorrow, and the camera screen shows the photo full size right now. The "tonight" grid shows thumbnails of shots that should be hidden. Generators draw each screen on its own and never check them against each other.
- **Ambiguous labels.** "Tonight, ready at 9:00" at 11:46 PM reads as 9 PM, which has already passed.
- **Outdated platform.** A grey solid tab bar from iOS 17 in an iOS 26 world. Mixed icon styles: two outlined system symbols and one custom filled glyph.
- **A known concept with a new name.** "Photos develop the next morning at 9" is an app that already existed. Someone in the comments will name it.

## Copy

- Long dashes everywhere.
- "Seamless", "elevate", "unlock", "empower", "effortless", "next level", "built for the way you work".
- Lists of exactly three adjectives.
- "Not just X, it's Y."
- Headlines that could sit on any product's landing page.

## What reads as human

These do not look generated, so keep them:

- **Invented details that add up.** 24 shots minus 8 taken equals "16 left". Later "9 so far, 15 left". Yesterday's date stamp matches today's date minus one. The battery drains from screen to screen as the clock moves.
- **Exact facts.** Reference 15510ST, 41 mm, calibre 4302. A real anecdote instead of a slogan.
- **Specific copy.** "You'll see this one tomorrow at 9." beats "Capture moments that matter."
- **A visible flaw on purpose.** An overexposed shot in the grid. A correction line crossed out in a sketch.

The problem is that these details are quiet and only noticed on a second look, while the tells above are noticed in the first second.
