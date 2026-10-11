# Dawn Engine Releases

Official public downloads for Dawn Engine and Dawn Hub.

## Downloading builds

Published versions use GitHub Releases with version tags such as `26.1.1`, `26.1.2`, and `26.1.3`. Dawn Hub reads published releases from this repository and can download/install a Windows x64 ZIP automatically.

## Publishing a Windows editor build

1. Build the matching Dawn Engine version from the private `APGSwizzVR/DawnEngine` source repository.
2. Package the Windows x64 runtime as a ZIP. The ZIP must contain `DawnEditor.exe` and every required runtime/DLL file. `DawnEditor.exe` may be in a subfolder; Dawn Hub locates it and installs that folder.
3. Create a GitHub Release in this repository with a matching version tag, for example `26.1.1`.
4. Attach the ZIP as a release asset. Use a clear asset name such as `DawnEngine-26.1.1-Windows-x64.zip`.
5. Publish the release. It will appear in Dawn Hub's online versions list.

Only version tags beginning with `26.1` are shown by the current Dawn Hub online browser. Each installed version is stored side-by-side; existing installs are not overwritten.

## Important

A release entry without a Windows ZIP asset cannot be installed. Only upload binaries built from trusted source. This repository distributes builds; the engine source remains in `APGSwizzVR/DawnEngine`.