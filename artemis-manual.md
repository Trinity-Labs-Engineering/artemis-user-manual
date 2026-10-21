# Artemis User Manual

## Table of Contents

- [Introduction](#introduction)
- [Specifications](#specifications)
- [Rear Panel Connections](#rear-panel-connections)
- [System Diagram](#system-diagram)

## Introduction

## Specifications

### Mechanical

| Item | Specification |
| --- | --- |
| Dimensions (W × D × H) | Approx. 25.5 × 14.5 × 5.5 cm (10.0 × 5.7 × 2.2 in) |
| Mass | Approx. 1.5 kg — to be confirmed |
| Enclosure | 2.5 mm bead-blasted, anodised aluminium |
| Side panels | 5 mm solid walnut |

### Power, processing and controls

| Item | Specification |
| --- | --- |
| Power supply | 12 V DC, 2 A, centre-positive, 2.1 mm barrel connector; power supply included |
| Processor | Raspberry Pi Compute Module 5; 2.4 GHz quad-core Arm Cortex-A76 |
| Display | 6.25-inch touchscreen |
| Footswitches | 5 momentary footswitches |
| Indicators | 5 individually addressable RGB LEDs |
| Power control | Power button |
| MIDI | 5-pin DIN MIDI IN and MIDI OUT; optically isolated MIDI input |
| USB | USB-C, device mode only; Artemis requires its DC power supply |
| Expression inputs | 2 × 6.35 mm (1/4-inch) TRS expression pedal inputs |
| Control outputs | 2 × 6.35 mm (1/4-inch) TS isolated relay-contact outputs for amplifier switching or footswitch emulation |

### Audio and routing

| Item | Specification |
| --- | --- |
| Audio inputs | 2 independent inputs for stereo or dual-mono operation |
| Audio connectors | 6.35 mm (1/4-inch) TS, unbalanced; each loop channel has separate send and return sockets |
| Input routing | Either input can feed either bus; one input can also feed both buses |
| Signal paths | 2 analogue buses: Bus A and Bus B |
| Reorderable loops | 5 mono loops (L1–L5), with relay-switched true bypass |
| Loop assignment | L1–L3 assignable to Bus A or Bus B; L4–L5 on Bus A only |
| Fixed stereo loop | L6/L7 form the left/right channels of the final stereo loop, with relay-switched true bypass |
| Audio outputs | 2 outputs for stereo or dual-mono operation |
| Mixer | 2-channel analogue mixer for blending Bus A and Bus B |
| Input buffers | Switchable buffers with a shared bypass control |
| Output pads | Selectable nominal −6 dB pads on both bus outputs, before the mixer |
| Polarity control | Selectable polarity inversion on Bus B |
| Virtual blocks | 2 mono DSP blocks (V1 and V2), each independently bypassable or assignable to a Pre, Mid or Post position on either bus |

### Virtual block positions

| Position | Bus A | Bus B |
| --- | --- | --- |
| Pre | Before slot 1 | Before slot 1 |
| Mid | After slot 2, before slot 3 | After slot 1, before slot 2 |
| Post | After slot 5 | After slot 3 |

Slots are positions in the reordered chain, not fixed loop numbers. Bypassed loops still occupy their slots. Both Post positions are before the output bus swap and final stereo loop.

V1 and V2 can use the same position or different positions on either bus. When both use the same position, the signal passes through V1 followed by V2. Bypassing a virtual block keeps the signal on its analogue through-path.

### Digital audio and switching performance

| Item | Specification |
| --- | --- |
| Sample rate | 48 kHz (32bit) |
| Reported round-trip latency per virtual block | 2.3 ms at 48 kHz, using 32 frames per period and 2 periods |
| Best-case switching time, analogue-only changes | Approx. 30 ms; test conditions to be documented |
| DSP/NAM preset switching time | Depends on the preset and DSP load; worst-case figure to be confirmed |

Round-trip latency describes audio passing through a virtual block. Preset switching time describes the transition between presets and is a separate measurement.

## Rear Panel Connections

![Artemis rear panel showing labelled inputs, loop sends and returns, expression inputs, control outputs, audio outputs, power, USB and MIDI sockets](assets/images/artemis-io.JPG)

*Rear view of Artemis. The guide below follows the connector groups from left to right as shown in the photograph.*

| Panel label | Position | Function |
| --- | --- | --- |
| IN A / IN B | Leftmost pair: A above B | Two audio inputs, routable to Bus A or Bus B. |
| L1–L5: SND / RTN | Five pairs, each with SND above RTN | Reorderable mono effects loops. Connect SND to the pedal's input and the pedal's output to RTN. |
| L6/7: SND L / SND R / RTN L / RTN R | Two pairs within the L6/7 outline: left channel on the left, right channel on the right; sends above returns | Fixed stereo effects loop. Connect the sends to the effect's left/right inputs and its left/right outputs to the matching returns. |
| EXP 1 / EXP 2 | EXP 1 above EXP 2 | Two TRS expression pedal inputs. |
| CTRL 1 / CTRL 2 | CTRL 1 above CTRL 2 | Two isolated relay-contact outputs for compatible amplifier switching or footswitch inputs. |
| OUT L / OUT R | OUT L above OUT R | Main left and right audio outputs. |
| 12 V DC | Above MIDI IN | Power input for the supplied 12 V DC, 2 A, centre-positive adapter. |
| USB | USB-C socket above MIDI OUT | USB device connection to a host computer. Artemis still requires its DC power supply. |
| MIDI IN / MIDI OUT | Lower-right DIN sockets: IN on the left, OUT on the right | MIDI IN receives messages from an external controller; MIDI OUT sends messages to connected equipment. |

Audio inputs, outputs and loop sends/returns use 6.35 mm (1/4-inch) TS connections. Expression inputs use TRS connections; CTRL outputs use TS connections.

## System Diagram

![Artemis system diagram](assets/images/analog-architecture.png)
