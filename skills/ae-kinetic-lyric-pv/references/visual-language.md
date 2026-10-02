# Visual language and motion

Treat these as a coherent starting vocabulary, not a demand to clone a reference. Create a new title, scene order, motifs, character design, and specific compositions for each song.

## Selectable visual styles

Choose a visual treatment independently from color mode, lyric tone, and subject. The following are starting options; accept custom styles and combinations. Preserve readable lyric hierarchy and intentional section development in every style.

| Style | Artwork and layout direction | Motion direction |
| --- | --- | --- |
| Manga | Newly drawn ink/tonal illustrations, purposeful panel-like framing | Phrase reveals, panel wipes, restrained artwork drift |
| Minimal typography | Original text and geometric shapes; generous negative space | Word-group staging, line assembly, precise rhythmic cuts |
| Cinematic illustration | Fresh narrative scenes with intentional light, depth, and wide compositions | Slow scene movement, restrained parallax when supported, deliberate section cuts |
| Watercolor | Fresh painted artwork with paper-like texture, soft pigments, and clear space for text | Gentle fades, masks, and quiet movement; keep lyric text crisp |
| Retro print | Fresh poster-like composition, intentional grain and limited palette | Stepped reveals and bold graphic transitions; avoid accidental low-resolution artifacts |

Style affects artwork, composition, and motion choices. It cannot always be changed by a filter. If the user changes style mid-project, create the needed new artwork and revise affected layouts while preserving compatible lyrics and timing. Do not import an old style pack. For unspecified style, start with crisp narrative typography and tailor illustration to the song.

## Two visual modes

Both modes share the chosen visual style, type hierarchy, and phrase-driven motion. Mode selection changes the palette and artwork treatment, not the song's timing or narrative. Adapt the layout and motion suggestions below to the selected style.

| Mode | Palette and artwork | Selection |
| --- | --- | --- |
| `monochrome` / 黑白 | Near-black, white, and restrained gray; fresh grayscale artwork or desaturated fresh color artwork with tuned tonal separation | Default when the user has not selected a mode |
| `color` / 彩色 | Fresh color artwork; a coordinated background, foreground, and small set of accent colors | Use when requested, even if the reference is monochrome |

### Monochrome

Use a near-black field, white primary text, and restrained gray supporting elements. Suggested starting values are `#080808`, `#F2F2F2`, and a small number of gray steps. Preserve deliberate contrast between lyric, artwork, background glyph, and microtext.

### Color

Choose a palette from the current song's mood, not from an old project. Begin with a background, readable foreground, and two or three accent colors; keep illustration colors coordinated with them. Warm/cool relationships, restrained cinematic tones, or vivid manga colors are creative options rather than fixed requirements. Let a chorus evolve the balance of color without making every line a different rainbow hue.

Preserve the chosen artwork treatment and typography hierarchy. Use color to emphasize a lyric, section, or narrative turn. Keep important text readable against bright and saturated artwork, using negative space or a separate text field when necessary. Do not rely on hue alone to distinguish important information: retain tonal and structural contrast. Avoid grading that unintentionally obscures important visual detail; intentional painted softness is compatible with sharp lyric text.

### AE mode control

Expose a clearly labeled native control such as `Color mode` with `0 = monochrome`, `1 = color` on a project control layer. Route palette-dependent text, shapes, rules, symbols, and backgrounds through centralized color controls. Use native desaturation and tonal treatment on artwork/precompositions for monochrome; bypass that treatment for color. Verify the installed AE supports the chosen controls and expressions before building the complete project.

When both modes must be switchable, generate new color-capable artwork at the start of the current production. The monochrome view should be intentionally tuned, not accepted blindly after desaturation. When switching a previously grayscale-only project, create fresh color artwork rather than claiming that toggling saturation restores absent color. Check both modes for background/foreground contrast, clipping, and legibility. Deliver both renders only if requested; a mode control does not require duplicate timelines.

## Shared typography and clarity

Use large CJK serif-like lettering for lyrical emphasis where a suitable installed font exists; use a clear sans serif for secondary text and a compact mono or condensed face for metadata. Confirm real font coverage and render the actual characters. Do not identify a reference font by guesswork or bundle font files.

For 1920×1080, useful starting ranges are 48–80 px safe margins, 1–2 px separator rules, 24–32 px secondary text, and 14–20 px microtext. Scale these with the output and evaluate the compressed video at normal viewing size. Primary text size is driven by its length and composition. Keep essential lyrics large enough to read on a phone; metadata may be quieter but should not carry indispensable meaning.

Work at the output resolution or higher for artwork. Keep vector/text layers sharp. Align stationary horizontal rules carefully to avoid shimmer. Preserve intended texture and edges through export. A request to match a sharp screenshot usually concerns clarity, linework, and typography; it does not imply retro pixel art or deliberate blocky downsampling. Use pixel art only when that style is explicitly chosen.

## Layout families

| Family | Construction | Dramatic use |
| --- | --- | --- |
| Quiet title field | Original title, small secondary line, fine border/rules, restrained metadata | Introduce the motif and establish breathing room |
| Alternating lyric card | Fresh scene artwork on one side, lyric block on the other; reverse later | Give verses direction without monotonous centered slides |
| Wide illustration band | Original panoramic drawing with a separate lyric area | Open the world during a long phrase or instrumental section |
| Ghost-word field | One oversized, low-contrast current lyric keyword behind readable foreground text | Connect the line to a recurring emotional image |
| Chorus assembly | Newly designed geometric symbols or freshly drawn figures in a row, ring, or two-tier arrangement | Expand the visual scale of the refrain |
| Sparse ending | Reduce elements, complete a motif, let the last line settle | Resolve the emotional arc without a cluttered credit wall |

Use rules, chapter labels, counters, and a small progress cue as structural elements. Write metadata for the current project; do not reproduce another creator's handle, watermark, diagnostic labels, or branding. Avoid turning every frame into a dashboard.

Fresh symbols can share a consistent visual weight. Do not substitute a downloaded set of AI logos or extract reference icons. For a moving ring, orbit symbol positions around a center while keeping individual symbols upright when readability matters. Transforming the arrangement from a ring into rows can make a later chorus feel larger without adding visual noise.

## Motion grammar

- **Phrase reveals:** introduce meaningful word groups on vocal entries; use short opacity/position changes or text animators. Avoid revealing arbitrary single characters when that delays comprehension.
- **Held readability:** keep a stable interval after the reveal. A lyric should not be moving away while the viewer is still reading it.
- **Artwork drift:** use a restrained pan or scale change that preserves the focal point and negative space. Separate foreground elements only when the newly created drawing supports it.
- **Structural cuts:** align layout changes with audible phrase boundaries, accents, or section changes. Not every beat needs a cut.
- **Directional transitions:** thin sweeps, diagonal mask wipes, or stepped reveals can connect cards. Start around 2–8 frames for sharp accents, then adjust to the song and output frame rate.
- **Chorus expansion:** increase occupied space, widen rows, assemble original symbols, or reveal a larger background word. Make later refrains develop rather than loop mechanically.
- **Controlled disruption:** brief inversion or displacement can underline a specific lyrical moment. Use sparingly; sustained flicker, blur, or glitch harms the crisp vocabulary.

Use easing for deliberate arrivals and exits. Inspect the actual intermediate frames: an appealing first/last frame can hide collisions, premature cutoffs, or a transition that briefly covers the lyric. If a reference effect is unclear, propose a native construction and test its appearance rather than claiming the original implementation is known.

## Narrative rhythm

Shape section development around the chosen lyric tone and song. Intimate verses may grow into expansive choruses and a simpler ending, but a quiet or unresolved piece may call for a different arc. Alternate visual density, negative space, and focus. Humor is optional; use it only where the current text and brief support it.

A good lyric PV has a developing timeline. A series of still cards with identical entrances feels like a presentation even when the images are attractive. Give each section a different compositional purpose and at least one intentional motion event, without adding motion merely to fill time.
