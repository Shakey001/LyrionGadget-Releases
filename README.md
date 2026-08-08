# Lyrion Gadget Releases

Public update feed and packaged releases for Lyrion Gadget owners.

- `update.json` is read by Advanced Setup.
- `packages/` contains versioned broker update packages.

## Lyrion piCorePlayer Player (32-bit)

The legacy-player package builds a player-only Lyrion appliance on official
32-bit piCorePlayer for Raspberry Pi Zero W and older Raspberry Pis. It keeps
the native pCP Squeezelite as Player 1 and supports up to three additional
local players. It does not install LMS, the Lyrion broker, RTI server features,
DietPi, or a Python web service.

- Current version: `0.9.17`
- Package: `packages/lyrion-picoreplayer-player-0.9.17.tgz`
- Update feed: `picoreplayer-player-update.json`
- Target: ARMv6/ARMv7 32-bit Raspberry Pi systems running piCorePlayer
- Setup page: `http://<player-address>:9099`
- Initial setup password: `LyrionGadget`

The setup page provides one-to-four-player provisioning, detected ALSA output
selection, USB/HDMI mixing, full Gadget/LMS discovery, managed `a0`-`a3` player MACs,
fixed-volume controls, hostname management through pCP's native reboot flow,
and the standard Lyrion Gadget visual theme.

The appliance advertises itself to Lyrion Gadget Finder as a `player_only`
unit over UDP port 9099. It does not answer broker/RTI discovery requests.

The development source is maintained separately in a private repository.
