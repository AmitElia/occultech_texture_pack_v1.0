# Occultech texture pack

The resource pack of **Occultech**, a Slimefun addon of occult rituals, summoned bosses and relics (Minecraft 26.2).
Everything lives in its own `occultech` namespace: no vanilla item or block is retextured, so it works alongside any
other pack.

**This repository is generated - don't edit it by hand.** It is published from the addon's art pipeline
(`tools/art/build_pack.py` and `tools/art/publish_pack.py`).

| | |
|---|---|
| Download (what the server sends players) | `https://raw.githubusercontent.com/AmitElia/occultech_texture_pack_v1.0/main/occultech-pack.zip` |
| SHA-1 | `c6dab9ccf5ead11ebf86b0549697478064850593` |
| Size | 580 KiB |
| Item models | 127 (35 placed blocks with 3D skins) |
| Textures | 505 (203 animated) |
| Pack format | 88 (Minecraft 26.2) |
| Published | 2026-10-06 |

## Layout
- `occultech-pack.zip` - the pack itself; the server's `resource-pack.external-url` points at its raw link above.
  The server verifies the SHA-1, so this must be exactly the file built with the plugin.
- `pack/` - the same pack unzipped, for browsing textures and seeing what changed between versions.

## Server setup
In `plugins/Occultech/config.yml`:
```yaml
resource-pack:
  external-url: "https://raw.githubusercontent.com/AmitElia/occultech_texture_pack_v1.0/main/occultech-pack.zip"
```
After an update, push the new zip and wait a few minutes (GitHub caches raw files briefly) before restarting the
server.
