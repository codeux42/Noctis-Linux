# Noctis Linux

Application bureau Noctis (Electron) pour Linux. Version **1.3.1**.

## Installer

Téléchargez l'un des installeurs de la release **v1.3.1** :

- `Noctis-1.3.1-x86_64.AppImage` (x64, portable)
- `Noctis-1.3.1-arm64.AppImage` (ARM64, portable)
- `Noctis-1.3.1-amd64.deb` (Debian/Ubuntu x64)
- `Noctis-1.3.1-arm64.deb` (Debian/Ubuntu ARM64)

```bash
chmod +x Noctis-1.3.1-x86_64.AppImage
./Noctis-1.3.1-x86_64.AppImage
```

## Build

```bash
npm ci
npx electron-builder --linux --x64 --arm64 --publish never
```

Le workflow GitHub Actions `.github/workflows/release.yml` construit les installeurs et les publie dans la release `v1.3.1`. Un poussage de tag `build-1.3.1` déclenche le build.
