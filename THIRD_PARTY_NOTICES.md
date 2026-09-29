# Third-party notices

The Windows preview does not bundle or download third-party Python packages. It uses Python and Tk/Tkinter from the user’s Python installation.

The Linux ISO is assembled from Debian 13 Stable packages under their respective licenses. Important upstream components include:

- Debian GNU/Linux and Debian Live
- Linux kernel
- systemd, AppArmor, nftables and NetworkManager
- greetd, tuigreet, Cage, GTK, and PyGObject
- labwc, wlroots, wlrctl, PyWayland, and Mako
- PipeWire, WirePlumber, pavucontrol, and the freedesktop sound theme
- FFmpeg/ffprobe and mpv local media decoding/rendering components
- Tk/Tkinter
- Firefox ESR
- PostgreSQL
- Git and GitHub CLI
- apt-offline and power-profiles-daemon
- GNOME Keyring and libsecret
- Podman, Buildah and Distrobox
- Poppler PDF tools and Kiwix/libzim offline ZIM reader (GPL-family licences)
- llama.cpp, downloaded from its official upstream only when the user explicitly runs the installer helper

RaccoonOS 6.0 Personal bundles the official amd64 `@openai/codex` 0.147.0 package
under its Apache-2.0 license so a clean reinstall reaches the tested local CLI
state without a network-time package substitution. User credentials, chats,
and authentication state are not bundled. The optional
`raccoonos-install-cloud-tools` helper can update Codex and install Vercel and
Neon CLIs into the current user's `~/.local` prefix after explicit confirmation.

RaccoonOS-owned source code, artwork, configuration, and documentation in this
archive are licensed under the RaccoonOS Personal Use License 1.0 unless a file
states otherwise. That license does not apply to, replace, or restrict any
third-party component. Copies validly received under an earlier MIT grant keep
the rights that grant already provided.

The generated `wlr-foreign-toplevel-management-unstable-v1` Python bindings
retain the protocol's permissive upstream copyright and license notice in the
generated source files.

Raccoon Maps bundles generalized Natural Earth 1:110m geography. Natural Earth
data is public domain; source and transformation details are retained in the
`maps-world` pack's `SOURCES.json` and README.

Raccoon Maps implements the public PMTiles version 3 archive specification and
Mapbox Vector Tile 2.1 wire/geometry specification with bounded RaccoonOS-owned
Python code. The PMTiles specification is public domain/CC0; the Mapbox Vector
Tile specification permits unrestricted implementation. No Protomaps planet,
font, sprite, JavaScript package, or CLI binary is bundled. If an operator adds
a Protomaps basemap, its tiles are an OpenStreetMap-derived ODbL Produced Work
and the map must display OpenStreetMap attribution. Other PMTiles publishers and
datasets retain their own terms. The software does not make a selected source
licensed, current, complete, or operationally safe.

After separate operator consent, Maps can fetch Geofabrik's public regional
index and one selected `*-latest.osm.pbf` extract to build a bounded saved area.
Geofabrik's service and data are not bundled. The resulting place and road
indexes derive from OpenStreetMap data and remain subject to the Open Database
License 1.0; Maps displays **OpenStreetMap contributors / ODbL 1.0** attribution
and retains the source URL, size, and SHA-256 provenance.

Raccoon Maps can, only after operator consent, request allow-listed NASA EOSDIS
GIBS products: Suomi NPP VIIRS true colour, IMERG 30-minute precipitation,
MODIS Terra cloud fraction, and ASTER GDEM elevation colour index. NASA
attribution is displayed with the layers. These are delayed Earth observations,
not live video, radar, or forecasts. Downloaded tiles are transient unless the
operator explicitly saves a visible VIIRS snapshot, which retains provenance.

Raccoon Maps can, only after separate operator consent, show Finnish road-camera
metadata and periodic still images from Fintraffic Digitraffic. That material is
licensed under Creative Commons Attribution 4.0. Required attribution:
**Fintraffic / digitraffic.fi · CC BY 4.0**. Provider terms are at
<https://www.digitraffic.fi/en/terms-of-service/>. Camera images are not bundled,
silently cached, or represented as live video.

Raccoon Chess uses the separately packaged Stockfish chess engine through its
UCI process interface. Stockfish is licensed under GPL-3.0-or-later; its NNUE
networks are supplied under CC0 by the Debian package. The package retains the
notices in `/usr/share/doc/stockfish/copyright` and system license texts.
Upstream source: <https://github.com/official-stockfish/Stockfish>;
Debian source package: <https://sources.debian.org/src/stockfish/>.
The generated chess artwork and locally synthesized sounds have provenance in
`assets/games/chess/ARTWORK.md` and `tools/generate-chess-sounds.py`.
