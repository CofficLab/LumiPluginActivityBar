# LumiPluginActivityBar

📖 English | [中文版](README_zh.md)

Lumi editor plugin.

> **Important rule: this plugin package must not depend on other plugin packages, and must not be depended on by other plugin packages.**
>
> Plugins communicate only through Provider contracts: shared capabilities go into `Provider*` / `Kit*` packages, assembled uniformly by the host (`Factory*`); cross-plugin references break independent plugin assembly and uninstallation.

## Package

- Product: `PluginActivityBar`
- Platform: macOS 14+
- Swift tools: 6.0

## What It Provides

<!-- TODO: describe what this package provides -->

## Dependencies and Integration

```swift
dependencies: [
    .package(url: "https://github.com/lumi-softworks/LumiPluginActivityBar.git", from: "1.0.0"),
],
targets: [
    .target(name: "YourTarget", dependencies: ["PluginActivityBar"]),
]
```

## Testing

From this package directory:

```sh
swift test
```

