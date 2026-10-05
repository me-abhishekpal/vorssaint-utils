# Intel (x86_64) build

This fork builds Vorssaint natively on Intel Macs. `build.sh` now targets the host architecture
(`uname -m`) instead of always targeting `arm64`; on Apple Silicon the result is unchanged.

```sh
./build.sh --dev --install
```

Tested: the app compiles and installs on an Intel (x86_64) Mac running macOS 26.

Not verified on Intel: sensor-based features (fan control, temperatures, GPU stats, battery details),
which rely on hardware access that differs from Apple Silicon.

This is an unofficial community build. See TRADEMARKS.md: the Vorssaint name and icon belong to the
upstream maintainer, and this fork carries no official identity.
