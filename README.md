# Flax Engine — Hardion Labs fork

[![Visual Studio extension](https://img.shields.io/badge/Visual%20Studio-extension-green.svg)](https://marketplace.visualstudio.com/items?itemName=Flax.FlaxVS)

**This repository is an unofficial public fork of [FlaxEngine/FlaxEngine](https://github.com/FlaxEngine/FlaxEngine).** It contains the Flax Engine source code and any changes maintained in this fork. It is not an official Flax Engine repository and is not endorsed by Flax or Wojciech Figat.

Flax Engine is a 3D game engine written in C++ and C#. The upstream project website is [flaxengine.com](https://flaxengine.com/).

> **Important — proprietary license:** The Flax Engine source code, editor and related content are governed by the [Flax Engine End User License Agreement (EULA)](https://flaxengine.com/licensing/), not by an OSI-approved open-source license. Making this repository public does not remove the EULA's restrictions or grant recipients unrestricted redistribution rights. Read [LICENSE.md](LICENSE.md) before using or distributing this code.

## Project links

- [Upstream repository](https://github.com/FlaxEngine/FlaxEngine)
- [Flax Engine website](https://flaxengine.com/)
- [Official documentation](https://docs.flaxengine.com/)
- [Official forum](https://forum.flaxengine.com/)
- [Official roadmap](https://trello.com/b/NQjLXRCP/flax-roadmap)
- [Fork-specific contribution guide](CONTRIBUTING.md)
- [Security policy](SECURITY.md)
- [Upstream and license notes](UPSTREAM.md)

## What this fork is

- A GitHub fork in the Flax Engine repository network, intended for changes that remain subject to the EULA.
- A place to maintain and review fork-specific changes.
- Not a replacement for the upstream project, its support channels, or its official releases.
- Not a grant to relicense Flax Engine under MIT, BSD, Apache-2.0, GPL, or another license.

Fork-specific changes should be clearly described in commits and pull requests. Unless explicitly stated otherwise, upstream functionality, names, notices, and third-party components retain their original ownership and licensing.

## Screenshots

![PBR rendering](Development/Images/flax-pic-2.jpg "PBR Rendering and Global Illumination")
![Rendering](Development/Images/flax-pic-1.jpg "Rendering")
![Performance](Development/Images/flax-pic-3.jpg "High Performance")

## Getting started

Follow the instructions below to compile and run the engine from source. These are the upstream build instructions; check the official documentation and the current CI configuration if a toolchain requirement changes.

### Windows

1. Install Visual Studio 2026 or newer.
2. Install the Windows 10 SDK or newer through Visual Studio Installer.
3. Install the Microsoft Visual C++ 2015 v140 toolset or newer.
4. Install the .NET 10 SDK or newer for Windows x64.
5. Install Git with Git LFS and run `git lfs install`.
6. Clone this repository with LFS files.
7. Run `GenerateProjectFiles.bat`.
8. Open `Flax.slnx`; select solution configuration `Editor.Development` and platform `Win64`.
9. Set `Flax` (C++) or `FlaxEngine` (C#) as the startup project.
10. Build and run the editor.

### Linux

Install the .NET 10 SDK, Vulkan development files, Git LFS, X11 development headers and Clang.

Fedora:

```bash
sudo dnf install dotnet-sdk-10.0 \
  vulkan-headers vulkan-tools vulkan-validation-layers \
  git git-lfs libX11-devel libXcursor-devel libXinerama-devel \
  zlib-ng-compat-devel clang llvm lldb lld
git lfs install
```

Ubuntu/Debian and Arch package names differ; consult the distribution documentation for the equivalent packages. Install the [Vulkan SDK](https://vulkan.lunarg.com/) where required by your build configuration.

Clone with LFS, generate project files, then build using the generated VS Code task:

```bash
git clone https://github.com/CeoMatheusDev/FlaxEngine.git
cd FlaxEngine
git lfs pull
./GenerateProjectFiles.sh
```

Use the `Flax|Editor.Linux.Development|x64` build task in Visual Studio Code.

### macOS

Install Xcode 16.4 or newer, the .NET 10 SDK or newer, the Vulkan SDK, and Git LFS. Clone this repository with LFS, run `GenerateProjectFiles.command`, then build the `Editor.Mac.Development` configuration in Xcode or Visual Studio Code.

## Repository layout

- `Binaries/` — executable files, including Editor and tool binaries.
- `Cache/` — local build and tool caches; normally generated locally.
- `Content/` — assets and binary content used by the engine and editor.
- `Development/` — development resources and helper scripts.
- `Source/Editor/` — editor source code.
- `Source/Engine/` — engine source code.
- `Source/Platforms/` — platform-specific code, dependencies and binaries.
- `Source/Shaders/` — shader sources.
- `Source/ThirdParty/` — third-party components and their license notices.
- `Source/Tools/` — build and development tools.

## Licensing and required notices

Use of Flax Engine is conditional on the [Flax Engine EULA](https://flaxengine.com/licensing/). In particular:

1. **Source and tools distribution:** public distribution of Engine Tools and modified Engine Tools must use the channels specified by the EULA. For public source distribution, the EULA identifies a fork in Flax's GitHub network. Other distribution is limited to the recipients and conditions described in the EULA.
2. **Product release notification:** before generating revenue from a Product or distributing it to end users, the EULA requires advance notification to Flax through [flaxengine.com/release](https://flaxengine.com/release).
3. **Royalties:** the standard EULA generally requires 4% of worldwide gross revenue attributable to each Product above the first US$250,000 per Product per calendar quarter, subject to the exclusions and reporting rules in the EULA. Reports and payments are generally due within 45 days after the applicable quarter.
4. **Product credits:** retain the proprietary notices in the source and content. Product credits must include the notices required by EULA section 6, with the year updated for the release:
   `[Product name] uses the Flax Engine`
   `Flax Engine, Copyright 2012 – [current year], Wojciech Figat. All rights reserved.`
5. **Third-party software:** individual components may have separate licenses. Preserve their notices and comply with each component's license. Do not assume the Flax EULA replaces third-party terms.
6. **License compatibility:** the EULA restricts combining Flax technology with certain non-compatible licenses. Review section 1(C) before adding dependencies or redistributing combined work.

The EULA may change. Always consult the current official text rather than relying solely on this summary. This README is informational and is not legal advice.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening an issue or pull request. Contributions to this fork must respect the EULA and all applicable third-party licenses. Submitting a change to this fork is not the same as submitting it to the upstream Flax project; the EULA contains a separate assignment provision for contributions made available to Flax.

## Disclaimer

“Flax” and “Flax Engine” are used only to identify the upstream technology on which this repository is based. All applicable trademarks and intellectual property remain with their respective owners. This fork is independently maintained and is not an official Flax release.
