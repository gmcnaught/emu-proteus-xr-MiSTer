# Notices

E-mu Proteus/1 XR core. Copyright (c) 2026 The synthcores contributors.

The source is in https://github.com/gmcnaught/synthcores under `cores/proteus/` (paths below are
relative to that folder). This repository holds the built cores (`releases/*.rbf`), the MGL, the
tools that build the system image the core loads (`tools/`) and the documentation. Its history
before the move to synthcores still holds the source up to v0.2.0.

The core is licensed under the GNU General Public License v3.0 or later (`LICENSE`), except where a
file states otherwise.

| Component | Path in the source | Author / origin | License |
|---|---|---|---|
| fx68k 68000 core (unmodified) | `mister/rtl/fx68k/` | Jorge Cwik | GPL-3.0 |
| MiSTer framework (`sys/`) | `mister/sys/` | MiSTer-devel (Template_MiSTer) | GPL-2.0-or-later / GPL-3.0-or-later, per file |
| MAME changes (driver, sound device, MC68901) | `mame/patches/` | this project, against MAME | BSD-3-Clause (MAME per-file license) |
| Proteus core HDL, tools, docs | everything else | this project | GPL-3.0-or-later |

The HDL models of the MC68901 and HD44780 follow the behaviour of MAME's `mc68901` and `hd44780`
devices (BSD-3-Clause); no MAME source code is included in the HDL.

No ROM, firmware, sample or preset data is distributed. The core loads a system image that users
build from their own files (`tools/build_image.py`). E-mu, Proteus and ProtoLogic are trademarks of
their respective owners; this project is not affiliated with them.
