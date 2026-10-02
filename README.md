# AE Kinetic Lyric PV Skill

[简体中文](README.zh-CN.md) · English · [MIT License](LICENSE)

A Codex skill for making narrative lyric videos in Adobe After Effects with switchable **monochrome and color modes**, **selectable visual styles**, and **independent lyric tones**, using native layers, expressions, keyframes, and project-specific scripts. It connects full-reference analysis, phrase-timed lyric writing, freshly created visuals, kinetic typography, and verified full-song delivery.

**This repository contains production instructions only. It contains no music, lyrics from existing songs, illustrations, character sheets, screenshots, brand logos, fonts, rendered videos, or AE projects. Every new production starts with newly created visual material. Reference videos inform decisions; their frames and assets are never copied into the output.**

## What it teaches

- Analyze the complete reference timeline, then inspect motion at a finer interval instead of relying on isolated keyframes.
- Write screen lyrics in the selected tone and align them to vocal phrases while preserving the current project's chosen audio.
- Combine fresh monochrome or color illustration, large CJK typography, quiet metadata, thin rules, alternating layouts, and restrained transitions.
- Build an editable, plugin-free AE project with independent text, artwork, shapes, and animation.
- Test a short engine prototype and a representative chorus before committing to a full render.
- Verify video decoding, timing, missing footage, text readability, and the stated degree of audio preservation.

It is an instruction skill, not a bundled renderer or a collection of reusable media. Resolution, frame rate, tone, budget, and composition are project decisions. The suggested 1080p/60 fps profile is adjustable.

## Two visual modes

| Mode | Visual direction | Invocation |
| --- | --- | --- |
| Monochrome | Black, white, restrained gray, crisp linework and strong tonal hierarchy | `Use monochrome mode` or `visual_mode: monochrome` |
| Color | Fresh color artwork and a coordinated palette, with the same typography and motion grammar | `Use color mode` or `visual_mode: color` |

Monochrome is the default when no mode is selected. The AE project exposes a mode control and centralized palette controls so a switch preserves lyrics, timing, and animation. A genuinely switchable project uses freshly created color-capable artwork with a tuned monochrome treatment. Grayscale-only artwork needs newly created color artwork before a full color version is possible. Only the requested mode is exported unless both versions are requested.

## Style, tone, and theme

These are independent choices, not presets that force one another:

| Choice | Examples |
| --- | --- |
| `visual_style` | Manga, minimal typography, cinematic illustration, watercolor, retro print, or your own combination |
| `lyric_tone` | Lyrical, uplifting, soothing, melancholic, romantic, narrative, satirical, self-deprecating, or a custom tone |
| `theme` | The subject you choose; an AI theme is optional |

Self-deprecation is one option, not the default. A monochrome PV can be uplifting and a color PV can be melancholic. Changing visual style may require new artwork and layout work; changing tone may require rewriting lyrics. Only color mode is designed as an AE toggle, and no historical media is reused for any of these changes.

## Install in Codex

Ask the built-in installer:

```text
$skill-installer Install the skill from https://github.com/yifanchen12/ae-kinetic-lyric-pv-skill/tree/main/skills/ae-kinetic-lyric-pv
```

Alternatively, place the complete `skills/ae-kinetic-lyric-pv` folder in the user skill directory recognized by your Codex installation. Keep its reference documents and license together. Consult the [official skill documentation](https://learn.chatgpt.com/docs/build-skills) for local discovery locations. Newly installed skills should be available on the next turn; if the entry does not appear, restart Codex.

## Use

```text
$ae-kinetic-lyric-pv Create a full-length lyric PV from the audio and lyrics I provide for this project. Use color mode, watercolor visuals, a soothing lyric tone, and a theme of companionship. Analyze my reference video across its entire duration, create all visual artwork anew, and deliver an editable plugin-free AE project plus a verified video. Use my chosen project directory and budget.
```

Provide the current audio, source text when needed, an optional reference video, output directory, and creative constraints. The skill distinguishes screen lyric adaptation from rewriting the actual sung vocals. A reference is optional; there are no bundled example media.

For color, add `Use color mode` to the request. To change a current project, request `Switch this project's visual mode to color; retain the lyrics, timing, and motion, then verify a short preview`. The same operation supports switching back to monochrome. All artwork must originate in the current project.

## Requirements and boundaries

Actual video production needs an accessible, licensed After Effects installation and tools capable of operating it or running project scripts. Media inspection tools such as FFmpeg/FFprobe are useful. Illustrated scenes require an available image-generation capability or newly drawn artwork; typography and geometric scenes can be created natively. The skill does not install paid software, provide an Adobe license, guarantee access to a model, or require third-party AE plugins.

The agent must disclose missing capabilities and unverified checks. It must not silently substitute old project assets. Publication, paid purchases, and cleanup outside the current project require their own task authorization.

## Package

```text
skills/ae-kinetic-lyric-pv/
├── SKILL.md                       Entry point and production boundaries
├── LICENSE                        License retained with the installed skill
├── agents/openai.yaml             Codex display metadata
└── references/
    ├── workflow.md                Analysis, writing, AE build, storage, delivery
    ├── visual-language.md         Layout, illustration, typography, motion
    └── verification.md            Acceptance checks and honest reporting
```

## License

The original instructions and documentation in this repository are released under the [MIT License](LICENSE). The license does not grant rights to music, fonts, artwork, trademarks, or reference videos supplied for a future production. Those materials retain their respective rights and are not included here. This is an independent community project with no affiliation or endorsement from Adobe or OpenAI.
