# FnMacKickFix

Compatibility layer for running the Fortnite iOS binary on macOS (Apple Silicon).

## Installation

1. Download the latest `FnMacKickFix-V*.dylib` from [Releases](https://github.com/AlexGRDev/FnMacKickFix/releases/latest).

2. Inject it before launching Fortnite:

```bash
DYLD_INSERT_LIBRARIES=/path/to/FnMacKickFix-V1.0.0.dylib /path/to/FortniteClient-IOS-Shipping
```

3. (Optional) Create `$HOME/Documents/FnDiag.conf` to configure behavior:

```
relative_paths=true
patch_status=true
create_dirs=true
```

## Releases

| Channel | Description |
|---------|-------------|
| Stable (`v1.0.0`) | Recommended for normal use |
| Beta (`v1.0.0-beta`) | Verbose logging enabled, for debugging |

Each release includes a `manifest.json` used by the built-in auto-updater.

## Channels

Two distributions are available with identical functionality:

- **FnMacKickFix** — this repo
- **[FnMacUpdateFix](https://github.com/AlexGRDev/FnMacUpdateFix)** — alternate distribution

Both publish the same version simultaneously.
