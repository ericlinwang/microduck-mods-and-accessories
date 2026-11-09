![Microduck mods workshop: a robot duck surrounded by a sensor board, backpack mount, roller feet and docking base](https://microduck-mods-gallery.niftycucumber1.chatgpt.site/assets/github-header.jpg)

# Awesome Microduck Mods & Accessories

**English** · [简体中文](README.zh-CN.md)

## Visual Gallery

Browse the projects as a visual catalog:  
[Open Microduck Mods Gallery →](https://microduck-mods-gallery.niftycucumber1.chatgpt.site)

> A curated directory of Microduck robot mods and accessories: 3D-printed parts, charging docks, tactile sensors, controller ports and DIY builds.

Microduck is the biped robot from Pollen Robotics and Hugging Face. Around it, community builders are doing more than writing new moves: fitting roller skates, mounting extra compute, making touch-sensitive head covers, and rebuilding the robot around different motors and electronics. Each of those changes can leave behind useful designs, code and lessons from the workbench.

This collection starts with the part of the duck you want to change. Its eight categories cover individual accessories, modifications inside larger replica projects, and the software needed to run replacement hardware. You might come looking for a calibration tray, or to compare several controller platforms. The aim is to help DIY builders find something they can make, and robotics developers find a useful starting point or a potential collaborator.

The directory currently contains **45 projects**. Each entry explains the purpose, the available materials and the key development milestone, then links to the author's own project. It should be clear whether the next step is downloading a model, following a build guide, studying code or watching an experiment develop. Projects are listed once, under their primary use.

This is an independent community collection, unaffiliated with Pollen Robotics or Hugging Face. Linked projects belong to their authors; code, CAD, models and images retain their own licenses. The header is a concept illustration, not a set of validated accessory designs.

## Contents

- [Visual Gallery](#visual-gallery)
- [Ecosystem Status](#ecosystem-status)
- [Appearance](#appearance)
- [Mounts](#mounts)
- [Motion Accessories](#motion-accessories)
- [Power Systems](#power-systems)
- [Sensors](#sensors)
- [Electronics](#electronics)
- [Mechanical Design](#mechanical-design)
- [Assembly Tools](#assembly-tools)
- [Contributing](#contributing)
- [Related Resources](#related-resources)

## Ecosystem Status

These observations reflect the **45 projects in this directory as of 9 November 2026**. They show a community building and testing as it goes: some modifications have reached physical robots, while others explore new structures, controller platforms and ways to interact.

**Many accessories grow out of full replica builds.** Choosing different motors, a computer or a battery creates work elsewhere: connection boards, internal space, feet and calibration fixtures may all need to change. [Microduck-kissqy](https://github.com/kissqy/Microduck-kissqy) includes replaceable feet and revised leg supports; [CMU Microduck](https://github.com/qilinxiaoxiang/cmu-microduck) documents changes to head covers, ankles, cable clips and electronics mounts. A full-build repository can therefore be a useful source of individual parts, with a practical assembly problem behind each change.

**There are physical examples to learn from.** [microduck-tools](https://github.com/jackwuwei/microduck-tools) publishes both printable calibration-tray files and photographs of the tray in use. [FabricTouch](https://github.com/JoyrayGu/Microduck-FabricTouch) records touch input turning into joint movement, and several replica projects show walking prototypes. These materials help connect a design to the work of making it. Reuse still depends on the build: a board that fits one body, or a calibration pose for one motor, may need adjustment on another duck.

**New capabilities are driving broader system experiments.** Automatic charging needs a dock, localization, motion control and an electrical connection to work together. [duckmind](https://github.com/joseyarashio/duckmind) and [Gonzalo Duck](https://github.com/ggoonnzzaallo/gonzalo_duck) publish designs and simulation experiments, but have not demonstrated a complete physical auto-charging cycle. Controller replacements have their own stages: [esp-duck](https://github.com/xingxingRealzyx/esp-duck) runs models on a real small board, while [spacemit-microduck](https://github.com/fivif/spacemit-microduck) uses development boards to control a simulated duck. Those are useful foundations; real motors, power delivery and whole-robot tests remain further steps.

**What is published determines where you can pick up the work.** Some projects include editable CAD and printable files; others share circuits and firmware, or only photographs, interfaces and instructions. Entries distinguish the available materials from the validation stage. Hardware results are the authors' published reports, not independent assembly tests by this directory. Follow the original source for version-specific manufacturing files, build instructions and licenses.

## Appearance

A different look for Microduck: themed shells, colors, clothing and decorative parts. Design-only work is included when its digital and physical validation boundaries are explicit.

- **[Microduck Color and Sticker Console](https://github.com/lucienxxxxxx/microduck-console)** (lucienxxxxxx) — A browser-based preview tool for trying colors and preset stickers on individual body parts before making the modification. It does not manufacture a part. The console code is MIT; the official meshes and assembly data retain their CC BY-NC-SA non-commercial terms.

- **[Gritty-Themed Microduck](https://github.com/maddiedreese/gritty-microduck)** (maddiedreese) — An editable orange-shag, googly-eye and hockey-sweater costume concept with two reproducible MuJoCo performances. The fur and clothing are massless, non-colliding visual geometry. No physical garment or hardware validation has been completed.

## Mounts

A place for the duck to carry equipment or other objects. Mounting geometry and the effect of the added weight both matter.

- **[microduck-jetson-mount](https://github.com/adammong/microduck-jetson-mount)** (adammong) — A mount for carrying a Jetson computer and external battery on Microduck, giving extra onboard AI compute somewhere to live. Publishes adjustable CAD, printable parts and MuJoCo models of the loaded robot. Physical installation has not been validated, and some simulation checks still fail.

## Motion Accessories

From a change of feet to stilts and swings, these projects connect printable attachments with new ways for the duck to move.

- **[Microduck Playground](https://github.com/Vottivott/microduck-playground)** (Vottivott) — A collection of movement experiments around swings, stilts, climbing ladders and other props, with accessory models and simulation material. A printed stilt is shown; physical progress varies by experiment. The repository also includes the MicroDock charging-dock concept, currently at the design and simulation stage with no demonstrated physical charging.

- **[Microduck-kissqy](https://github.com/kissqy/Microduck-kissqy)** (kissqy) — An HD1910 replica route with revised foot attachments, leg supports and supporting electronics, including the option to switch between ordinary feet and roller skates. The skates use the official design. Hardware material is available; movements need to be matched to the particular mechanical and software version.

## Power Systems

Supplying power and finding a way back to the charger. Both dock projects below study the hardware alongside docking behavior; neither currently provides a complete solution validated through physical charging.

- **[duckmind](https://github.com/joseyarashio/duckmind)** (joseyarashio) — Explores a low-battery routine in which Microduck finds its dock, aligns, backs into position and sits down to charge. The dock and behavior are modeled together, with published [dock hardware specifications](https://github.com/joseyarashio/duckmind/blob/HEAD/docs/dock-hardware.md). Charging currently means a change in the simulated battery state; physical charging remains unverified.

- **[Gonzalo Duck](https://github.com/ggoonnzzaallo/gonzalo_duck)** (ggoonnzzaallo) — Develops charging as separate steps: finding the dock, approaching, making contact, monitoring charge and leaving. The [charging plan](https://github.com/ggoonnzzaallo/gonzalo_duck/blob/HEAD/docs/charging-plan.md), 3D simulation and manual docking experiments show how the dock and controller could work together. Autonomous docking, real charging conditions and production-robot fit still need validation.

## Sensors

Knowing where the duck was touched, or which way its body is leaning. Touch sensors support interaction; an inertial measurement unit, or IMU, supplies motion and orientation data to the controller.

- **[microduck_imu_to_ttl](https://github.com/avanx/microduck_imu_to_ttl)** (avanx) — A sensor board and firmware for replica builders, bringing LSM6DSV16X IMU readings onto a motor communication bus. The PCB has powered up and the Feetech communication firmware has been debugged from a computer. Integration with a physical duck and Dynamixel communication support remain unfinished.

- **[imu-displace-microduck](https://github.com/Juxi-Technology/imu-displace-microduck)** (Juxi Technology) — A guide to replacing the body IMU in an HD1910 build with an ICM-42670-P, with wiring instructions, software patches and a companion [sensor-module project](https://github.com/Juxi-Technology/ICM42670P-High-Precision-IMU-Module). Readings from real hardware have been verified; completing their integration into the robot controller is the next step.

- **[Microduck FabricTouch](https://github.com/JoyrayGu/Microduck-FabricTouch)** (JoyrayGu) — A pressure-sensitive fabric “scalp” that turns taps and strokes into responses such as head tilts or beak movement. Publishes signal capture, gesture recognition and motor-control implementations, with physical touch-response records. Processing currently involves a computer; multi-finger recognition and neck control still have limitations.

- **[my-microduck](https://github.com/ReadbytheBeach/my-microduck)** (ReadbytheBeach) — Plans four 12×12 pressure arrays across Microduck's head and soles, using the head for touch interaction and the feet for ground-contact sensing. The repository describes scanning circuitry and communication integration. It is a design-stage project, without evidence of a complete physical deployment of the electronic skin.

- **[LSM6DSV16X Bare-IMU Compatibility Library](https://github.com/sim336/lsm6dsv16x-sflp)** (sim336) — Lets a Linux controller read the orientation chip directly over I²C and emit the same 12-byte data block as the existing MCU carrier. Tests cover silent register, scaling and mounting failures. Measurements come from one Radxa board, so each board and physical mounting still needs its own verification.

## Electronics

Changing a controller or a joint motor often means changing wiring and software as well. This section covers replica connection boards, alternative electronics and the work of running Microduck models on different computing platforms.

- **[microduck-community-kit](https://github.com/jyg9/microduck-community-kit)** (jyg9) — Collects several boards needed for a replica: an IMU board reads body tilt, a battery adapter connects the battery, and a hub brings motor wiring together. Covers HD1910 and XL330 routes, with wiring diagrams, firmware, debugging tools and a board-purchase link. The author reports batch validation; full robot assembly still needs additional guidance.

- **[microduck-replica](https://github.com/fanhao375/microduck-replica)** (fanhao375) — Brings mechanical models, internal electronics and firmware into one replica reference. Its [hardware materials](https://github.com/fanhao375/microduck-replica/blob/HEAD/hardware/README.md) include IMU, distribution and battery-interface boards for XL330 and HD1910 routes. The author shows an HD1910 robot moving; the manufacturing and test status of newer board revisions should be checked individually.

- **[Fanduck](https://github.com/7757/fanduck)** (7757) — A replica project containing the [DCHUB four-port motor distribution board](https://github.com/7757/fanduck/blob/HEAD/hardware/dchub-v1.1/README.md), a small internal junction for the head and leg motor wiring. Editable circuits, fabrication files and a bill of materials are published for builders making their own board. Connector pinouts and power conditions must match the intended build.

- **[Dukki](https://github.com/lachlanhurst/dukki)** (lachlanhurst) — Reworks the duck's computer and joint motors around a Radxa CM4 and Unitree J288 servos, with custom connecting electronics and firmware. The author is seeking more compute headroom and exploring a different set of motor tradeoffs. Circuit projects and STM32 communication firmware are available; the whole robot is still in development.

- **[DuckBuddy](https://github.com/Animan-AI/DuckBuddy)** (Animan-AI) — Combines speech, movement and autonomous behavior into a companion experience on custom hardware, including executing a spoken sequence of actions. Its expansion board connects audio, power and motors. A physical voice-to-action demonstration is published; some vision and autonomous tasks remain under test. Interface documentation is public, but PCB manufacturing designs are not.

- **[Microduck Companion Project](https://github.com/RomdhoniZidane20/Microduck_companion_project)** (RomdhoniZidane20) — A Raspberry Pi 4 replica plan that proposes shrinking a reference Dynamixel interface board to fit the chosen body. Publishes technical planning and circuit references for arranging the electronics inside a small robot. Fabrication and physical results for the custom smaller board have not been confirmed.

- **[microduck-opi3w](https://github.com/Jimzjy/microduck-opi3w)** (Jimzjy) — Adapts Microduck to an A733-based Orange Pi Zero 3W and HD1910 motors, adjusting the expansion board, wiring and runtime. Circuit designs, IMU firmware and deployment notes provide a starting point for this component combination. The mainboard boots; walking still awaits full assembly and validation.

- **[esp-duck](https://github.com/xingxingRealzyx/esp-duck)** (xingxingRealzyx) — Investigates whether an ESP32-S3 can handle Microduck's motion inference. Nine converted policies share one firmware image and can be switched at runtime, with checks for numerical accuracy, execution speed and real IMU input. This is currently a board-level experiment; motor communication and joint feedback are not yet fully connected.

- **[spacemit-microduck](https://github.com/fivif/spacemit-microduck)** (fivif) — Ports the Microduck runtime to SpacemiT K3 and K1 development boards, exploring a RISC-V controller route. Both real boards have records of controlling a MuJoCo duck; K1 also has a camera-to-browser pipeline. The work offers porting and performance references, rather than a completed controller swap in a physical robot.

- **[microduck-imx6ull](https://github.com/TonyRuan/microduck-imx6ull)** (TonyRuan) — Runs motion calculations on an i.MX6ULL board and connects it to a MuJoCo duck on a Mac to test the control loop. Publishes model-to-C conversion, timing measurements and keyboard control. Real motors and physical sensors have not been validated, and some movements remain unstable.

- **[ArduPilot Neural Mixer](https://github.com/virtualrobotix/Ardupilot-Neural-Mixer)** (virtualrobotix) — Puts learned motion models inside ArduPilot firmware to explore controlling a biped using a flight controller's compute, sensors and radio inputs. Microduck is one reference robot. Simulation and Pixhawk 6C Mini hardware-in-the-loop tests are documented; independent physical operation still needs motor-bus communication and joint-feedback support.

- **[RDK X5 Microduck](https://github.com/Xiaomiju-x/rdk-x5-microduck)** (Xiaomiju-x) — Follows an RDK X5-based duck from sourcing and printing through assembly, wiring and physical debugging. An older dual-battery prototype moves forward briefly using action sequences; the newer single-supply layout boots and stands. Load-bearing power delivery and reinforcement-learning control remain in progress, with the different configurations documented separately.

- **[Xbotics MiniDuck Course](https://github.com/Xbotics-Embodied-AI-club/Xbotics-MiniDuck-Course)** (Xbotics) — A replica course built around custom boards, a battery and HD1910 motors, linking hardware versions to firmware, motion models, training code and flashing materials. Useful for following the author's integrated build-and-training route. Whether the PCB manufacturing files are fully public still needs confirmation.

- **[microduck-hd1910m](https://github.com/zhuoligetu123/microduck-hd1910m)** (zhuoligetu123) — Adapts runtime and training software to a Radxa ZERO 3W, HD1910M motors and BNO08x IMU, with wiring material and an Android controller. Explains how motor IDs, direction and zero positions correspond. Some movements still have heading drift or recovery problems; simulation demonstrations need to be distinguished from physical results.

- **[duck-a733](https://github.com/weilan157/duck-a733)** (weilan157) — Builds an SD-card system image for the A733 route, packaging the bootable system and robot application at specified versions. Reduces the work of compiling, installing and assembling compatible software versions. It is supporting software for a hardware modification; wiring, joint calibration and movement testing still belong to the corresponding robot build.

- **[Radxa ZERO 3W Robot HAT](https://github.com/juper007/radxa-zero3w-robot-hat)** (juper007) — A compact expansion board for fifteen XL330 servos, the body IMU, I²C sensors, microphone, speaker and protected 5 V power. KiCad projects, Gerbers, BOM and bring-up tools are available. V1 is still under power and high-current layout review and has not been fabrication-approved.

- **[Duck King S288 Conversion](https://github.com/zhanma666/Xihack2026_The_Duck_King)** (zhanma666) — Replaces XL330 joints with Unitree S288 servos and supplies a rebuilt MuJoCo model, joint mapping, setup script and training task. Actuator values are still placeholders, the BAM model is missing and passive standing falls forward. Training integration is therefore not evidence of a working physical S288 duck.

## Mechanical Design

Making the body fit a different component, manufacturing method or scale. Some projects address local assembly problems; others redesign the whole structure.

- **[MICDUCK_FTHD1901_REBUILD](https://github.com/fengj4780-sudo/MICDUCK_FTHD1901_REBUILD)** (fengj4780-sudo) — Revises motor connections and adds five optional reinforcement parts to address flexible replica parts and assembly interference. Publishes 3MF and SolidWorks files, aiming for stronger connections and easier assembly. CNC reinforcements are still being prototyped; motor compatibility should be checked against the actual drawings, not just the repository name.

- **[MicroDuck BoBoRedesign](https://github.com/AiBoBoMaker/MicroDuck-BoBoRedesign)** (AiBoBoMaker) — Keeps the familiar Microduck appearance while adapting factory-oriented parts for personal 3D printing, with supporting expansion boards, IMU boards and code. Covers XL330 and HD1910 routes and builds on upstream community work. A reference for printable construction and assembly; physical progress varies by revision.

- **[microduck-original-look-v2](https://github.com/zhoudongT/microduck-original-look-v2)** (zhoudongT) — Attempts a Microduck with twice the external dimensions, redesigning motor clamps, output brackets and adapters so real components fit the larger body. STEP designs and assembly checks are published. Physical validation and some linkage adaptation remain unfinished, making it a structural starting point for a larger build.

- **[microduck-s288](https://github.com/zheflow/microduck-s288)** (zheflow) — Rearranges the body around alternative motors, a mainboard and a battery, designing shells, internal mounts and flexible soles together. Publishes CAD-generation source for studying how component changes affect structure. The author has not completed assembly and explicitly advises against buying parts or printing the current version as a ready build.

- **[CMU Microduck](https://github.com/qilinxiaoxiang/cmu-microduck)** (qilinxiaoxiang) — Changes head covers, ankles, soles, cable clips and electronics enclosures on an A7Z/OpenRB replica, with touch sensing that detects a grip on the head. Parts lists and physical walking and touch records show the modifications in a complete build. The battery backpack has been designed but is not installed.

- **[MicroDinosaur](https://github.com/eugenewang5425/MicroDinosaur)** (eugenewang5425) — Reworks Microduck into an S288-powered small biped dinosaur. Publishes the current Blender assembly, a 30-part print project, a three-piece calibration fixture, a six-layer head board and dual-bus software. The head board is not fabricated and the complete robot has not been assembled, stood or walked.

- **[DuckLite](https://github.com/charlie8612/DuckLite)** (charlie8612) — A low-cost open-hardware redesign targeting a roughly US$150, 22 cm vision biped while keeping Microduck's 50 Hz control and ONNX policy interfaces. Mechanical, electronics, firmware and simulation workspaces are organized, but the project remains at architecture and component-selection stage; its next milestone is a one-leg actuator bench.

- **[Micro Cat](https://github.com/hwkim3330/micro-cat)** (hwkim3330) — An independent cat-shaped biped that keeps the 61-input/14-output Microduck policy interface while redesigning the head, ears, tail, feet and internal layout. CAD checks cover print volume, static interference and balance. No physical printing, assembly, walking or durability test has been completed.

- **[HL-2909 Servo Print Set](https://github.com/MenciousL/microduck-hl2909-print)** (MenciousL) — Provides four fit coupons and 39 printable body parts for replacing XL330 joints with Feetech HL-2909 servos. It is a drawing-validation release: builders should test the coupons first. Power is not adapted, because HL-2909 servos require 9–14 V and add roughly 67 g across fifteen joints.

- **[Microduck × Stack-chan](https://github.com/meganetaaan/microduck-stackchan)** (meganetaaan) — Combines a portrait M5Stack Tab5 head with Microduck legs, including assembly geometry, a provisional BOM, trained arm-free gaits and a browser simulator. The thin-arm version is visual only and has not been included in mass, collisions or retraining. Physical wiring, strength and safety remain unverified.

- **[IndieDuck Cyber Edition](https://github.com/armature-ai-labs/indieduck)** (Armature AI Labs) — Organizes editable FreeCAD/STEP/STL, 55 printed parts, a BOM and an interactive assembly guide around one mechanism with interchangeable exteriors. The R25 steps are CAD-reviewed rather than physically verified; wiring, strength, sensors, power and trained locomotion are still open work.

## Assembly Tools

Holding the body steady and placing joints in a known pose. These tools help with assembly and zero calibration so the controller's joint positions correspond to the physical robot.

- **[microduck-tools](https://github.com/jackwuwei/microduck-tools)** (jackwuwei) — Pairs a motor-calibration workbench with a printable tray: the tray supports the head, body and feet while the software connects to motors, checks them and sets zero positions. STEP, STL and photographs of actual use are available. Designed for XL330-M288-T motors and the author's calibration pose.

- **[JIG-190](https://github.com/superobk/microduck-cad)** (superobk) — A static support that holds Microduck during assembly, inspection and calibration, leaving both hands free for joints and wiring. The [R5 design folder](https://github.com/superobk/microduck-cad/tree/HEAD/projects/microduck-stand/r5-compact-full15) contains STL, 3MF and assembly illustrations. R5.0-rc1 still awaits slicing and physical fit checks; motor calibration needs separate software.

- **[MHDuck](https://github.com/MHDuck/microduck)** (MHDuck) — A [zero-calibration reference](https://github.com/MHDuck/microduck/blob/master/%E6%A0%A1%E5%87%86.md) within the HD1910/BNO085 replica route, showing how a fixture supports and positions the body before joint setup. Runtime code, policy files and a [training repository](https://github.com/MHDuck/microduck_rl) are public. The fixture can be studied through photographs and instructions; printable design files have not been found.

- **[Wamoduck](https://github.com/Wamotech/Wamoduck)** (Wamotech) — A [standing-zero calibration fixture](https://github.com/Wamotech/Wamoduck/tree/HEAD/hardware/fixtures/standing-zero) for the author's redesigned robot, using four printed parts to hold a consistent reference pose. STEP, STL and print-project files are published. Physical fit status is unconfirmed; it targets the Wamoduck structure, with no verified fit for an official retail duck.

- **[Microduck Servo Bench Tools](https://github.com/masszhou/microduck-notes)** (masszhou) — A DSH web dashboard and Mac command-line bench for finding, inspecting, centering and carefully moving fifteen XL330 servos before full assembly. It records position, current, temperature and bus errors with explicit safety limits. Encoder center is a bench reference, not the assembled robot's standing zero pose.

## Contributing

Suggestions, new projects and corrections are welcome. Include the original project link, author, suggested category, available materials and current validation stage. Design-only and simulation-only work can be included when clearly identified.

See the [contribution guidelines](CONTRIBUTING.md). Authors are welcome to submit their own work; please disclose authorship or any commercial relationship. Follow each linked project's license when reusing code, designs or images.

## Related Resources

- [Microduck official runtime](https://github.com/pollen-robotics/microduck) — The original controller, device interfaces and usage documentation.
- [Microduck official training environment](https://github.com/pollen-robotics/microduck_rl) — Motion-policy training and a starting point for adapting behavior to a different body, motor or foot contact.
- [Awesome Microduck](https://github.com/joeynyc/awesome-microduck) — A broader community directory covering software, simulation, policies and related resources. Its categorized-list format inspired this collection, whose focus is modifications and accessories.
