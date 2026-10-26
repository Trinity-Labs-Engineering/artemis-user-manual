# Artemis User Manual

> **Drafting guide:** Work through the unchecked items below, replacing each with finished instructions and illustrations. For walkthroughs, include the starting setup, exact Houston actions, expected result, and what needs saving. Document features available in the manual's stated software version. Remove this guide and remaining drafting prompts before publication.

## Table of Contents

- [Introduction](#introduction)
- [Quick Start](#quick-start)
- [Connections](#connections)
- [Routing Basics](#routing-basics)
- [Building a Preset](#building-a-preset)
- [Playing Live](#playing-live)
- [MIDI](#midi)
- [Digital Effects](#digital-effects)
- [Maintenance and Troubleshooting](#maintenance-and-troubleshooting)
- [Reference](#reference)

## Introduction

Artemis brings your effects pedals and built-in digital effects together in one pedalboard system. You can arrange your signal path, create presets, and recall sounds as you play. This introduction takes you through the startup screen, connecting to Wi-Fi, checking for updates, and opening Houston, the main application.

### Launchpad Basics

When you switch on Artemis, it opens Launchpad. This is where you manage device settings, including Wi-Fi, software updates and storage, and launch applications.

Houston is the main application for setting up your pedalboard, working with effects and managing presets. You can open it from the **Apps** tab in Launchpad.

![Launchpad Apps tab showing Houston ready to launch](assets/screenshots/launchpad_load.png)

#### Connecting to Wi-Fi

For your first setup, we recommend connecting Artemis to a Wi-Fi network. This makes it easy to download software updates and browse Neural Amp Modeler (NAM) models, which recreate the sound of amplifiers and pedals.

Open the **Wi-Fi** tab in Launchpad and connect to your network.

![Launchpad Wi-Fi settings](assets/screenshots/wifi_settings.png)

### Artemis Software Updates

Once connected, we recommend checking for software updates so you have the latest features and effects. Follow the Wi-Fi instructions below, or see [USB Updates](#usb-updates) in Maintenance and Troubleshooting to transfer an update from your computer.

#### Wi-Fi Updates

1. Connect Artemis to a Wi-Fi network.
2. Open the **Updates** tab in Launchpad and select **Wi-Fi**.
3. Follow the guided wizard to download and install the update. If prompted, delete a previously cached update bundle to make space. This cached bundle is safe to delete.
4. When installation is complete, reboot Artemis when prompted to finish the update.

![Wi-Fi update page in Launchpad](assets/screenshots/wifi_updates.png)

### Opening Houston

When you have finished setup and any update has completed, open the **Apps** tab in Launchpad. Find **Houston** and tap the orange play button to launch it.

### Houston Home Screen

The screen below shows Houston's Home screen. The following sections introduce the main areas of Houston; when you are ready to connect your instrument and get your first sound, follow [Quick Start](#quick-start).

![Houston Home screen](assets/screenshots/home_screen.png)

### My Pedalboard

### Presets, Songs and Setlists


## Quick Start

### Before you begin

- [ ] List the supplied items and the cables, instrument, pedal and amplifier needed for the walkthrough.
- [ ] Explain the power requirements and essential connection precautions before first use.

### First-time setup

Follow [Launchpad Basics](#launchpad-basics) for initial setup, then [open Houston](#opening-houston) to begin the walkthrough.

- [ ] Identify the starting screen and initial settings needed for the first-sound walkthrough.

### Get your first sound

- [ ] Walk through the simplest guitar-to-amplifier connection, including input selection, routing, output settings and level checks.
- [ ] State what the user should hear and link to troubleshooting if there is no sound.

### Add one pedal

- [ ] Show one pedal connected to L1, enable the loop, and demonstrate the difference between active and bypassed states.
- [ ] Add a simple cable diagram and a screenshot of the resulting route.

### Shut down

- [ ] Document the shutdown procedure and the indication that power can be disconnected.

## Connections

### Rear Panel Connections

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

### Example setups

- [ ] Add a labelled mono guitar/pedal/amplifier wiring example.
- [ ] Add a stereo example showing the L6/7 sends and returns and both main outputs.
- [ ] Explain the routing settings needed for each example, alongside its cable diagram.

### Expression, control and MIDI connections

- [ ] Document compatible expression pedal wiring, resistance range and calibration procedure.
- [ ] Explain CTRL contact wiring, electrical limits and supported switching modes with one compatible amplifier example.

See [MIDI](#midi) for controller connections, channel settings and message setup.

### USB connection

- [ ] Document the available USB functions, supported hosts and connection steps, including the separate DC power requirement.

## Routing Basics

### System Diagram

![Artemis system diagram](assets/images/analog-architecture.png)

### Buses and loop assignment

- [ ] Explain Bus A and Bus B, input selection, and the difference between series and parallel signal paths.
- [ ] Show how the five mono loops are shared, including the L1–L3 assignment options and L4–L5 restriction.
- [ ] Explain where the fixed L6/7 stereo loop sits and when to use it.

### Virtual block placement

- [ ] Explain the two virtual blocks and their Pre, Mid and Post positions with one worked routing example.
- [ ] Show how reordering and bypassing physical loops affect the slot positions, and what happens when both virtual blocks share a position.

### Levels, mixing and bypass

- [ ] Explain input buffers, pads, Bus B polarity, bus levels, mixing and output selection in terms of their audible effects.
- [ ] Describe physical-loop and virtual-block bypass behaviour, including any interaction with effect tails.
- [ ] Identify which routing and level settings belong to a preset and which are global.

## Building a Preset

### Your first preset

- [ ] Define a practical target sound and list the required pedals and connections.
- [ ] Show how to create or open a preset using the exact Houston screen and control names.
- [ ] Assign and reorder physical loops, then add and position a virtual effect.
- [ ] Set the levels and check the result with each effect active and bypassed.
- [ ] Name and save the preset, recall another preset, then return to verify that the intended settings were saved.
- [ ] Include screenshots at the key steps and a final signal-path diagram.

### Editing and managing presets

- [ ] Explain what saving captures, how unsaved changes are indicated, and what happens when another preset is recalled.
- [ ] Document the available rename, duplicate, organise and delete operations, including overwrite or confirmation behaviour.

## Playing Live

### Footswitches and LEDs

- [ ] Explain how to assign footswitches, the supported press/hold actions, and the meaning of each LED state.
- [ ] Walk through a useful assignment, such as bypassing a drive loop while keeping the rest of the preset active.

### Performance workflow

- [ ] Introduce the available performance views and demonstrate moving between sounds during a song.
- [ ] Explain preset ordering and any supported bank, song or setlist organisation with one short example.
- [ ] Describe what to expect during preset changes, including any audible transition or effect-tail behaviour.

### External control

- [ ] Show one expression assignment and explain its range and behaviour when presets change.
- [ ] Show how supported MIDI and CTRL actions are assigned and triggered; link to the [MIDI chapter](#midi) and relevant connection instructions.

## MIDI

### Connections and channel setup

- [ ] Show an external controller connected to Artemis MIDI IN and an external pedal connected to Artemis MIDI OUT, with a labelled wiring diagram.
- [ ] Explain where to set receive and transmit channels in Houston and on the connected equipment. Identify which settings are global or saved per preset.
- [ ] State which MIDI connections are supported by the documented software version, including USB MIDI only if implemented.

### Controlling Artemis from a MIDI controller

- [ ] Document supported incoming Program Change (PC) messages and their preset mapping, including the numbering convention shown by Houston and the controller.
- [ ] Document supported incoming Control Change (CC) messages and value ranges. Walk through one supported action, including assignment or MIDI learn if available, saving and testing.

### Controlling external MIDI pedals

- [ ] Show how to configure supported outgoing messages, their destination channels, and the preset or footswitch actions that trigger them.
- [ ] Walk through recalling an external pedal's preset, including any supported bank selection, message ordering or timing requirements.

### Clock, synchronisation and MIDI thru

- [ ] State whether MIDI clock can be sent or received, which functions follow it, and how the tempo source is selected where supported.
- [ ] Document whether incoming messages can be forwarded to MIDI OUT, including any filtering, merging or routing options. Explain how to avoid sending messages back into the same route.

### MIDI troubleshooting

- [ ] Add checks for no response, the wrong preset being recalled, unexpected parameter changes and duplicate messages: cable direction, channels, message numbers, values and forwarding settings.
- [ ] Describe any available MIDI activity indicators or monitoring tools and show how to test one message at a time.

Use the [MIDI implementation reference](#midi-implementation) for the complete list of supported messages and values.

## Digital Effects

### Using effects and models

- [ ] Explain the distinction between a virtual block and the effects running inside it.
- [ ] Show how to add, arrange, adjust and bypass the available digital effects.
- [ ] If model or impulse-response loading is supported, document the accepted formats, import steps and file-management behaviour.

### Levels and processing limits

- [ ] Explain digital input/output levels, clipping indicators and how to balance processed and analogue paths.
- [ ] Describe processing limits, overload indications and practical ways to reduce DSP load.
- [ ] Explain latency where it affects a user's routing choices, especially parallel paths.

### Effect reference

- [ ] Explain common controls once, using the names displayed in Houston.
- [ ] For each effect, give its purpose, distinctive controls, relevant limits and one useful example setting.
- [ ] Link to separate detailed parameter documentation where needed.

## Maintenance and Troubleshooting

### Updates

For the recommended update method, see [Wi-Fi Updates](#wi-fi-updates). To transfer an update from your computer, follow the USB instructions below.

- [ ] Document how to check the installed software version.
- [ ] Explain what to do if an update is interrupted or fails, using the verified recovery procedure.

#### USB Updates

1. Download the latest ArtemisOS update bundle to your PC or Mac from [trinity-labs.co.uk/downloads](https://trinity-labs.co.uk/downloads).
2. Connect Artemis to your computer using a USB cable. Open the **Updates** tab in Launchpad, select **USB**, and start the guided wizard.

   ![USB update page in Launchpad](assets/screenshots/usb_updates.png)

3. If prompted, delete a previously cached update bundle to make space for the new one.

   ![Remove a cached update bundle](assets/screenshots/delete_old_bundle.png)

4. Enable the USB connection when prompted. The **ARTEMIS** drive will appear on your computer.

   ![Enable the USB connection](assets/screenshots/enable_usb.png)

5. Copy the downloaded update bundle into the **Updates** folder on the **ARTEMIS** drive (`ARTEMIS/Updates`). Wait for the copy to finish.

   ![Copy the update bundle to the Updates folder](assets/screenshots/copy_update_to_artemis.png)

6. Safely eject the **ARTEMIS** drive from your computer, then continue in the wizard.

   ![Safely eject the ARTEMIS drive](assets/screenshots/eject.png)

7. Follow the remaining prompts to install the update.

   ![Finish the wizard and install the update](assets/screenshots/finish_update.png)

8. When installation is complete, reboot Artemis when prompted to finish the update.

### Backups and recovery

- [ ] Document the supported backup and restore methods, including what is and is not included.
- [ ] Explain any available reset procedure and exactly which settings or files it removes.

### Troubleshooting

Complete each row with checks in the order a user should try them.

| Symptom | Checks and resolution |
| --- | --- |
| No sound | TODO: Power, cables, input selection, routing, loop returns, mute and output levels. |
| One side of a stereo setup is silent | TODO: Left/right wiring, stereo loop returns and output routing. |
| Distortion or unexpected volume change | TODO: Signal levels, clipping, pads, mixing and preset settings. |
| Thin or hollow sound when mixing buses | TODO: Polarity, digital latency and parallel-path interaction. |
| Hum or noise | TODO: Cable, power and connected-equipment checks appropriate to the setup. |
| Footswitch or expression control does not respond | TODO: Assignments, connection compatibility and calibration. |
| MIDI or USB connection does not respond | TODO: Cables, host/device roles, supported functions and settings. |
| Changes disappear after switching presets | TODO: Save behaviour and preset/global settings. |

### Getting support

- [ ] Add the support contact and list useful information to provide: hardware/software versions, wiring, preset, reproduction steps and screenshots.

## Reference

### Specifications

#### Mechanical

| Item | Specification |
| --- | --- |
| Dimensions (W × D × H) | Approx. 25.5 × 14.5 × 5.5 cm (10.0 × 5.7 × 2.2 in) |
| Mass | Approx. 1.5 kg — to be confirmed |
| Enclosure | 2.5 mm bead-blasted, anodised aluminium |
| Side panels | 5 mm solid walnut |

#### Power, processing and controls

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

#### Audio and routing

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

#### Virtual block positions

| Position | Bus A | Bus B |
| --- | --- | --- |
| Pre | Before slot 1 | Before slot 1 |
| Mid | After slot 2, before slot 3 | After slot 1, before slot 2 |
| Post | After slot 5 | After slot 3 |

Slots are positions in the reordered chain, not fixed loop numbers. Bypassed loops still occupy their slots. Both Post positions are before the output bus swap and final stereo loop.

V1 and V2 can use the same position or different positions on either bus. When both use the same position, the signal passes through V1 followed by V2. Bypassing a virtual block keeps the signal on its analogue through-path.

#### Digital audio and switching performance

| Item | Specification |
| --- | --- |
| Sample rate | 48 kHz (32bit) |
| Reported round-trip latency per virtual block | 2.3 ms at 48 kHz, using 32 frames per period and 2 periods |
| Best-case switching time, analogue-only changes | Approx. 30 ms; test conditions to be documented |
| DSP/NAM preset switching time | Depends on the preset and DSP load; worst-case figure to be confirmed |

Round-trip latency describes audio passing through a virtual block. Preset switching time describes the transition between presets and is a separate measurement.

### MIDI implementation

- [ ] Add a table of supported messages, channels, value ranges and actions, including program changes, control changes and clock/thru behaviour where implemented.

### Compatibility

- [ ] Summarise confirmed expression pedal requirements, CTRL limits, USB host requirements and supported effect/model formats.
- [ ] Link to the relevant setup instructions and distinguish tested devices from general compatibility requirements.

### Glossary

- [ ] Define loop, send, return, bus, slot, virtual block, preset, bypass, polarity, TS and TRS using consistent terminology.
