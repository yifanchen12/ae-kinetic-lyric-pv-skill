# AE Kinetic Lyric PV Skill

[简体中文](README.zh-CN.md) · English · [MIT License](LICENSE)

A Codex skill for making monochrome narrative lyric videos in Adobe After Effects using native layers, expressions, keyframes, and project-specific scripts. It connects full-reference analysis, phrase-timed lyric writing, crisp manga-inspired visuals, kinetic typography, and verified full-song delivery.

**This repository contains production instructions only. It contains no music, lyrics from existing songs, illustrations, character sheets, screenshots, brand logos, fonts, rendered videos, or AE projects. Every new production starts with newly created visual material. Reference videos inform decisions; their frames and assets are never copied into the output.**

## What it teaches

- Analyze the complete reference timeline, then inspect motion at a finer interval instead of relying on isolated keyframes.
- Write lyrical, optionally self-deprecating screen text and align it to vocal phrases while preserving the current project's chosen audio.
- Combine black-and-white illustration, large CJK typography, quiet metadata, thin rules, alternating layouts, and restrained transitions.
- Build an editable, plugin-free AE project with independent text, artwork, shapes, and animation.
- Test a short engine prototype and a representative chorus before committing to a full render.
- Verify video decoding, timing, missing footage, text readability, and the stated degree of audio preservation.

It is an instruction skill, not a bundled renderer or a collection of reusable media. Resolution, frame rate, tone, budget, and composition are project decisions. The suggested 1080p/60 fps profile is adjustable.

## Install in Codex

Ask the built-in installer:

```text
$skill-installer Install the skill from https://github.com/yifanchen12/ae-kinetic-lyric-pv-skill/tree/main/skills/ae-kinetic-lyric-pv
```

Alternatively, place the complete `skills/ae-kinetic-lyric-pv` folder in the user skill directory recognized by your Codex installation. Keep its reference documents and license together. Consult the [official skill documentation](https://learn.chatgpt.com/docs/build-skills) for local discovery locations. Newly installed skills should be available on the next turn; if the entry does not appear, restart Codex.

## Use

```text
$ae-kinetic-lyric-pv Create a full-length monochrome lyric PV from the audio and lyrics I provide for this project. Analyze my reference video across its entire duration, write an original self-deprecating AI-themed adaptation for the screen, create all visual artwork anew, and deliver an editable plugin-free AE project plus a verified video. Use my chosen project directory and budget.
```

Provide the current audio, source text when needed, an optional reference video, output directory, and creative constraints. The skill distinguishes screen lyric adaptation from rewriting the actual sung vocals. A reference is optional; there are no bundled example media.

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
