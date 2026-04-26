# Co-opalypse Project Rules
- Engine: Godot
- Style: Realistic Survial, Open-world, zombies.

## Networking Rules
- Model: Client-Server (Dedicated or Listen Server).
- Authority: Server owns mechanical state and world; Clients own their own Player transforms.
- Sync: Use SceneReplicationConfig for high-frequency data (position/rotation).
- RPCs: Use `@rpc("any_peer", "call_remote", "reliable")` for interaction events.