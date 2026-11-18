# Goldshell KD Box Recovery Firmware Research

Independent community research into the original Goldshell KD Box ASIC miner firmware, including reverse engineering, hardware configuration, recovery mechanisms, and community development.

## Recovery Firmware 2.2.3

| Property | Value |
|---|---|
| Manufacturer | Goldshell |
| Model | KD Box (original, non-Pro) |
| Firmware | 2.2.3 |
| Control Board | MCB_V5_4 |
| Firmware type | Recovery disk image |
| Format | IMG (partitioned disk image) |

**[Download Recovery Firmware Release v2.2.3](https://github.com/booozytheclown/goldshell-kdbox-firmware/releases/tag/recovery-2.2.3)**

This is a recovery image, **not** a normal firmware upgrade package. Use only an appropriate, documented recovery procedure for compatible original KD Box hardware; do not upload this `.img` through the regular firmware-update interface unless Goldshell explicitly instructs you to do so.

### SHA-256 Verification

Firmware: `burn-Goldshell-KDBox_MCB_V5_4-2.2.3.img`

Expected SHA-256:

`fe7238fc3f01ea4e913c22a61142ad5d4936d2438c12d4ab6b264872697c9314`

Linux verification (download both release assets to the same folder):

```bash
sha256sum -c burn-Goldshell-KDBox_MCB_V5_4-2.2.3.img.sha256
```

Windows PowerShell verification:

```powershell
Get-FileHash -LiteralPath ".\burn-Goldshell-KDBox_MCB_V5_4-2.2.3.img" -Algorithm SHA256
```

The checksum was computed from the uploaded image before publication. It establishes integrity relative to that image, **not** independent manufacturer authenticity.

## Research Objectives

- Preserve a copy of the original KD Box recovery image for community access.
- Document the embedded Linux filesystem and firmware architecture.
- Investigate firmware validation, signing, recovery, and compatibility.
- Share reproducible technical findings and encourage community development.

## Contributing

Community contributions are welcome!

Use GitHub Issues to document firmware behavior or propose improvements, and Pull Requests for research documentation and independently developed tools.

Please avoid publishing passwords, private keys, device credentials, or personally identifiable information.

## Disclaimer

This project is independent and is not affiliated with or endorsed by Goldshell.

Original firmware and manufacturer documentation remain subject to their respective intellectual property rights.

Flashing or recovering firmware carries risks, including hardware damage and device failure. Use appropriate safeguards and confirm hardware compatibility first.

This repository does not guarantee firmware safety, authenticity, or suitability for production hardware.
