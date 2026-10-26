# v1.0.0 publication review

This file is for the manual's maintainer, not part of the reader-facing manual.

## Source baseline

The manual targets ArtemisOS / Houston **v1.0.0**, as requested. Behaviour was checked against these source snapshots on 26 October 2026:

| Component | Branch | Commit |
| --- | --- | --- |
| Houston | dev | `7cf9dbc55bd67d27b4d0cb8088f074bfcbed5a12` |
| Launchpad | main | `e2ed8c7e6484961027ff0d59f4ed64c50a303acd` |

The current Houston dev branch was explicitly selected for verification. These are development snapshots, not proof that the final v1.0.0 image contains exactly this code. Launchpad's source still includes a “0.9 beta” Houston badge; the reader manual therefore distinguishes application labels from the ArtemisOS release and asks users to report the Build identifier.

## What was checked

- Preset sharing, duplication and immediate library deletion; editor save prompts and CTRL/buffer persistence.
- Song/utility behaviour, Invert Menu, hold defaults, LED modes and independent Stompbox state.
- Setlist ordering, initial preset selection and automatic saving.
- Expression calibration, curve/smoothing controls and per-preset assignments.
- MIDI PC/CC mappings, address ranges, clock controls and editor-specific command scope.
- NAM/IR transfer paths, import formats, library rename/delete behaviour and automatic import.
- Launchpad archive/restore/reset paths and USB transfer ownership.
- Reader documentation links, image references, heading anchors and Markdown structure.

Key source locations include Houston's `backend/midi_map.py`, `backend/DOCUMENTATION.md`, `ui/src/lib/jamUtilities.ts`, `footswitchConfig.ts`, `ledConfig.ts`, `expressionControlConfig.ts`, `presetPedalCatalog.ts`, `virtualPedalCategories.ts`, the editor/manager views, and the pedal JSON catalogues. Launchpad's `webkiosk/user_archive.py`, `data_paths.py`, `file_manager.py` and Storage/Updates/Asset UI establish the maintenance workflows.

## Editorial decisions

- Kept the confirmed example wiring: OC-2 L1, TS9 L2, DS-2 L3 and stereo CE-20 L6/L7.
- Kept shared-preset and mixer-save behaviour explicit. Saving a song does not create an independent copy of its sounds.
- Corrected MIDI capacity to 7,680 presets, 7,808 songs and 128 setlists. Documented CC 0 as the EXP BT source, following the runtime behaviour rather than the older selected-parameter label.
- Distinguished a Houston archive from the separate USB transfer area. Recordings and pending imports need separate copies.
- Removed unverified 2.3 ms latency and approximately 30 ms switching figures from the reader-facing specifications. Keep measured figures out until the release configuration and measurement conditions are approved.
- Did not invent expression resistance/pinout or CTRL voltage/current ratings. These remain undetermined, as confirmed by the product owner. The manual describes calibration and relay-contact use and routes model-specific compatibility questions to support.
- Did not advertise general Bluetooth MIDI interoperability or USB MIDI/audio. Current source contains a Shuttle-related Bluetooth workflow behind an opt-in path; its protocol entries are identified in the MIDI reference without promising support for arbitrary devices.
- The effects reference lists visible pedal choices; hidden legacy catalogue entries are omitted. Its suggested settings are listening starting points, not hardware-tested factory presets.

## Final release checks

The documentation work is complete, but these checks require the actual release image and hardware:

1. Follow Quick Start on v1.0.0, including input/output selection, loop bypass and shutdown.
2. Recall edited presets through songs; check mixer save prompts, CTRL/buffer persistence and Stompbox independence.
3. Reopen a setlist after editing and confirm order, starting presets and footswitch/LED defaults.
4. Exercise MIDI recall, clock and Thru with external equipment; confirm the displayed map agrees with the documented runtime.
5. On a test unit with disposable data, create an archive, copy it off-device, restore it and perform Factory Reset. Confirm recovery of the intended data and separate handling of recordings.
6. Run the update sequence, including the matching firmware stage, on the release image.
7. Compare screenshots with the release UI and refresh any materially changed controls. Additional setlist, calibration and Storage screenshots would improve the text-only walkthroughs.
8. Confirm the retained physical specifications against the production hardware sheet. Add electrical compatibility limits only after they are approved.
9. Preview the intended publishing format. The Markdown includes Mermaid diagrams, so a PDF/site export needs a renderer that supports Mermaid and preserves relative image/link paths.

No hardware measurements, destructive device operations or firmware installations were performed during this documentation edit.
