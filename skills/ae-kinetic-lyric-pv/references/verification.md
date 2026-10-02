# Verification and delivery

Verify the rendered result, not merely the build script's exit code. Use checks proportionate to the production. Do not report a planned test as a completed one.

## Acceptance checks

| Check | Evidence to collect | Failure to resolve |
| --- | --- | --- |
| Full coverage | Section/timing map through the requested end, including instrumental passages | Missing lines, accidental blank gaps, premature ending |
| AE integrity | Saved project and inspected or reopened footage links; prototype/render logs | Missing artwork, substituted fonts, expression errors, unsupported output module |
| Export structure | Media probe plus a full error-reporting decode of video and audio | Truncated file, decoder errors, incorrect dimensions/frame rate, missing audio |
| Typography | Frames from every section and dense samples around motion | Clipped CJK glyphs, illegible secondary lines, low contrast, shimmer, collisions |
| Mode switching | Mode control and representative rendered frames in monochrome and color, when both are deliverable | Partial recoloring, unreadable accents, flat grayscale contrast, unintended changes to lyrics/timing/motion |
| Creative direction | Brief, lyric document, and representative section frames | Unrequested self-mockery or AI subject, artwork inconsistent with the selected style, tone that contradicts the brief |
| Synchronization | Listening/playback of phrase entries and section transitions where available | Drift, wrong repeated line, text too late or too briefly shown |
| Audio policy | Stream comparison or decoded-sample comparison appropriate to the claim | Unintended processing, offset, altered samples, unreported re-encoding |
| Fresh material | Current task's asset manifest and generation/drawing provenance | Historical assets or reference frames entering the final composition |

A probe describes a file; it does not establish that the whole file decodes. A successful decode establishes structural validity; it does not establish artistic quality or synchronization. Sampled frames reveal layouts; they do not establish unobserved motion. Keep those distinctions in the report.

## Audio preservation

Choose the claim before checking it:

- **Encoded stream preserved:** use stream copy into a compatible container. Compare extracted elementary audio payloads with consistent extraction; metadata and container bytes may differ. Codec names matching is insufficient evidence.
- **Decoded samples preserved:** compare decoded samples with the same format and channel mapping, accounting explicitly for encoder delay, padding, and time range. Do not hide an offset or trim to make a comparison pass.
- **Re-encoded audio:** report the codec/settings and conversion. It is not byte-identical to the source, even if it sounds similar.

An MP4 container's file hash will not match the source audio file. Do not use that comparison as an audio fidelity test. Check duration and start offset as well as content. Some formats or tools make exact payload comparison impractical; state that limit and use the strongest valid check available.

## Visual and timing review

Review at least one meaningful interval in each verse, each chorus variant, all instrumental sections, the opening, climax, and ending. Include the longest line, smallest important text, fastest transition, and most crowded arrangement. Sample motion densely enough to catch brief overlays or collisions. Confirm readability at the target viewing size after final compression.

Record the selected mode and palette. Verify that the mode control changes artwork treatment and palette-dependent layers together. When both modes are requested, render and review a representative sample in each, checking saturated backgrounds in color and tonal separation in monochrome. Keep timing, text, and motion identical unless the user asked to change them. If fresh color artwork is unavailable, report color switching as incomplete rather than testing only a text recolor. A single-mode delivery needs a full review of the requested mode and an honest statement of which alternative-mode checks were performed.

Listen to representative phrase entries in each section and check the full timeline for accumulated drift. Where possible, play the completed video from start to finish with sound. If playback tools are unavailable, retain the structural and frame checks but label listening/synchronization review as unverified. Automated signal analysis is supplementary evidence, not a replacement for hearing words.

## Final project package

Include the final video, saved editable AE project, current project's newly created artwork, lyric/timing document, and any task-local scripts needed to rebuild it. Keep media paths resolvable within the collected project. Do not package third-party font binaries by default. Include the current production's accurate credits where relevant; do not inherit credits from another project.

Summarize actual checks, remaining limitations, and the audio policy in a short verification document. Retain useful logs; clean only disposable intermediates inside the authorized task directory. Do not publish or commit the production package into this method-only skill repository.

When distributing the skill itself, include only its instruction files, references, Codex metadata, and MIT license. No example media, existing lyric excerpts, absolute personal paths, source project caches, or credentials belong in that distribution.
