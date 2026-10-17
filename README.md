# Ben Patterson

Senior staff software engineer — 13 years shipping production C/C++ and Python on safety-critical aerospace programs, and a daily practitioner of LLM coding agents.

I use agent harnesses every day for code review, debugging, tooling, and research. Most of that work sits on proprietary, access-restricted hardware, so it can't live here. The public projects below are things I designed, built, and tested myself, with agents as part of the workflow.

## What's here

| Repo | What it is |
|---|---|
| [epub-reader](https://github.com/bpbenpatterson/epub-reader) | Kotlin Android app that reads EPUB books aloud through the system TTS engine — sentence-level navigation, chapter progress, sleep timer, resume, recents. |
| [what-to-wear](https://github.com/bpbenpatterson/what-to-wear) | Kotlin Android app giving clothing advice from current location and weather. Open-Meteo API, programmatic UI, no framework. |
| [blockbound](https://github.com/bpbenpatterson/blockbound) | Browser voxel sandbox in Three.js — procedural biomes, mining, crafting, day/night cycle. Single HTML file, no external image assets. |

## How I work

**Agents as leverage; verification as the job.** I check generated code against the compiler, the tests, and real hardware behavior before acting on it — a habit from safety-critical work that transfers directly to non-deterministic systems.

**Context is the real constraint.** I built an MCP server that hands an agent structured `{file, line, severity, message}` compiler diagnostics instead of dumping thousands of lines of raw build output into its context window.

**Tooling has to meet people where they are.** I wrote roughly 10–15 helper and automation scripts over about 18 months; 3–5 of them were actually adopted by other engineers. The adoption gap taught me more than the scripts did.

## Background

Embedded and real-time systems: RTOS and bare-metal, multi-core SoC, ARM Cortex-M, Xilinx Zynq, device drivers and bootloaders, DSP and FPGA. Debugging is the part I like most — GDB and JTAG on target hardware, PDB for Python tooling, root-cause work across the stack from algorithm down to hardware/software integration.

Also: static analysis, unit and integration testing, GitLab CI regression gates, and legacy-system rescue.
