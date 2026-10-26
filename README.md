# Artemis User Manual

> **Drafting guide:** Work through the unchecked items below, replacing each with finished instructions and illustrations. For walkthroughs, include the starting setup, exact Houston actions, expected result, and what needs saving. Document features available in the manual's stated software version. Remove this guide and remaining drafting prompts before publication.

## Table of Contents

- [Introduction](#introduction)
- [Houston](#houston)
  - [Houston Home Screen](#houston-home-screen)
  - [My Pedalboard](#my-pedalboard)
  - [Presets, Songs and Setlists](#presets-songs-and-setlists)
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

## Houston

When you have finished setup and any update has completed, open the **Apps** tab in Launchpad. Find **Houston** and tap the orange play button to launch it.

### Houston Home Screen

The screen below shows Houston's Home screen, this is a handy pop up that takes you to the most important places in Houston. You can access the home pop-up at any time by breifly pressing the *tl* logo  button on the left hand corner of the artemis. 

![Houston Home screen](assets/screenshots/home_screen.png)

 The following sections introduce the main areas of Houston; when you are ready to connect your instrument and get your first sound, follow [Quick Start](#quick-start).

### My Pedalboard

My Pedalboard tells Artemis which pedals are connected to each physical loop. The names and colours you choose help you recognise those pedals in the Preset Editor. Set up My Pedalboard when you first open Houston, before building your presets.

**Setup order:** check your connections → choose a pedalboard configuration → add pedals to the library → assign them to the matching loops → check the result before building a preset.

#### 1. Check your physical connections

Start with the pedals connected to Artemis and make a note of which loop each pedal uses. See [Connections](#connections) for send/return wiring and [Routing Basics](#routing-basics) for signal-path options.

**Plan your loop connections before setup:** L1–L3 can be assigned to either Bus A or Bus B; L4–L5 are restricted to Bus A. Connect any pedal you need on Bus B to L1, L2 or L3. L6/L7 form the fixed stereo loop.

The walkthrough uses the following physical setup:

![Physical pedalboard used for the walkthrough](assets/images/physical_setup.jpg)

| Artemis loop | Connected pedal | Name used in My Pedalboard |
| --- | --- | --- |
| L1 | BOSS OC-2 | OC-2 |
| L2 | Ibanez TS9 | TUBE SCREAMER |
| L3 | BOSS DS-2 | DS-2 |
| L4–L5 | Unused | Leave empty |
| L6/L7 | BOSS CE-20, connected in stereo | CE-20 in both L6 and L7 |

#### 2. Open My Pedalboard and choose a configuration

Open **My Pedalboard** using the shortcut in the Home pop-up. Alternatively, tap the **Home** icon in the top navigation bar to open the home carousel, find **My Pedalboard**, and tap **Edit**.

Choose the pedalboard configuration you want to set up using the numbered selector in the navigation bar. You can keep separate configurations for different physical pedalboards, such as boards you use with different bands. This walkthrough uses **My Pedalboard 1**.

On first setup, the loop slots are empty:

![My Pedalboard 1 with empty loop slots](assets/screenshots/empty_my_pedalboard.png)

#### 3. Add your pedals to the library

Create one library entry for each pedal in the example:

1. Drag the library drawer up from the bottom of the screen and tap **+ Add Pedal**. You can also begin by tapping an empty pedal slot.
2. Enter a **Pedal Name**, then choose a **Category** and **Colour**. Use a name and colour that make the pedal easy to recognise.
3. Tap **Add** to add the pedal to your library.
4. Repeat for the remaining pedals. Create the stereo CE-20 entry once; you will use it in both L6 and L7.

![New pedal dialog with Pedal Name, Category, Colour and Add controls](assets/screenshots/create_a_new_pedal.png)

Your library should now contain OC-2, TUBE SCREAMER, DS-2 and CE-20. The order in the library does not determine their loop assignments.

![Pedal library containing the four example pedals](assets/screenshots/populate_mypedalboard_library.png)

#### 4. Assign pedals to the matching loops

Drag each pedal from the library into the slot that matches its physical connection:

1. Drag **OC-2** into **L1**.
2. Drag **TUBE SCREAMER** into **L2**.
3. Drag **DS-2** into **L3**.
4. Leave **L4** and **L5** empty.
5. Drag **CE-20** into **L6**, then drag the same library entry into **L7** to represent both stereo channels.

**Match the physical loop numbers here.** You will choose the order in which effects process your signal later in the Preset Editor. The pedal names and colours help identify each effect.

![Completed My Pedalboard with OC-2 in L1, TUBE SCREAMER in L2, DS-2 in L3 and CE-20 in L6 and L7](assets/screenshots/fully_setup_mypedalboard.png)

#### 5. Check your setup and continue

Compare the on-screen assignments with the cables connected to Artemis. For this example, L1–L3 should contain the three mono pedals, L4–L5 should be empty, and CE-20 should appear in both L6 and L7.

If you also use MIDI-controlled pedals, see [MIDI Librarian](#midi-librarian) for instructions on finding your devices in the MIDI library and adding them to the current pedalboard configuration.

Once your pedalboard setup is complete, continue to [Quick Start](#quick-start) to get your first sound, or [Building a Preset](#building-a-preset) to arrange your effects and create your first preset.

### Presets, Songs and Setlists


## Quick Start

### Before you begin

- [ ] List the supplied items and the cables, instrument, pedal and amplifier needed for the walkthrough.
- [ ] Explain the power requirements and essential connection precautions before first use.

### First-time setup

Follow [Launchpad Basics](#launchpad-basics) for initial setup, then [open Houston](#houston). Before building a preset, use [My Pedalboard](#my-pedalboard) to match the on-screen pedals to your physical connections.

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
Artemis supports MIDI In, Out, Thru, as well as Clock - allowing it to exist in a chain of midi capable devices - either as master, slave, or somewhere in-between.

### Connections and channel setup

- [ ] Show an external controller connected to Artemis MIDI IN and an external pedal connected to Artemis MIDI OUT, with a labelled wiring diagram.

Artemis contains a publically available MIDI librarian (https://github.com/Morningstar-Engineering/openmidi - you can submit any missing devices from https://www.openmidi.com/), which allows you to set which MIDI capable devices are connected to your Artemis per Pedalboard configuration:

1. Simply click Edit on the My Pedalboard slide of the Carousel
2. Then click the blue MIDI button in the Navbar to open the MIDI Devices Configuration Page ![](assets/screenshots/midi/midi-devices.png)
# NOTE: MAKE TEXT MUCH LARGER ON THIS PAGE

#### MIDI Librarian

Clicking on the red Library button will open the MIDI Librarian, which is a searchable library of MIDI capable devices and their functions ![](assets/screenshots/midi/midi-librarian.png)

You can favourite any that you want to use with Artemis (seeing only these quickly through the yellow Star button in the Navbar), as well as assigning them to specific MIDI channels, which allows you to easily assign MIDI messages to them from a Preset or MIDI Utility.

You can add a device to the current board by clicking the orange Plus button in the top right corner of the Navbar

#### Supported MIDI Connection Types
At the moment, Artemis only supports MIDI through standard 5-pin DIN connectors, although we plan to add USB MIDI at some point in the future.

### Controlling Artemis from a MIDI controller (MIDI In)

Controlling Artemis externally via MIDI is simple. Simply:
1. Plug the MIDI Out / Thru port on the MIDI Controller to the Artemis' MIDI In Port with a 5-pin MIDI DIN cable
2. Send messages from the Controller to the Artemis according to the mappings below

Artemis supports the following PC Messages into the device:

| PC | Function |
| --- | --- |
| 0 | Toggle Tuner |
| --- | --- |
| 1 | Switch to Preset 1 (Jam Page) |
| 2 | Switch to Preset 2 (Jam Page) |
| 3 | Switch to Preset 3 (Jam Page) |
| 4 | Switch to Preset 4 (Jam Page) |
| 5 | Switch to Preset 5 (Jam Page) |
| --- | --- |
| 6 | Immitate Pressing Footswitch 1 |
| 7 | Immitate Pressing Footswitch 2 |
| 8 | Immitate Pressing Footswitch 3 |
| 9 | Immitate Pressing Footswitch 4 |
| 10 | Immitate Pressing Footswitch 5 |
| --- | --- |
| 11 | Immitate Releasing Footswitch 1 |
| 12 | Immitate Releasing Footswitch 2 |
| 13 | Immitate Releasing Footswitch 3 |
| 14 | Immitate Releasing Footswitch 4 |
| 15 | Immitate Releasing Footswitch 5 |
| --- | --- |
| 123 | Go To Jam Page |
| 124 | Go To Preset Editor (Current Preset)|
| 125 | Go To Home / Settings Carousel |
| 126 | Go To Mixer |
| 127 | Save on Current Page |

![Artemis publishes these as a scrolable list:](assets/screenshots/midi/midi-mapping.png)

These (along with CC mappings for the device) are reachable from two places:
1. The Preferences slide in the Carousel![](assets/images/preferences-slide.png)
2. The MIDI Out section from the Preset Editor (SCREENSHOT REQUIRED)

Artemis also supports the following CC messages into the device:

| CC | Value | Function |
| --- | --- | --- |
| 0 | n | Set Currently Selected Parameter To n/127 (Virtual Loop Editor) |
| 1 | n | Load The n'th Preset On The Device
| 61 | n | Load the n'th Song On The Device
| 122 | n | Load the n'th Setlist On The Device

# NOTE - ANY FURTHER cc COMMANDS SHOULD BE MADE pc. Any invert menu function should also be added as pc

This means that Artemis supports:
- Up to 7,680 MIDI addressed Presets (CC 1 to 60, with value 0 to 127)
- Up to 7,680 MIDI addressed Songs (CC 61 to 121, with value 0 to 127)
- Up to 640 MIDI addressed Setlists (CC 122 to 127, with value 0 to 127) PENDING NOTE ABOVE

### Controlling external MIDI pedals (MIDI Out)

Using Artemis to control external MIDI devices is simple. Simply:
1. Plug the MIDI Out / Thru port on Artemis to the external Devices MIDI In Port with a 5-pin MIDI DIN cable
2. Send messages from Artemis to the external device according to the devices internal MIDI mapping

There are two main ways to send MIDI messages from Artemis:

1. From A Preset
- Simply tap the Blue MIDI button on the navbar in the Preset Editor (SCREENSHOT REQUIRED), then click the Send button to open that Presets Send Menu
- From the MIDI Send Table, you can send any number of MIDI messages (CC or PC) to connected devices by setting the channel, and message values
![](assets/screenshots/midi/midi-send-table.png)

2. From A MIDI Utility
- When adding a Preset on the Jam Page, simply tap the highlighted Preset title text to swap to viewing the available Utility Presets
- Then tap 'Add MIDI Utility' in the top right to create your MIDI only Jam Page Slot
![](assets/screenshots/midi/create-midi-utility.png)

You can use the arrow button to test these from this page before saving them to the Preset or Utility.

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
| Mass | Approx. 1.4 kg / 3lbs|
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
