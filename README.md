# mc-bot

Minecraft bot framework in Almide. Handles authentication, login sequence, NeoForge handshake, and keep alive.

## Usage

```almide
import mc_bot

effect fn main() -> Unit =
  mc_bot.start({ ...mc_bot.DEFAULT_CONFIG, host: "localhost", port: 25565 })!
```

## Dependencies

- [mc-protocol](https://github.com/almd-mc/mc-protocol) — Packet-level protocol
- [mc-auth](https://github.com/almd-mc/mc-auth) — Microsoft/Xbox authentication
- [almide/sha1](https://github.com/almide/sha1) — Server hash (native)
- [almide/rsa](https://github.com/almide/rsa) — Login encryption
- [neoforge](https://github.com/almd-mc/neoforge) — NeoForge mod loader handshake
