# UniXNU-sm8850-common

Shared SM8850 (Snapdragon 8 Elite Gen 5, "canoe"/"kaanapali") platform support for UniXNU.
Board peripherals, firmware selection, partition layout and power policy live in the device
repository (`UniXNU-pma120` for the OPPO Find X9 Ultra).

## Scope

- SoC facts: `soc.toml`
- Kernel configuration fragment: `configs/sm8850.config`
- SoC device tree include: `dts/sm8850.dtsi`
- XNU SoC patch series: `patches/xnu/series`
- SoC platform kits: `kits/`

## Status (2026-11-07)

Skeleton only. Pending: SM8850 XNU SoC patches, device tree include from mainline kaanapali,
Adreno 840 / UFS platform components.

## References

- Hardware facts (GIC bases, CPU topology, panel, memory map): `X9U-iOS移植/设备情报.md`
- Upstream mainline: [Xlie-Electronic-Customs/linux](https://github.com/Xlie-Electronic-Customs/linux),
  [Codelinaro kernel-qcom (kaanapali)](https://git.codelinaro.org/clo/linux-kernel/kernel-qcom/-/tree/kaanapali)
