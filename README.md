# unixnu-ums9621

UniXNU SoC feed for the Unisoc UMS9621 (Rongyue E5 e-reader): 8x Cortex-A53,
GICv3 at 0x12000000 (GICD 0x20000 / GICR 0x12040000 0x100000, stride 0x20000),
PSCI 0.2 via SMC, 26 MHz generic timer (CNTFRQ measured on hardware).

The DTS mirrors the shape the UniXNU `ArmCpu` driver was verified with
(`UniXNU/UniXNU-sm8550-common`): `unixnu,adt-name = "intc"` exposes the GIC in
the generated ADT.

Used by the device repository `Enceka/UniXNU-e5` (board: Rongyue E5).
