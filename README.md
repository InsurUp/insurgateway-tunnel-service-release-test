[🇹🇷 TR](./README.tr.md)

<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset=".github/assets/insurup-logo-dark.svg"><img src=".github/assets/insurup-logo.svg" alt="InsurUp" width="360"></picture></p>

# InsurGateway Tunnel service `Test`

This repository holds no source code, only the signed InsurGateway Tunnel service pre-release files that InsurUp's release pipeline publishes.

> [!WARNING]
> These pre-releases are for InsurUp's own testing. Do not install them on customer machines. Use the stable repository: [InsurUp/insurgateway-tunnel-service-release](https://github.com/InsurUp/insurgateway-tunnel-service-release).

## Integrity

Each package (`.zip`, `.tar.gz`) has a `.sig`, an ECDSA P-256 signature that the updater verifies before it applies the package, and a `.sha256`.

<details>
<summary>Check the SHA-256 by hand</summary>

Files in the same folder. The hash values must match.

### Windows

```powershell
(Get-FileHash .\igw-tunnel-win-x64.zip -Algorithm SHA256).Hash
Get-Content .\igw-tunnel-win-x64.zip.sha256
```

### Linux

```sh
sha256sum -c igw-tunnel-linux-x64.tar.gz.sha256
```

### macOS

```sh
shasum -a 256 -c igw-tunnel-osx-arm64.tar.gz.sha256
```

</details>

## Contact

https://www.insurup.com
