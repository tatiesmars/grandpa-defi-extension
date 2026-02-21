# Grandpa DeFi Chrome Extension

This repository contains compiled builds of the Grandpa DeFi browser extension.
It does not contain source code.

## Download

Build artifacts are published in the `/builds` directory of this repository.

- For the latest version, download the highest semantic version build from `/builds`.
- Download a specific version from `/builds` when needed.
- If GitHub Releases are used in the future, artifacts may also appear in the Releases tab.

## Install (Manual – Developer Mode)

1. Download the desired version zip from `/builds`.
2. Unzip it.
3. Open Chrome and go to `chrome://extensions/`.
4. Enable `Developer mode`.
5. Click `Load unpacked`.
6. Select the unzipped folder.

## Verify Integrity (Optional)

Compare the SHA256 hash of your downloaded zip with the value in `/builds/SHA256SUMS.txt`.

macOS/Linux:

```sh
shasum -a 256 chrome-extension-vX.Y.Z.zip
```

Windows:

```powershell
certutil -hashfile chrome-extension-vX.Y.Z.zip SHA256
```

## Security

- Extension code is inspectable after extraction.
- Only download builds from this official repository.

## Updates

Updates are manual in this distribution model. To update, download a newer build from `/builds` and reinstall it. Automatic updates are not available unless distribution moves to the Chrome Web Store.
