---
name: ae-kinetic-lyric-pv
description: Make full-length narrative lyric PVs in Adobe After Effects with switchable monochrome/color modes, selectable visual styles and lyric tones, fresh artwork, phrase-synchronized screen lyrics, kinetic typography, and native plugin-free animation. Use for lyrical, uplifting, soothing, satirical, or other reference-inspired lyric video production; not for generic highlight cuts or asset reuse.
license: MIT
---

# AE Kinetic Lyric PV

Turn the current project's audio and creative brief into an editable, full-length lyric PV. Offer monochrome and color modes, selectable visual styles, and independent lyric tones while preserving readable typography and phrase-driven motion. Create a new visual identity for each project. Explicit user instructions take precedence over the stylistic defaults below.

## Independent creative choices

Record `visual_mode`, `visual_style`, `lyric_tone`, and `theme` separately. Mode means monochrome or color; visual style means the drawing/layout treatment; lyric tone means the voice and emotional arc; theme means the subject. None determines the others. A color video can be sorrowful; a monochrome video can be uplifting. An AI topic and self-mockery are optional, not defaults.

Offer a compact choice when useful: visual styles may include manga, minimal typography, cinematic illustration, watercolor, or retro print; lyric tones may include lyrical, uplifting, soothing, melancholic, romantic, narrative, satirical, or self-deprecating. Accept the user's own style or a coherent combination instead of limiting them to this list. Match the brief and song; when unspecified, use crisp narrative typography with a tone suited to the song and state the choice.

Changing tone may require new lyrics and a revised storyboard. Changing visual style may require newly created artwork and redesigned layouts; it is not a palette toggle. Preserve timing and motion where compatible, and revise what no longer serves the new direction. Do not promise every style can be switched with one AE control.

## Mode selection and switching

- Support `visual_mode: monochrome` (黑白模式) and `visual_mode: color` (彩色模式). Honor the user's selection; when none is given, state that monochrome is the default and continue. Do not infer monochrome solely from a black-and-white reference when color was requested.
- Keep the selected mode and palette in the project data and expose one clearly labeled AE mode control. Centralize palette decisions so switching updates artwork treatment, text, rules, symbols, and backgrounds coherently. Preserve lyrics, timing, layer structure, and motion.
- For two genuinely switchable versions, create fresh color-capable artwork for the current project and derive its monochrome appearance with native desaturation and tonal adjustments. Grayscale artwork cannot recover its original colors; if only grayscale art exists, a color switch requires newly created color artwork. Never claim a grayscale filter creates a true color version.
- Export only the requested mode unless both versions are requested. When switching an existing project, recheck contrast and readability and render a short sample before the final export. This does not authorize historical asset reuse.

## Essential boundaries

- This package supplies methods only. Create all production artwork, character designs, decorative symbols, and scene graphics anew for the current project. Never import historical project assets, old AE projects, cached generated images, stock starter packs, or artwork extracted from reference frames. Do not silently substitute old material when generation is unavailable.
- Inspect only inputs selected for the current task. Reference videos and screenshots are analytical inputs, not production footage. Do not copy their illustrations, exact compositions, logos, watermarks, or creator identity. Derive abstract layout and motion principles, then design new scenes.
- The current task's chosen audio may be imported as requested. Installed fonts may be used without bundling their files. Do not include music, fonts, source lyrics, artwork, or rendered examples in a distributable copy of this skill.
- Separate screen lyric adaptation from a vocal rewrite. Keeping the source recording does not make new screen text its sung words. Preserve the requested audio and describe the adaptation accurately.
- Deliver through available tools. Do not claim that AE, image generation, audio playback, or rendering ran when they did not. If a capability is missing, finish the useful independent writing or planning work and identify the concrete dependency.

## Work sequence

1. Establish current inputs, theme, lyric tone, visual style, visual mode and palette, audio policy, output root, budget, and target format. Ask only for missing information that materially blocks the next step. Discover the installed AE and available media tools; do not assume a version, executable path, plugin, or image model.
2. For a supplied reference, analyze the entire timeline and inspect motion intervals in detail. Record coverage and separate observations from proposed implementations. Read [workflow.md](references/workflow.md) for analysis, lyric writing, timing, storage, and AE construction.
3. Draft a graceful project title, full screen lyrics, section map, and timed storyboard in the selected tone and theme. If an AI theme or self-mockery is requested, use concrete personal moments rather than a catalogue of model names. Follow the song's phrase lengths, pauses, repeats, and emotional escalation.
4. Read [visual-language.md](references/visual-language.md). Design original layouts and freshly created artwork for the selected visual style and monochrome or color mode. Keep text sharp and artwork faithful to its chosen treatment; do not introduce pixelation unless requested.
5. Prove a short native-AE prototype, then a representative passage containing the most demanding typography and transitions. Keep text, shapes, artwork, and motion editable. Scale the validated construction to the complete song, including intro, instrumental breaks, and outro.
6. Read [verification.md](references/verification.md) before export. Render, inspect the full output structurally, review every section visually, and check lyric/audio timing through playback when available. State the exact checks performed and any limitations.
7. Deliver the video, editable project, current project's newly created assets, lyric/timing document, and concise verification report. Confirm that the saved project can resolve its footage. Publishing the result is a separate action unless the user has requested it.

## Completion standard

The requested song or excerpt is covered; screen text follows the intended phrases; motion develops across sections; typography remains sharp and readable; the AE project has editable layers and working footage links; the exported video decodes without errors; audio meets the stated preservation requirement. Report partial completion honestly if tools or inputs prevent any of these checks.

Use the user's project root for large files. Change AE cache paths or clean storage only when requested, limiting changes to the authorized locations. Never make global storage changes a prerequisite for this skill.
