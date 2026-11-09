# Agent instructions

This repository owns shared SM8850 resources and platform operations.
Keep board peripherals, firmware selection, partition layout, and power
policy in the device repository (`UniXNU-pma120`). Preserve runtime source
filenames, classes, symbols, bundle IDs, and protocol IDs.

Read these UniXNU pages before editing:

1. [Porting](https://unixnu.com/porting/)
2. [Device repositories](https://unixnu.com/porting/device-repository)
3. [Components](https://unixnu.com/reference/components)
4. [Device trees](https://unixnu.com/porting/device-tree)

Inspect existing SM8550 support (`UniXNU-sm8550-common`) and the component
catalog before adding a capability. Select by interface, hardware scope, OS
ABI, and board dependencies.

Hardware facts for SM8850 (GIC bases, CPU topology, memory reservations) are
recorded in `X9U-iOS移植/设备情报.md`; verify additions against the phone's
own device tree (`device/PMA120/fdt.dtb`) before committing.

Run builds from the UniXNU checkout and report commands, results, required
inputs, and hardware checkpoints separately. Write concise English.
