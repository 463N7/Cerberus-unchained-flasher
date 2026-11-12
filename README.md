# Cerberus Unchained web flasher

[Open the flasher](https://463n7.github.io/Cerberus-unchained-flasher/) ·
[rev144 experimental release](https://github.com/463N7/Cerberus-unchained-flasher/releases/tag/v0.1.0-dev.rev144)

This repository contains only the built public installer, matched firmware
images, SD downloads, user guides and redistribution notices. Firmware source,
development history, pull requests, tests and board diagnostics are not included.

Use desktop Chrome or Edge with a production S3/C5 Cerberus and a USB data
cable. The installer checks all nine image hashes before any device write.
The selected pair is rev144 / C5 75, protocol 2. This remains experimental;
see the release notes for validation and service limits.

## SD card and manual uploads

The flasher's SD section provides the asset ZIP, checksum and copy instructions.
The existing rev136 pack remains compatible with rev144. The upload-profile
example is empty, with every service disabled. Keep completed profiles private.
See [the setup guide](https://463n7.github.io/Cerberus-unchained-flasher/guides/wardrive-uploads.html).

## Add GPS

[GPS wiring and receiver profiles](https://463n7.github.io/Cerberus-unchained-flasher/#gps-pinout)
are on the flasher page, below the SD section. Rev144 receives NMEA on S3 GPIO1
from the GPS module's TX output. Follow the supply/logic-level instructions for
your exact breakout. GPIO2 transmit and GPIO46 PPS are reserved and can remain
disconnected. LC29H reception/fix has been tested; ATGM336H has a firmware preset
but remains physically unverified.

## Credits and notices

Credit to the Sentinel foundation, @valleytechsolutions, JustCallMeKoko and
the [ESP32 Marauder contributors](https://github.com/justcallmekoko/ESP32Marauder).
Retain all included licenses and notices when redistributing.
[Complete distribution notices](notices.txt) include the retained ESP32 Marauder
MIT notice and the other firmware, installer, fonts and data notices. This
acknowledgment does not change those licenses or imply upstream endorsement.

## Publication

GitHub Pages serves the root of main with .nojekyll. Updates are reviewed,
validated static exports from the private development repository. Never push
firmware source/history, credentials, captures, reports or device backups here.
The site's JavaScript and firmware binaries are public downloads by design.
