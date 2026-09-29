# Public release verification

RaccoonOS 6.0.0 Public revision 25 is distributed as two raw parts that join into `raccoonos-6.0.0-public-r25-amd64.iso` (2,701,131,776 bytes). The assembled ISO SHA-256 is `ab9a5ae6d1924c619c87242ad55512b5af3bf49f15d9b1fa06334e3ea2846d8e`. The signed release checksum file lists both part hashes. Verify the release-key fingerprint `9E72550546933FD41FF2F553295A9061A70E7A13` before trusting its signature.

The exact final image passed the Public ISO verifier, including checks for Personal fonts and settings, readable RaccoonOS source, developer material, machine identity, home data, and the pinned update source. A QEMU live login reached the desktop with the documented Public credential. Debian package preflight covered 263 packages; the OS unit suite passed 1,146 tests.

An offline QEMU test installed a revision 25 candidate into encrypted LVM, booted it, reached the desktop, installed signed revision 26, rolled back, and recovered automatically from an interrupted update. A separate encrypted installation of the exact final ISO also passed disk unlock, first-boot cleanup, graphical login, and desktop rendering. These are VM checks; users should test graphics, input, Wi-Fi, audio, suspend and shutdown on their own hardware in the live session.

The signed Public update repository is published independently at <https://jonaskuusela393-ctrl.github.io/raccoonos-public-updates/>. The installed system checks its pinned signing key and Public profile before installing a RaccoonOS package. Debian's signed repositories provide base system packages.
