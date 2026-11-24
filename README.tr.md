<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset=".github/assets/insurup-logo-dark.svg"><img src=".github/assets/insurup-logo.svg" alt="InsurUp" width="360"></picture></p>

# InsurGateway Tunnel service `Test`

Bu repoda kaynak kod yoktur, yalnızca InsurUp'ın yayın hattının yayımladığı imzalı InsurGateway Tunnel servisi ön sürüm (pre-release) dosyaları bulunur.

> [!WARNING]
> Bu ön sürümler InsurUp'ın kendi testleri içindir. Müşteri bilgisayarlarına kurmayın. Kararlı repoyu kullanın: [InsurUp/insurgateway-tunnel-service-release](https://github.com/InsurUp/insurgateway-tunnel-service-release).

## Bütünlük

Her paketin (`.zip`, `.tar.gz`) bir `.sig` dosyası (güncelleyicinin paketi uygulamadan önce doğruladığı ECDSA P-256 imzası) ve bir `.sha256` dosyası vardır.

<details>
<summary>SHA-256'yı elle denetle</summary>

Dosyalar aynı klasörde. Özet değerleri aynı olmalıdır.

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

## İletişim

https://www.insurup.com
